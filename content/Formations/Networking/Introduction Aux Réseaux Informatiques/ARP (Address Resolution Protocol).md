---
date: 19-02-2024
Time: 21:09
---

# ARP (Address Resolution Protocol)

L'ARP (Address Resolution Protocol) est un protocole de la couche 2 du modèle OSI utilisé dans les réseaux locaux. Son principal objectif est de faire correspondre une adresse IP à une adresse MAC. Lorsqu'un périphérique souhaite communiquer avec un autre sur le même réseau, il utilise l'adresse IP du destinataire pour demander à l'ARP de fournir l'adresse MAC correspondante.

## Fonctionnement de l'ARP

Lorsqu'un périphérique souhaite connaître l'adresse MAC associée à une adresse IP spécifique, il envoie une requête ARP broadcast (diffusée) sur le réseau local. Le périphérique cible répond avec son adresse MAC, et cette information est ensuite stockée dans la table ARP du périphérique émetteur.

## Commande ARP -a

Sur les systèmes d'exploitation Windows, la commande ARP -a est utilisée pour afficher la table ARP. Cette table contient les informations de correspondance entre les adresses IP et les adresses MAC des périphériques avec lesquels l'ordinateur a récemment communiqué.

### Utilisation de la commande ARP -a

Pour afficher la table ARP dans l'invite de commandes (cmd) :

```shell
arp -a
```

Cela affichera une liste des entrées ARP, indiquant l'adresse IP, l'adresse physique (adresse MAC) et le type d'interface associés à chaque périphérique.
