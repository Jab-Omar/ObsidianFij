---
date: 2023-12-30
---

# Gestion des Utilisateurs et Groupes sur Linux

## Introduction

La gestion des utilisateurs et groupes sur Linux est fondamentale pour contrôler l'accès aux ressources système. Cela implique la création, la modification et la suppression d'utilisateurs et de groupes, ainsi que l'attribution des autorisations appropriées.

## Utilisateurs

### Concepts Clés

- **UID (User ID)** : Identifiant unique pour chaque utilisateur.
- **Login Shell** : Interpréteur de commandes utilisé lors de la connexion.
- **Home Directory** : Répertoire personnel de l'utilisateur.
- **GECOS** : Informations supplémentaires sur l'utilisateur (nom, numéro de téléphone, etc.).

### Types d'Utilisateurs

1. **Utilisateur Standard** :
    - UID généralement supérieur à 1000.
    - Utilisé pour les opérations quotidiennes.
2. **Utilisateur Système** :
    - UID inférieur à 1000.
    - Utilisé pour les services et processus système.
3. **Utilisateur Root** :
    - UID 0.
    - Dispose de privilèges administratifs complets.

### Fichiers Liés

- `/etc/passwd` : Informations des utilisateurs.
- `/etc/shadow` : Stocke les mots de passe chiffrés.
- `/etc/group` : Liste des groupes disponibles.
- `/etc/gshadow` : Mots de passe chiffrés des groupes.

## Commandes et Utilisation

1. `useradd` : Crée un nouvel utilisateur.
    - Utilisé dans les distributions RedHat.
2. `adduser` : Crée un nouvel utilisateur.
    - Utilisé dans les distributions Ubuntu.
3. `id` : Affiche les informations d'un utilisateur.
4. `passwd` : Définit ou réinitialise le mot de passe d'un utilisateur.
5. `usermod` : Modifie les détails d'un utilisateur existant.
6. `userdel -r` : Supprime un utilisateur, y compris son répertoire personnel.

## Groupes

### Concepts Clés

- **GID (Group ID)** : Identifiant unique pour chaque groupe.
- **Groupe Principal** : Groupe par défaut de l'utilisateur.
- **Groupes Supplémentaires** : Groupes auxquels un utilisateur peut appartenir en plus du groupe principal.

### Fichiers Liés

- Mêmes fichiers que pour les utilisateurs.

## Commandes et Utilisation

1. `groupadd` : Crée un nouveau groupe.
2. `groupdel` : Supprime un groupe.
3. `usermod -G` : Ajoute un utilisateur à un groupe existant.

## Propriétés des Fichiers et Processus

- Chaque fichier est associé à un propriétaire et à un groupe.
- Les processus en cours ont également un propriétaire et un groupe, déterminant leurs autorisations d'accès.

## Commandes Utiles

- `last` : Affiche les dernières connexions au système.
- `who` : Montre les utilisateurs connectés.
- `whoami` : Affiche l'utilisateur courant.
- `lsof -u user` : Liste les fichiers ouverts par un utilisateur spécifique.

## Conclusion

La gestion appropriée des utilisateurs et groupes sur Linux est essentielle pour assurer la sécurité et la gestion des ressources système. Ces commandes et fichiers permettent un contrôle précis des accès et des autorisations.