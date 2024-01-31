---
date: 2024-01-31
---
# Processus de Location d'Adresses DHCP

Le processus de location d'adresses DHCP est une étape cruciale dans le fonctionnement du protocole DHCP. Il implique plusieurs étapes pour permettre à un appareil de recevoir une adresse IP dynamiquement. Voici une explication détaillée :

1. **Requête de Diffusion (Discover) :**
    
    - Lorsqu'un appareil rejoint le réseau ou a besoin d'une nouvelle adresse IP, il envoie une requête de diffusion DHCP (DHCP Discover) sur le réseau.
    - Cette requête est généralement diffusée à tous les serveurs DHCP disponibles dans le réseau.
2. **Offre de Serveur (Offer) :**
    
    - Les serveurs DHCP du réseau reçoivent la requête de diffusion et répondent avec une offre DHCP (DHCP Offer).
    - Chaque offre contient une adresse IP disponible, la durée de la location (lease), et d'autres paramètres de configuration.
3. **Requête de Demande (Request) :**
    
    - L'appareil DHCP, après avoir reçu plusieurs offres, sélectionne l'une d'entre elles et envoie une requête de demande DHCP (DHCP Request) au serveur choisi.
    - Cette étape confirme le choix de l'adresse IP par le client.
4. **Accord (Acknowledge) :**
    
    - Le serveur DHCP qui a reçu la requête de demande envoie un accord DHCP (DHCP Acknowledge) au client.
    - Cet accord confirme l'attribution de l'adresse IP au client pour la durée spécifiée.
5. **Renouvellement de la Location :**
    
    - Pendant la période de location, le client peut renouveler l'attribution de l'adresse IP en envoyant une requête de renouvellement DHCP au serveur.
    - Le serveur peut accorder le renouvellement ou attribuer une nouvelle adresse IP.
6. **Libération de la Location :**
    
    - Lorsque l'appareil n'a plus besoin de l'adresse IP ou quitte le réseau, il envoie une requête de libération DHCP (DHCP Release) au serveur pour indiquer que l'adresse IP peut être réutilisée.

Ce processus garantit une attribution efficace et dynamique des adresses IP, facilitant la gestion des réseaux et l'adaptation aux changements de configuration.