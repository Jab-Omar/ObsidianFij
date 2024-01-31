---
date: 31-01-2024
Time: 23:44
---
# Laboratoire de Détection des Conflits d'Adresses IP

## Objectif du Laboratoire
Ce laboratoire vise à comprendre et à tester la détection des conflits d'adresses IP sur un serveur DHCP. Nous allons intentionnellement configurer deux périphériques avec la même adresse IP pour déclencher un conflit, puis vérifier les journaux DHCP pour détecter et résoudre ce conflit.

## Prérequis
- Un serveur DHCP configuré et fonctionnel.
- Deux périphériques (ordinateurs, appareils mobiles, etc.) pouvant être configurés pour obtenir une adresse IP via DHCP.

## Étapes du Laboratoire

### Étape 1: Activation de la Détection des Conflits d'Adresses IP
1. Ouvrez le Gestionnaire DHCP sur le serveur.
2. Cliquez avec le bouton droit sur le nom du serveur dans l'arborescence et sélectionnez "Propriétés".
3. Allez dans l'onglet "Avancé" et cochez l'option "Activer la détection des conflits d'adresses IP".

### Étape 2: Configuration des Conflits d'Adresses IP
1. Configurez deux périphériques pour obtenir une adresse IP via DHCP.
2. Intentionnellement attribuez la même adresse IP à ces deux périphériques (par exemple, 192.168.1.100).

### Étape 3: Vérification des Conflits d'Adresses IP
1. Sur le serveur DHCP, ouvrez les journaux DHCP pour surveiller les événements.
   - Dans l'Observateur d'événements sous Windows Server, recherchez les événements de type "DHCP-Server".
   - Sur d'autres systèmes, consultez les journaux DHCP pour trouver des informations sur les conflits d'adresses IP.
2. Attendez quelques instants pour permettre au serveur DHCP de détecter le conflit.

### Étape 4: Résolution du Conflit
1. Une fois que le conflit est détecté, le serveur DHCP enregistre un événement dans les journaux.
2. Identifiez les adresses MAC des périphériques en conflit à partir des journaux DHCP.
3. Accédez aux périphériques en conflit et modifiez la configuration réseau pour résoudre le conflit en attribuant des adresses IP uniques.

## Points à Noter
- La détection des conflits d'adresses IP peut prendre quelques minutes, assurez-vous de vérifier régulièrement les journaux DHCP.
- Les actions à entreprendre pour résoudre un conflit d'adresses IP dépendent de la configuration réseau spécifique et des périphériques impliqués.

Ce laboratoire offre une expérience pratique pour comprendre la détection et la résolution des conflits d'adresses IP sur un serveur DHCP. La surveillance des journaux DHCP est un outil essentiel pour maintenir l'intégrité du réseau et garantir une attribution correcte des adresses IP aux périphériques.