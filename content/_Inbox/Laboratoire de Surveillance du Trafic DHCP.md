---
date: 31-01-2024
Time: 23:46
---
# Laboratoire de Surveillance du Trafic DHCP

## Objectif du Laboratoire
Ce laboratoire a pour objectif de vous familiariser avec la surveillance du trafic DHCP en utilisant un outil tel que Wireshark. Vous allez capturer le trafic réseau entre les clients et le serveur DHCP, puis analyser les échanges pour comprendre les différentes étapes du processus d'attribution dynamique d'adresses IP.

## Prérequis
- Un réseau fonctionnel avec un serveur DHCP et au moins un client.
- Wireshark (ou un outil équivalent) installé sur une machine capable de capturer le trafic sur le réseau.

## Étapes du Laboratoire

### Étape 1: Configuration de Wireshark
1. Assurez-vous que Wireshark est installé sur la machine que vous allez utiliser pour la capture du trafic.
2. Lancez Wireshark et sélectionnez l'interface réseau à surveiller.

### Étape 2: Capture du Trafic DHCP
1. Commencez la capture dans Wireshark.
2. Demandez au client de renouveler son bail DHCP en utilisant la commande `ipconfig /renew` (sous Windows) ou l'équivalent sur d'autres systèmes d'exploitation.
3. Arrêtez la capture après avoir observé suffisamment d'échanges DHCP.

### Étape 3: Analyse du Trafic
1. Examinez la capture dans Wireshark pour identifier les paquets DHCP.
   - Filtrez les paquets DHCP en utilisant le filtre `dhcp` dans la barre de filtrage.
2. Identifiez les différentes étapes du processus d'attribution dynamique d'adresses IP, notamment :
   - Découverte DHCP (DHCP Discover)
   - Offre DHCP (DHCP Offer)
   - Demande DHCP (DHCP Request)
   - Attribution DHCP (DHCP Acknowledgment)
3. Notez les adresses IP source et destination, les options DHCP, les identifiants de transaction, etc.

### Étape 4: Compréhension des Échanges
1. Analysez le contenu des paquets DHCP pour comprendre comment les clients et le serveur communiquent.
2. Identifiez les informations clés telles que les adresses IP attribuées, les options spécifiques et les détails des transactions DHCP.

### Étape 5: Réflexion sur le Processus
1. Réfléchissez à la manière dont le processus d'attribution dynamique d'adresses IP via DHCP fonctionne en examinant les échanges capturés.
2. Notez les avantages de chaque étape du processus pour le client et le serveur DHCP.

## Points à Noter
- L'analyse du trafic DHCP avec Wireshark offre une vision détaillée du processus d'attribution d'adresses IP.
- Les identifiants de transaction DHCP sont cruciaux pour associer les messages correspondants entre les clients et le serveur DHCP.
- Comprendre le processus DHCP est essentiel pour diagnostiquer les problèmes de configuration réseau.

Ce laboratoire vous permettra de visualiser et de comprendre concrètement le trafic DHCP à l'aide d'outils de surveillance réseau. Cela renforce votre compréhension du fonctionnement du protocole DHCP dans un environnement réseau.