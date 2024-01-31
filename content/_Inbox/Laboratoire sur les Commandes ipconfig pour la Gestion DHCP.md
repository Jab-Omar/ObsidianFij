---
date: 31-01-2024
Time: 23:41
---
# Laboratoire sur les Commandes ipconfig pour la Gestion DHCP

## Objectif du Laboratoire

Ce laboratoire vise à familiariser les utilisateurs avec les commandes `ipconfig` sous Windows pour la gestion des configurations réseau, en mettant particulièrement l'accent sur les commandes `release` et `renew` pour travailler avec un serveur DHCP (Dynamic Host Configuration Protocol).

## Prérequis

- Un ordinateur sous Windows avec une interface réseau connectée à un réseau DHCP.
- Accès administratif à l'ordinateur.

## Étapes du Laboratoire

### Étape 1: Vérification de la Configuration Actuelle

1. Ouvrez l'invite de commandes en tant qu'administrateur (clic droit sur le menu Démarrer -> Invite de commandes (Admin)).
2. Exécutez la commande `ipconfig` pour afficher les informations actuelles de configuration réseau.

### Étape 2: Libération de l'Adresse IP Actuelle

1. Exécutez la commande `ipconfig /release` pour libérer l'adresse IP actuelle attribuée par le serveur DHCP.
2. Vérifiez à nouveau la configuration réseau avec `ipconfig`. Notez que l'adresse IP devrait être indiquée comme "Aucune configuration IP".

### Étape 3: Renouvellement de l'Adresse IP

1. Exécutez la commande `ipconfig /renew` pour demander au système d'obtenir une nouvelle adresse IP auprès du serveur DHCP.
2. Vérifiez à nouveau la configuration réseau avec `ipconfig`. Notez la nouvelle adresse IP attribuée par le serveur DHCP.

### Étape 4: Compréhension des Commandes

1. Explorez les options supplémentaires de `ipconfig` en utilisant `ipconfig /?`.
2. Comprenez le rôle des commandes `release` et `renew` dans la gestion de la configuration DHCP.

## Points à Noter

- La commande `ipconfig /release` libère toutes les adresses IPv4 configurées sur toutes les interfaces réseau.
- La commande `ipconfig /renew` demande une nouvelle configuration DHCP pour toutes les interfaces réseau.

Ce laboratoire démontre l'utilisation des commandes `ipconfig /release` et `ipconfig /renew` pour gérer la configuration DHCP sous Windows. Comprendre ces commandes est essentiel pour diagnostiquer et résoudre les problèmes de configuration réseau liés au DHCP.