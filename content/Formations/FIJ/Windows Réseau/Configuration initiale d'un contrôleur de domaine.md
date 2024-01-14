---
date: 2024-01-14
---
# Configuration Initiale d'un Contrôleur de Domaine dans Active Directory

## 1. Prérequis

Avant de commencer la configuration initiale, assurez-vous de :

- **Choisir le Nom du Serveur :** Sélectionnez un nom de serveur significatif, conforme aux meilleures pratiques, et vérifiez la résolution DNS pour ce nom.
    
- **Attribuer une Adresse IP Statique :** Afin de maintenir une stabilité d'adresse, configurez une adresse IP statique pour le serveur.
    

## 2. Installation des Rôles et Fonctionnalités

- **Ouverture du Gestionnaire de Serveur :** Depuis le menu Démarrer, ouvrez le Gestionnaire de Serveur.
    
- **Ajout du Rôle AD DS :** Sélectionnez "Ajouter des rôles et fonctionnalités", puis choisissez le rôle "Services de domaine Active Directory".
    
- **Options Supplémentaires :** Sélectionnez les fonctionnalités nécessaires et suivez l'assistant pour compléter l'installation.
    

## 3. Promotion en Contrôleur de Domaine

- **Accès à "Gérer" :** Depuis le Gestionnaire de Serveur, cliquez sur "Gérer" puis sur "Ajouter des rôles et fonctionnalités".
    
- **Choix de la Fonction AD DS :** Sélectionnez "Promouvoir ce serveur en contrôleur de domaine".
    
- **Type d'Installation :** Choisissez l'option appropriée pour votre scénario, qu'il s'agisse d'un nouveau domaine, d'une nouvelle forêt ou de l'ajout à une forêt existante.
    
- **Options de Forêt :** Configurez le nom de la forêt, le niveau fonctionnel de la forêt et du domaine, et le mot de passe du mode de restauration du service d'annuaire.
    

## 4. Configuration des Options Additionnelles

- **Emplacement des Données d'Annuaire :** Définissez les chemins d'accès pour les fichiers de base de données, le journal de transactions et la sauvegarde.
    
- **Mot de Passe DSRM :** Configurez le mot de passe pour le mode de restauration du service d'annuaire (DSRM).
    
- **Vérification des Paramètres :** Revérifiez toutes les configurations avant de cliquer sur "Installer" pour garantir l'exactitude des paramètres.
    

## 5. Redémarrage

Une fois l'installation terminée, le serveur sera automatiquement redémarré. Connectez-vous ensuite avec des privilèges d'administrateur de domaine.

## Conseils Pratiques

- **Surveillance :** Surveillez les journaux d'événements pour détecter des erreurs éventuelles.
    
- **Sauvegarde :** Effectuez une sauvegarde de la base de données d'annuaire régulièrement.
    
- **Planification de la Réplication :** Assurez-vous que la réplication avec d'autres Contrôleurs de Domaine fonctionne correctement.
    

En résumé, la configuration initiale d'un Contrôleur de Domaine dans Active Directory nécessite des étapes soigneusement planifiées, de la préparation des prérequis à la promotion en tant que Contrôleur de Domaine, en passant par la configuration des options spécifiques. La surveillance continue et les bonnes pratiques de gestion sont cruciales pour maintenir la stabilité et la fiabilité de l'environnement AD.