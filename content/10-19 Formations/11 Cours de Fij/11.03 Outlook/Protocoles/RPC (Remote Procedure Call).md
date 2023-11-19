---
tags: 
date: 2023-11-12
---
# RPC (Remote Procedure Call)

Le **RPC (Remote Procedure Call)** permet à un programme sur un ordinateur de faire appel à une procédure sur un autre ordinateur comme s'il s'agissait d'une procédure locale. Voici une explication simplifiée :

## Fonctionnement

1. **Appel distant :** Un programme sur un ordinateur (client) peut invoquer une fonction sur un autre ordinateur distant (serveur) comme si elle était locale.
    
2. **Encapsulation des données :** Les paramètres de la fonction et les résultats sont encapsulés pour être transmis sur le réseau.
    
3. **Transmission des données :** Les données encapsulées sont envoyées au serveur, où la fonction est exécutée, et les résultats sont renvoyés au client.
    

## Avantages

1. **Abstraction réseau :** Permet aux programmes de s'appeler à distance sans se soucier des détails de la communication réseau.
    
2. **Réutilisation du code :** Facilite la réutilisation des fonctions dans des environnements distribués.
    

## Exemple simple

Supposons que vous avez un programme sur votre ordinateur local qui a besoin d'exécuter une fonction sur un serveur distant. Avec le RPC, vous pouvez invoquer cette fonction comme si elle était directement disponible sur votre ordinateur.

## Importance pour les techniciens informatiques

- **Intégration d'applications :** Utilisé pour permettre la communication entre différentes parties d'une application, même si elles s'exécutent sur des ordinateurs différents.
    
- **Optimisation des performances :** Bien configuré, le RPC peut contribuer à l'optimisation des performances dans des environnements distribués.