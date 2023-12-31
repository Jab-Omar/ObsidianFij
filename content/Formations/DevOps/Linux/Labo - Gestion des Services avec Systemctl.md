# Laboratoire : Gestion des Services avec Systemctl

## Objectif :

Apprendre à utiliser les commandes `systemctl` pour contrôler les services sous Linux.
## Prérequis :

- Accès à un système Linux (Ubuntu, CentOS, etc.).
- Autorisations administratives (utilisateur avec droits sudo).
## Étapes :

### Gestion des Services de Base

- **Démarrer un service :**
    - Choisis un service (par exemple `ssh`, `apache2`, `nginx`) et démarre-le avec `sudo systemctl start nom_du_service`.
- **Arrêter un service :**
    - Arrête le même service avec `sudo systemctl stop nom_du_service`.
- **Redémarrer un service :**
    - Redémarre le service précédent avec `sudo systemctl restart nom_du_service`.
- **Vérifier le statut d'un service :**
    - Utilise `sudo systemctl status nom_du_service` pour vérifier l'état actuel du service.
- **Recharger la configuration d'un service :**
    - Choisis un service (comme `nginx`) et recharge sa configuration sans redémarrer avec `sudo systemctl reload nom_du_service`.
### Gestion du Démarrage des Services

- **Activer le démarrage automatique :**
    - Active un service pour qu'il démarre automatiquement au démarrage du système avec `sudo systemctl enable nom_du_service`.
- **Désactiver le démarrage automatique :**
    - Désactive le même service pour qu'il ne démarre pas automatiquement avec `sudo systemctl disable nom_du_service`.
### Commandes spécifiques pour Ubuntu 20 (optionnel)

- **Vérifier si le service est actif :**
    - Utilise `sudo systemctl is-active nom_du_service` pour vérifier si le service est actif.
- **Vérifier si le service est activé au démarrage :**
    - Utilise `sudo systemctl is-enabled nom_du_service` pour vérifier si le service est activé au démarrage.
## Conclusion :

Résume l'expérience en mettant en évidence l'utilisation pratique des commandes `systemctl` pour contrôler les services. Mentionne l'importance de ces commandes dans l'administration système sous Linux.