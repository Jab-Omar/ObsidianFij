---
date: 2023-11-20
---
# Exercice : Configuration Initiale du Pare-feu Windows

## Objectif

L'objectif de cet exercice est de comprendre les bases de la configuration du Pare-feu Windows en créant une règle pour bloquer ou autoriser une application spécifique.

### Étape 1 : Accès aux Paramètres du Pare-feu Windows

1. Ouvrez le Panneau de configuration sur votre ordinateur.
2. Cherchez et sélectionnez "Système et sécurité" puis cliquez sur "Pare-feu Windows".

### Étape 2 : Création d'une Nouvelle Règle

1. Dans le Pare-feu Windows, sélectionnez "Paramètres avancés" sur la gauche.
2. Cliquez sur "Règles de trafic entrant" ou "Règles de trafic sortant" selon ce que vous souhaitez configurer.
3. Sur le côté droit, cliquez sur "Nouvelle règle" pour créer une nouvelle règle.

### Étape 3 : Configuration de la Règle

1. Choisissez le type de règle que vous souhaitez créer (par exemple, une règle pour un programme spécifique).
2. Sélectionnez "Programme" et cliquez sur "Suivant".
3. Parcourez votre système pour sélectionner l'application pour laquelle vous voulez créer la règle.
4. Choisissez "Bloquer la connexion" ou "Autoriser la connexion" selon ce que vous voulez faire avec cette application.
5. Donnez un nom à votre règle pour la reconnaître facilement.
6. Terminez en cliquant sur "Terminer".

### Étape 4 : Test de la Règle

1. Ouvrez l'application pour laquelle vous avez créé la règle.
2. Essayez d'accéder à internet ou à un service réseau.
3. Observez si la connexion est bloquée ou autorisée en fonction de la règle que vous avez créée.