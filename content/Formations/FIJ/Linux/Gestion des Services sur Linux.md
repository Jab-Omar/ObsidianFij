---
date: 2023-12-30
---

# Services dans Linux : Commandes Systemctl

## Syntaxe de Base
- **Start**: Démarre un service spécifique.
  ```bash
  sudo systemctl start nom_service
  ```
- **Stop**: Arrête un service spécifique.
  ```bash
  sudo systemctl stop nom_service
  ```
- **Restart**: Redémarre un service spécifique.
  ```bash
  sudo systemctl restart nom_service
  ```
- **Status**: Affiche le statut actuel d'un service.
  ```bash
  sudo systemctl status nom_service
  ```
- **Reload**: Recharge la configuration d'un service sans redémarrage complet.
  ```bash
  sudo systemctl reload nom_service
  ```

## Gestion au Démarrage
- **Enable**: Démarre un service automatiquement au démarrage du système.
  ```bash
  sudo systemctl enable nom_service
  ```
- **Disable**: Empêche le démarrage automatique d'un service au démarrage du système.
  ```bash
  sudo systemctl disable nom_service
  ```

## Commandes Spécifiques pour Ubuntu 20
- **is-active**: Affiche si le service est actif ou non.
  ```bash
  sudo systemctl is-active nom_service
  ```
- **is-enabled**: Indique si le service est activé pour démarrer au démarrage.
  ```bash
  sudo systemctl is-enabled nom_service
  ```

Ces commandes, exécutées avec `systemctl`, permettent de contrôler le démarrage, l'arrêt, le redémarrage et la vérification de l'état des services dans un environnement Linux.