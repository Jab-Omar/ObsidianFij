---
date: 2023-11-13
---
# Configuration d'un proxy sur un poste de travail

## 1. Configuration Globale dans les Options Internet

### Windows 11

- **Description :** Cette méthode permet de configurer le proxy au niveau du système d'exploitation, affectant ainsi l'ensemble des applications qui utilisent les paramètres système.
- **Procédure :**
    - Accéder aux "Paramètres".
    - Sélectionner "Réseau et Internet".
    - Aller à l'onglet "Proxy".
    - Cliquer sur "Configurer" à côté de "Utiliser un serveur proxy".
    - Renseigner l'adresse du proxy.

## 2. Configuration par Application

### Exemple avec Firefox

- **Description :** Certains navigateurs, comme Firefox, offrent une gestion interne du proxy, permettant des configurations spécifiques par logiciel.
- **Procédure :**
    - Dans Firefox, accéder aux "Options".
    - Aller à l'onglet "Général".
    - Sous "Paramètres réseau" dans la section "Paramètres", configurer les proxies.

## 3. Configuration Automatisée pour un Parc Informatique

### Utilisation de GPO (Stratégie de Groupe)

- **Description :** Les administrateurs peuvent déployer les paramètres de configuration du proxy sur l'ensemble d'un réseau en utilisant les GPO, ce qui offre une gestion centralisée.
- **Procédure :**
    - Utiliser une GPO pour déployer les paramètres du proxy au niveau de Windows ou des navigateurs.

### Utilisation d'un Script d'Auto-Configuration (PAC)

- **Description :** Un script d'auto-configuration, généralement en JavaScript et portant l'extension PAC, offre une flexibilité supplémentaire en déterminant dynamiquement si une connexion doit passer par le proxy en fonction de l'URL.
- **Procédure :**
    - Utiliser une GPO pour spécifier l'emplacement d'un script "proxy.pac" qui contient la fonction JavaScript "FindProxyForURL".

Ces différentes approches offrent aux administrateurs des options flexibles pour configurer les proxies sur les postes de travail, en fonction des besoins spécifiques de l'entreprise, de la sécurité et de la gestion du réseau.