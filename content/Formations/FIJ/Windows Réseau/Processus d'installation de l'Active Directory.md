---
date: 2024-01-14
---
# Processus d'Installation de l'Active Directory

L'installation de l'Active Directory sur un serveur Windows est une étape cruciale pour la gestion centralisée des utilisateurs, des groupes et des ressources réseau. Suivez ces étapes pour configurer l'Active Directory :

## 1. Configuration Préalable

### Paramètres IP
- **Adresse IP Statique :** Donnez à votre serveur une adresse IP fixe. Cela évite les changements d'adresse qui pourraient perturber la communication.
- **Serveur DNS :** Configurez le serveur pour utiliser sa propre adresse IP comme serveur DNS principal. Cela aide à résoudre les noms au sein du réseau.
### Nom du Serveur
- **Nom Significatif :** Choisissez un nom de serveur clair et unique dans le réseau, sans caractères spéciaux.
### Configurations DNS
- **Enregistrement DNS A :** Associez le nom du serveur à son adresse IP dans la configuration DNS.
- **Enregistrement PTR :** Configurez l'enregistrement Pointer pour résoudre l'adresse IP en un nom de domaine.
- **Réplication DNS :** Assurez-vous que tous les serveurs DNS se répliquent correctement pour maintenir des informations cohérentes.

## 2. Accéder au Gestionnaire de Serveur

Ouvrez le Gestionnaire de Serveur à partir du menu Démarrer. Cela peut être fait en sélectionnant "Gérer" dans le menu contextuel du bouton droit sur l'icône "Ce PC".

## 3. Ajout de rôles et de fonctionnalités

- Cliquez sur "Ajouter des rôles et des fonctionnalités".
- Suivez l'assistant d'installation en sélectionnant "Installation basée sur un rôle ou une fonctionnalité".
- Choisissez le serveur où vous souhaitez installer l'Active Directory.

## 4. Sélection du rôle

- Choisissez "Services de domaine Active Directory".
- L'assistant vous informera des fonctionnalités supplémentaires nécessaires. Cliquez sur "Ajouter des fonctionnalités".

## 5. Configuration de l'Active Directory

- Une fois les fonctionnalités ajoutées, accédez à "Gérer" dans le Gestionnaire de Serveur.
- Cliquez sur "Promouvoir ce serveur en contrôleur de domaine".
- Sélectionnez "Ajouter une nouvelle forêt" si c'est la première installation, sinon, ajoutez le serveur à une [[Arbres et Forêts#Forêts dans Active Directory|forêt]] existante.

## 6. Configuration des options

- Définissez un nom de domaine pour votre forêt.
- Choisissez le niveau fonctionnel de la forêt et du domaine en fonction de vos besoins.
- Configurez le mot de passe du mode de restauration du service d'annuaire.

## 7. Installation

- L'assistant vous permet de vérifier vos choix. Cliquez sur "Suivant" et attendez la vérification des prérequis.
- Si tout est correct, cliquez sur "Installer" pour démarrer le processus d'installation.

## 8. Redémarrage

Une fois l'installation terminée, le serveur redémarrera automatiquement. Connectez-vous avec les privilèges d'administrateur du domaine.

Félicitations, vous avez maintenant configuré l'Active Directory sur votre serveur Windows !