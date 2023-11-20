---
date: 2023-11-09
---

# CIDR (Classless Inter-Domain Routing) : Optimiser la Gestion des Adresses IP

Le CIDR, ou Classless Inter-Domain Routing, représente un système de notation d'adresses IP plus souple et efficace, introduit pour résoudre les limitations du système de classes d'adresses IP et optimiser l'utilisation des ressources d'adressage sur Internet.

## Notation CIDR et Masque de Sous-Réseau

La notation CIDR combine une adresse IP avec une indication de la longueur du préfixe, également appelée masque de sous-réseau. Le masque de sous-réseau est représenté par le nombre de bits alloués pour identifier le réseau dans une adresse IP. Par exemple, dans l'adresse **192.168.1.1/24**, le "/24" signifie que les 24 premiers bits sont réservés pour identifier le réseau, laissant 8 bits pour les hôtes.

## Objectif du CIDR

Le CIDR a été développé pour surmonter les limitations du système de classes (A, B, C) qui allouait des blocs d'adresses de taille fixe, conduisant souvent à un gaspillage d'adresses IP. Avec le CIDR, la taille des blocs d'adresses peut varier, permettant une allocation plus précise en fonction des besoins spécifiques des réseaux.

## Avantages du CIDR

### 1. **Optimisation de l'Espace d'Adressage :** 
CIDR permet une utilisation plus efficace des adresses IP en évitant les restrictions de taille fixe imposées par le système de classes. Cela permet une allocation plus précise des adresses, réduisant le gaspillage.

### 2. **Réduction de la Table de Routage :**
Le remplacement du système basé sur les classes par CIDR a conduit à une réduction significative de la taille des tables de routage sur les équipements réseau. Les routes sont plus spécifiques, ce qui améliore l'efficacité du routage sur Internet.

### 3. **Flexibilité dans l'Allocation d'Adresses :**
CIDR offre une flexibilité considérable dans l'allocation des adresses. Les blocs peuvent être ajustés en fonction des besoins spécifiques du réseau, évitant ainsi la surallocation ou la sous-allocation d'adresses IP.

## Exemple Pratique

Considérons une plage d'adresses IP **192.168.1.0 - 192.168.1.255**. Plutôt que de spécifier cela comme une classe C avec un masque de sous-réseau de 255.255.255.0, avec CIDR, vous pourriez le représenter comme **192.168.1.0/24**.

## Conclusion

Le CIDR, avec sa notation flexible et l'utilisation de masques de sous-réseau, offre une approche puissante pour gérer les adresses IP de manière plus efficace et scalable. Cette compréhension approfondie du CIDR est cruciale pour les professionnels travaillant avec les réseaux et les adresses IP, car il contribue à une utilisation plus judicieuse des ressources d'adressage IP sur Internet.