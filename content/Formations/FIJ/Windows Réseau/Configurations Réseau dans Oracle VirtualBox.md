---
date: 2024-01-09
---
# Configurations Réseau dans Oracle VirtualBox
## NAT (Network Address Translation)

- **Description** : La machine virtuelle est comme derrière un routeur. Elle accède à Internet via l'adresse IP de votre ordinateur réel, restant invisible de l'extérieur.
- **Utilité** : Pratique pour une navigation sur Internet sécurisée sans être directement accessible.

## Bridged Adapter

- **Description** : La machine virtuelle se connecte directement au réseau local comme un appareil réel. Elle possède sa propre adresse IP et peut être vue par d'autres appareils.
- **Utilité** : Idéal pour tester des applications nécessitant une visibilité dans le réseau local.

## Internal Network

- **Description** : Crée un espace réseau isolé où les machines virtuelles peuvent communiquer entre elles uniquement.
- **Utilité** : Parfait pour des tests isolés sans accès externe, pour simuler un réseau privé.

## Host-only Adapter

- **Description** : Établit un réseau isolé entre votre ordinateur hôte et les machines virtuelles.
- **Utilité** : Pour des communications internes entre les machines virtuelles et l'ordinateur hôte sans accès Internet.

## NAT Network

- **Description** : Crée un réseau privé où plusieurs machines virtuelles partagent une connexion à Internet via une interface NAT commune.
- **Utilité** : Pratique pour établir un réseau privé avec accès Internet pour les machines virtuelles.

## Generic Driver Cloud Network

- **Description** : Pilotes réseau pour se connecter à des services cloud ou à des réseaux basés sur des normes génériques.
- **Utilité** : Utilisé pour une connectivité spécifique à certains services ou environnements cloud.

## NAT Attached

- **Description** : Permet de lier une machine virtuelle à une interface NAT spécifique pour une communication précise dans des configurations avancées.
- **Utilité** : Pour des configurations réseau complexes nécessitant un contrôle précis.

## Paramètres Avancés :

### Promiscuous Mode

- **Description** : Permet à une machine virtuelle d'écouter tout le trafic réseau. À utiliser avec précaution pour éviter des risques de sécurité.

### MAC Address Spoofing

- **Description** : Change l'adresse MAC de la carte réseau virtuelle. Utile pour simuler une autre carte réseau physique.

## Réglages Additionnels :

### Réseau sans fil (Wireless)

- **Description** : Autorise la machine virtuelle à utiliser la connexion Wi-Fi de l'ordinateur hôte, si disponible.

### Qualité de Service (QoS)

- **Description** : Limite la vitesse de transfert de données de la machine virtuelle sur le réseau. Utile pour contrôler la bande passante utilisée.