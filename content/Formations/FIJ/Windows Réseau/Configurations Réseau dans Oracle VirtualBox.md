---
date: 2024-01-09
---
# Réseaux dans Oracle VirtualBox

## NAT (Network Address Translation)

- **Description** : La machine virtuelle est comme derrière un routeur. Elle accède à Internet via l'adresse IP de votre ordinateur réel, restant invisible de l'extérieur.
    
- **Utilité** : Pratique pour une navigation sur Internet sécurisée sans être directement accessible.
    
- **Scénario Pratique** : Configuration idéale pour un serveur web interne nécessitant un accès à Internet pour les mises à jour.
    
- **Fonctionnement** : Lorsque la machine virtuelle envoie des demandes à Internet, l'adresse IP source est modifiée par celle de l'ordinateur hôte grâce à la traduction d'adresse réseau (NAT). Les réponses reviennent à l'ordinateur hôte qui transmet ensuite à la machine virtuelle.
    
![[imgVirtualBoxNat.jpg]]

## Bridged Adapter

- **Description** : La machine virtuelle se connecte directement au réseau local comme un appareil réel. Elle possède sa propre adresse IP et peut être vue par d'autres appareils.
    
- **Utilité** : Idéal pour tester des applications nécessitant une visibilité dans le réseau local.
    
- **Scénario Pratique** : Parfait pour le développement et le test d'applications nécessitant une interaction avec d'autres machines du réseau local.
    
- **Fonctionnement** : La machine virtuelle est comme un appareil physique sur le réseau local. Elle obtient une adresse IP directement depuis le routeur, permettant une communication transparente avec d'autres dispositifs du réseau local.
    
![[imgVirtualBoxBridged.jpg]]
## Internal Network

- **Description** : Crée un espace réseau isolé où les machines virtuelles peuvent communiquer entre elles uniquement.
    
- **Utilité** : Parfait pour des tests isolés sans accès externe, pour simuler un réseau privé.
    
- **Scénario Pratique** : Configuration adaptée pour simuler un environnement d'entreprise isolé pour le développement et les tests.
    
- **Fonctionnement** : Les machines virtuelles connectées à un réseau interne peuvent se communiquer entre elles, mais aucune connexion externe n'est autorisée. Idéal pour tester des scénarios privés.
    
![[imgVirtualBoxInternal.jpg]]
## Host-only Adapter

- **Description** : Établit un réseau isolé entre votre ordinateur hôte et les machines virtuelles.
    
- **Utilité** : Pour des communications internes entre les machines virtuelles et l'ordinateur hôte sans accès Internet.
    
- **Scénario Pratique** : Utilisé pour la configuration d'un serveur de base de données accessible uniquement depuis l'ordinateur hôte.
    
- **Fonctionnement** : Les machines virtuelles peuvent communiquer uniquement avec l'ordinateur hôte, créant un réseau isolé. Aucune connexion externe n'est autorisée.
    
![[imgVirtualBoxHostOnly.jpg]]
## NAT Network

- **Description** : Crée un réseau privé où plusieurs machines virtuelles partagent une connexion à Internet via une interface NAT commune.
    
- **Utilité** : Pratique pour établir un réseau privé avec accès Internet pour les machines virtuelles.
    
- **Scénario Pratique** : Configuration utile pour un laboratoire de test où plusieurs machines virtuelles nécessitent un accès à Internet.
    
- **Fonctionnement** : Les machines virtuelles peuvent se communiquer entre elles dans un réseau privé et partagent une connexion à Internet via une interface NAT commune.
    
![[imgVirtualBoxNatNetwork.jpg]]
## Generic Driver Cloud Network

- **Description** : Pilotes réseau pour se connecter à des services cloud ou à des réseaux basés sur des normes génériques.
    
- **Utilité** : Utilisé pour une connectivité spécifique à certains services ou environnements cloud.
    
- **Scénario Pratique** : Configuré pour se connecter à des services cloud tels qu'Azure ou AWS pour des tests de déploiement.
    
- **Fonctionnement** : Les pilotes génériques permettent aux machines virtuelles de se connecter à des services cloud, simulant une connectivité à des environnements cloud spécifiques.
    

## NAT Attached

- **Description** : Permet de lier une machine virtuelle à une interface NAT spécifique pour une communication précise dans des configurations avancées.
    
- **Utilité** : Pour des configurations réseau complexes nécessitant un contrôle précis.
    
- **Scénario Pratique** : Configuration avancée pour des situations spécifiques nécessitant une gestion fine du trafic réseau.
    
- **Fonctionnement** : Cette configuration permet de contrôler précisément la communication de la machine virtuelle en la reliant à une interface NAT spécifique.
    

## Paramètres Avancés :

### Promiscuous Mode

- **Description** : Permet à une machine virtuelle d'écouter tout le trafic réseau. À utiliser avec précaution pour éviter des risques de sécurité.
    
- **Scénario Pratique** : Utilisé dans des cas de débogage ou d'analyse de réseau avancés.
    
- **Fonctionnement** : La machine virtuelle peut écouter tout le trafic sur le réseau, permettant des analyses détaillées mais nécessitant une précaution accrue pour éviter des risques de sécurité.
    

### MAC Address Spoofing

- **Description** : Change l'adresse MAC de la carte réseau virtuelle. Utile pour simuler une autre carte réseau physique.
    
- **Scénario Pratique** : Configuration pour tester des scénarios où l'adresse MAC doit être modifiée pour des raisons spécifiques.
    
-  **Fonctionnement** : Permet de changer l'adresse MAC de la machine virtuelle, utile pour simuler des scénarios où une autre carte réseau physique est utilisée.
    

## Réglages Additionnels :

### Réseau sans fil (Wireless)

- **Description** : Autorise la machine virtuelle à utiliser la connexion Wi-Fi de l'ordinateur hôte, si disponible.
    
- **Scénario Pratique** : Utile pour les tests sur des réseaux sans fil ou pour simuler des environnements avec une connexion Wi-Fi.
    
- **Fonctionnement** : Permet à la machine virtuelle d'utiliser la connexion Wi-Fi de l'ordinateur hôte, simulant une connexion sans fil.
    

### Qualité de Service (QoS)

- **Description** : Limite la vitesse de transfert de données de la machine virtuelle sur le réseau. Utile pour contrôler la bande passante utilisée.
    
- **Scénario Pratique** : Configuration pour tester des applications nécessitant une limitation de la bande passante.
    
-  **Fonctionnement** : Limite la vitesse de transfert de données de la machine virtuelle, permettant de contrôler la bande passante utilisée dans des scénarios spécifiques.