---
date: 2023-12-30
---

# Gestion avancée de Sudo (sudoers)

## Introduction à Sudo

Sudo, raccourci de "substitute user do", permet aux administrateurs système d'autoriser des utilisateurs ou des groupes à exécuter des commandes spécifiques avec des privilèges d'administration.

### Utilisation basique de Sudo

Utilisé en ligne de commande dans un terminal pour accéder aux droits root, il requiert le mot de passe de l'utilisateur invoquant Sudo.

```bash
$ sudo commande
```

### Durée de validité du mot de passe

Le mot de passe est mémorisé pendant 15 minutes par défaut pour des commandes ultérieures sans redemander le mot de passe.

### Oublier le mot de passe mémorisé

Pour "oublier" le mot de passe mémorisé avant la fin des 15 minutes :

```bash
$ sudo -k
```

### Session "root" avec Sudo

Pour ouvrir une session "root" avec Sudo :

```bash
$ sudo -i
```

Cette méthode demande le mot de passe de l'utilisateur.

## Configuration de Sudo via sudoers

- Les autorisations pour Sudo sont définies dans `/etc/sudoers`.
- Utiliser `visudo` pour éditer ce fichier, cela vérifie la syntaxe avant d'enregistrer.

### Syntaxe de configuration

Chaque ligne dans le fichier sudoers suit cette structure :

```bash
user/groupe cibles = (utilisateur à imiter) commandes
```

- `user/groupe`: nom d'utilisateur ou groupe (précédé de `%` pour les groupes).
- `cibles`: les machines concernées (normalement `ALL`).
- `(utilisateur à imiter)`: `ALL` pour tous, y compris root.
- `commandes`: commandes autorisées, chemin complet requis. Ajouter `!` devant pour les interdire.

## Utilisation sans mot de passe

- Bien que risqué, cela peut être utile pour des scripts spécifiques.

Exemple :

```bash
user ALL = (ALL) NOPASSWD: commandes
```

## Exemples pratiques

### Autoriser Apache à lancer "service" sans mot de passe :

```bash
apache ALL=(ALL) NOPASSWD: /usr/sbin/service
```

### Autoriser l'utilisateur "adrien" à exécuter toutes les commandes via Sudo :

```bash
adrien ALL=(ALL) ALL
```

### Autoriser "adrien" à utiliser "sudo reboot" sans mot de passe :

```bash
adrien ALL=(ALL) NOPASSWD: /usr/sbin/reboot
```

### Autoriser le groupe "devteam" à utiliser certaines commandes sans mot de passe :

```bash
%devteam ALL=(ALL) NOPASSWD: /path/to/command1, /path/to/command2
```
