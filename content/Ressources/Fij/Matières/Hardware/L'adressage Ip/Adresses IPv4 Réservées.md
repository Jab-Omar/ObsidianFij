---
tags:
  - Hardware
date: 2023-11-09
---
# Adresses IPv4 Réservées

Les adresses IPv4 réservées sont des plages d'adresses spécifiques qui sont réservées à des fins particulières, telles que les adresses de réseau local, les adresses de diffusion, etc. Voici quelques-unes des adresses IPv4 réservées couramment utilisées :

## 1. Adresse de réseau

L'adresse de réseau est l'adresse qui représente le réseau lui-même. Elle est utilisée pour identifier le réseau auquel un périphérique appartient. Par exemple, l'adresse `192.168.1.0` peut être utilisée pour représenter un réseau local.

## 2. Adresse de diffusion

L'adresse de diffusion est utilisée pour envoyer des données à tous les périphériques d'un réseau spécifique. Elle est généralement la dernière adresse disponible dans une plage. Par exemple, l'adresse `192.168.1.255` pourrait être une adresse de diffusion pour le réseau `192.168.1.0`.

## 3. APIPA (Automatic Private IP Addressing)

Les adresses APIPA sont utilisées lorsque la configuration DHCP échoue. Les systèmes d'exploitation utilisent une plage spécifique pour attribuer automatiquement une adresse IP lorsque la configuration via DHCP n'est pas possible. Cette plage est généralement entre `169.254.0.1` et `169.254.255.254`.

## 4. Adresse Loopback

L'adresse loopback (`127.0.0.1`) est utilisée pour tester la pile TCP/IP d'un périphérique. Elle permet à un périphérique de s'auto-envoyer des données sans passer par le réseau.

## 5. Adresse de test de documentation

L'adresse `192.0.2.0` est réservée à des fins de documentation et de test. Elle ne devrait pas être utilisée dans un environnement de production.

Ces adresses réservées sont essentielles pour le bon fonctionnement des réseaux et des périphériques, en assurant des communications efficaces et sûres.