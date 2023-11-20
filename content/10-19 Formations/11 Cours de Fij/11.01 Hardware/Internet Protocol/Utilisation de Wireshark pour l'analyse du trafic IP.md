---
date: 2023-11-09
---
Wireshark est un outil puissant d'analyse de paquets réseau qui permet de capturer et d'inspecter le trafic IP sur un réseau. Voici comment utiliser Wireshark pour l'analyse du trafic IP :

## 1. **Téléchargement et Installation de Wireshark :**

Avant de commencer, téléchargez et installez Wireshark à partir du site officiel : [Wireshark Download](https://www.wireshark.org/download.html).

## 2. **Lancement de Wireshark :**

Après l'installation, lancez Wireshark. Sur de nombreux systèmes, il peut nécessiter des privilèges d'administration pour capturer le trafic.

## 3. **Sélection de l'Interface Réseau :**

Une fois Wireshark ouvert, sélectionnez l'interface réseau que vous souhaitez surveiller. Cliquez sur l'icône de la carte réseau et choisissez l'interface appropriée.

## 4. **Démarrage de la Capture :**

Cliquez sur le bouton "Démarrer la capture" (icône du lecteur de médias) pour commencer à capturer le trafic sur l'interface sélectionnée.

## 5. **Analyse du Trafic IP :**

Pendant la capture, Wireshark affiche une liste détaillée des paquets capturés. Vous pouvez appliquer des filtres pour se concentrer sur le trafic IP spécifique.

- Utilisez le filtre `ip` pour filtrer uniquement les paquets IP.
- Pour un filtrage plus spécifique, utilisez des filtres tels que `ip.src == adresse_IP_source` ou `ip.dst == adresse_IP_destination`.

## 6. **Inspection des Paquets :**

Double-cliquez sur un paquet pour afficher les détails. Vous pouvez explorer chaque couche du modèle OSI pour comprendre la structure du paquet.

## 7. **Analyse des Statistiques :**

Wireshark offre des fonctionnalités de statistiques pour analyser le trafic.

- Allez dans "Statistics" > "Summary" pour obtenir une vue d'ensemble du trafic.
- "Statistics" > "Protocol Hierarchy" affiche une ventilation par protocole.

## 8. **Arrêt de la Capture :**

Lorsque vous avez capturé suffisamment de données, cliquez sur le bouton "Arrêter la capture" (icône du lecteur de médias).

## 9. **Enregistrement des Données :**

Si nécessaire, enregistrez la capture pour une analyse ultérieure. Allez dans "File" > "Save As" et choisissez le format de fichier.

## Remarques :

- Assurez-vous de comprendre et de respecter les lois et règlements locaux lors de la capture du trafic réseau.
- Wireshark offre de nombreuses fonctionnalités avancées pour une analyse approfondie. Consultez la documentation pour en savoir plus.

Wireshark est un outil puissant pour l'analyse du trafic IP, que ce soit pour le dépannage, la sécurité réseau, ou la compréhension approfondie du fonctionnement des protocoles sur un réseau.