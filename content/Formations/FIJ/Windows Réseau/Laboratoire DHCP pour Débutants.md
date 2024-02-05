---
date: 31-01-2024
Time: 23:38
---
# Laboratoire DHCP pour Débutants

## Objectif du Laboratoire

Le but de ce laboratoire est d'apprendre à configurer un serveur DHCP (Dynamic Host Configuration Protocol) sur un réseau local. Cela permettra aux périphériques du réseau d'obtenir automatiquement une adresse IP, un masque de sous-réseau, une passerelle par défaut, et d'autres informations réseau nécessaires.

## Prérequis

- Un ordinateur fonctionnant sous un système d'exploitation compatible avec la configuration d'un serveur DHCP (par exemple, Windows ou Linux).
- Un réseau local avec au moins un périphérique client (ordinateur, portable, etc.).
- Accès administratif à l'ordinateur qui servira de serveur DHCP.

## Étapes du Laboratoire

### Étape 1: Vérifier la Configuration du Serveur

Assurez-vous que l'ordinateur qui servira de serveur DHCP est correctement connecté au réseau et dispose d'une configuration réseau valide. Notez l'adresse IP actuelle de cet ordinateur.

### Étape 2: Installer le Service DHCP

1. Sur Windows :
    
    - Sur les systèmes d'exploitation Windows Server, installez le rôle "Serveur DHCP" via le Gestionnaire de serveur.
    - Sur les systèmes d'exploitation Windows non serveur, utilisez des outils tiers tels que "Internet Information Services (IIS)".
2. Sur Linux :
    
    - Sur les distributions basées sur Debian (comme Ubuntu), installez le paquet "isc-dhcp-server".
    - Sur les distributions basées sur Red Hat (comme Fedora), installez le paquet "dhcp".

### Étape 3: Configurer le Serveur DHCP

1. Sur Windows :
    
    - Ouvrez l'outil "Gestionnaire DHCP" depuis le Gestionnaire de serveur.
    - Sélectionnez le serveur dans l'arborescence et configurez les options telles que les plages d'adresses IP, le masque de sous-réseau, la passerelle, etc.
2. Sur Linux :
    
    - Éditez le fichier de configuration du serveur DHCP, généralement situé à "/etc/dhcp/dhcpd.conf". Configurez les options telles que les plages d'adresses IP, le masque de sous-réseau, la passerelle, etc.

### Étape 4: Redémarrer le Service DHCP

1. Sur Windows :
    
    - Redémarrez le service "Serveur DHCP" à partir de la console "Services" ou utilisez la commande PowerShell : `Restart-Service dhcpserver`.
2. Sur Linux :
    
    - Redémarrez le service DHCP avec la commande : `sudo service isc-dhcp-server restart` (ou utilisez le gestionnaire de service spécifique à votre distribution).

### Étape 5: Vérifier l'Attribution d'Adresses IP

1. Sur le périphérique client :
    
    - Configurez l'interface réseau en mode DHCP ou assurez-vous que la configuration réseau est en mode automatique.
    - Redémarrez l'interface réseau ou le périphérique si nécessaire.
2. Vérifiez si le périphérique client obtient une adresse IP attribuée par le serveur DHCP. Sur Windows, utilisez la commande `ipconfig` dans l'invite de commandes. Sur Linux, utilisez `ifconfig` ou `ip a`.
    

## Points à Noter

- Assurez-vous que le serveur DHCP et le périphérique client sont sur le même sous-réseau.
- Veillez à désactiver tout autre service DHCP sur le réseau pour éviter les conflits.
- Si des erreurs surviennent, consultez les journaux du serveur DHCP pour diagnostiquer et résoudre les problèmes.

Ce laboratoire simple devrait fournir une introduction pratique à la configuration d'un serveur DHCP pour les débutants. N'hésitez pas à explorer davantage en ajoutant des fonctionnalités ou en ajustant les paramètres pour mieux comprendre le fonctionnement du service DHCP.