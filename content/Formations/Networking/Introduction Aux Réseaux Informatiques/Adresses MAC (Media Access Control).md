---
date: 19-02-2024
Time: 21:11
---
# Adresses MAC (Media Access Control)

L'adresse MAC, ou adresse de contrôle d'accès au support, est un identifiant unique attribué à chaque interface réseau pour les dispositifs de communication. Elle opère au niveau de la couche 2 du modèle OSI et est utilisée pour identifier de manière unique les périphériques dans un réseau local.

## Format de l'Adresse MAC

Une adresse MAC est une séquence de 6 octets, souvent représentée sous la forme de 12 caractères hexadécimaux, séparés par des deux-points (par exemple, 00:1A:2B:3C:4D:5E). Les trois premiers octets représentent généralement le fabricant du périphérique (OUI - Organizational Unique Identifier), tandis que les trois derniers octets sont attribués de manière unique à chaque interface spécifique.

## Utilité de l'Adresse MAC

1. **Communication sur le Réseau Local :** L'adresse MAC est essentielle pour diriger les trames de données vers le bon périphérique au sein d'un réseau local. Les commutateurs réseau utilisent ces adresses pour acheminer efficacement le trafic.

2. **Contrôle d'Accès au Réseau :** Dans certains cas, les adresses MAC sont utilisées pour restreindre l'accès au réseau en autorisant uniquement les dispositifs ayant des adresses MAC spécifiques.

3. **Résolution d'Adresse IP :** Lors de la communication sur un réseau, le protocole ARP utilise l'adresse MAC pour faire correspondre une adresse IP à une adresse physique.

## Note sur la Confidentialité

Bien que les adresses MAC soient cruciales pour le fonctionnement des réseaux locaux, elles peuvent potentiellement être exploitées à des fins de suivi. Certaines technologies, comme le changement d'adresse MAC aléatoire, ont été développées pour atténuer ces problèmes de confidentialité.
