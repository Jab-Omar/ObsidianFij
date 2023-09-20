---
tags:
  - Windows
  - fij
---

## Introduction 
Une adresse MAC, abréviation de Media Access Control address, est un identifiant unique attribué à un contrôleur d'interface réseau (NIC) ou à un adaptateur réseau. Elle joue un rôle essentiel dans la mise en réseau, en aidant les périphériques d'un réseau à s'identifier et à communiquer entre eux. 
## Caractéristiques principales 

- Unicité:** Chaque appareil du réseau, qu'il s'agisse d'un ordinateur, d'un smartphone ou d'une imprimante en réseau, possède une adresse MAC unique au niveau mondial. 
- L'adresse MAC est une adresse matérielle intégrée par le fabricant dans le matériel de l'adaptateur réseau. 
- Format hexadécimal:** Les adresses MAC sont généralement exprimées sous la forme d'une série de six paires de chiffres hexadécimaux séparés par des deux points ou des traits d'union (par exemple, 00:1A:2B:3C:4D:5E). - 
- **Deux parties:** Une adresse MAC se compose de deux parties : l'OUI (Organizationally Unique Identifier) et la partie spécifique au NIC. 
## Fonctions 
L'adresse MAC remplit plusieurs fonctions importantes dans la mise en réseau : 

1. **Identification du périphérique:** Elle identifie de manière unique chaque périphérique réseau sur un segment de réseau local, ce qui permet aux périphériques de se reconnaître les uns les autres. 
2. **Les routeurs et les commutateurs utilisent les adresses MAC pour déterminer comment transmettre les paquets de données au sein d'un réseau local. 
3. **Protocole de résolution d'adresses (ARP):** Les adresses MAC sont utilisées dans le protocole ARP pour faire correspondre les adresses IP aux adresses MAC physiques. 
4. **Le filtrage MAC peut être utilisé pour contrôler l'accès à un réseau en autorisant ou en refusant des adresses MAC spécifiques. 
## Localisation de l'adresse MAC 
Pour trouver l'adresse MAC de votre appareil : 

- **Windows:** Ouvrez l'Invite de commande, tapez `ipconfig /all`, et recherchez "Physical Address" sous les informations de votre adaptateur réseau. 
- **MacOS:** Allez dans "Préférences système" > "Réseau", sélectionnez votre connexion réseau et cliquez sur "Avancé". L'adresse MAC est répertoriée dans l'onglet "Matériel". 
- Linux:** Utilisez la commande `ifconfig` ou `ip addr` pour afficher les informations relatives à l'interface réseau, y compris l'adresse MAC. 
- Smartphones:** Dans les paramètres réseau de l'appareil, vous trouverez généralement l'adresse MAC sous la forme "Wi-Fi MAC address" ou similaire. 
## Conclusion 
L'adresse MAC est un élément essentiel de la communication réseau, car elle garantit que les paquets de données sont correctement acheminés vers la destination prévue sur un réseau local. La compréhension des adresses MAC est essentielle pour les administrateurs de réseau et les utilisateurs afin de gérer et de dépanner la connectivité du réseau.