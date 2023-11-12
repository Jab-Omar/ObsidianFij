---
tags: 
date: 2023-11-12
---
# FTPS (File Transfer Protocol Secure)

Le **FTPS (File Transfer Protocol Secure)** est une extension sécurisée du protocole FTP utilisé pour le transfert sécurisé de fichiers. Il utilise un chiffrement SSL/TLS pour assurer la confidentialité des données pendant la transmission. Explorons plus en détail son fonctionnement :

## Fonctionnement

1. **Mode implicite et explicite:** FTPS peut fonctionner en mode implicite (connexion sécurisée dès le début) ou en mode explicite (la sécurisation de la connexion est négociée par un mécanisme de commande spécifique).
    
2. **Ports:** En mode implicite, le port 990 est généralement utilisé pour la connexion sécurisée. En mode explicite, la négociation SSL/TLS se fait sur le port de commande FTP régulier (généralement 21).
    
3. **Chiffrement SSL/TLS:** Une fois la connexion établie, le chiffrement SSL/TLS est initié, sécurisant ainsi toutes les données échangées entre le client et le serveur FTPS.
    

## Avantages

1. **Confidentialité des données:** Le chiffrement SSL/TLS garantit que les fichiers transférés entre le client et le serveur sont sécurisés contre les interceptions non autorisées.
    
2. **Authentification sécurisée:** FTPS utilise des certificats SSL/TLS pour authentifier le serveur, renforçant la sécurité et garantissant que le client communique avec le serveur légitime.
    

## Tâches courantes pour les techniciens informatiques

1. **Configuration du serveur FTPS:** Installation et configuration d'un serveur FTPS, y compris la gestion des certificats SSL/TLS et la définition des politiques de sécurité.
    
2. **Gestion des certificats SSL/TLS:** Veiller à ce que les certificats soient correctement installés, valides et mis à jour pour assurer une connexion sécurisée.
    
3. **Dépannage des problèmes de transfert:** En cas de problème, les techniciens doivent diagnostiquer les problèmes potentiels liés au chiffrement, aux certificats ou à d'autres aspects du transfert FTPS.
    

## Importance pour les techniciens informatiques

La maîtrise du FTPS est cruciale pour les techniciens informatiques, car il offre une méthode sécurisée pour le transfert de fichiers. La configuration, la gestion des certificats et le dépannage sont des compétences essentielles pour assurer un transfert de fichiers sécurisé.