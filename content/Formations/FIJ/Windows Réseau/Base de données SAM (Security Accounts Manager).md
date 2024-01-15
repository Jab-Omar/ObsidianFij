---
date: 2024-01-15
---
# Base de données SAM (Security Accounts Manager)

Dans le contexte des systèmes d'exploitation Windows, la base de données SAM (Security Accounts Manager) joue un rôle crucial dans la gestion des comptes d'utilisateurs et de groupes. Cependant, il est important de noter que l'utilisation de la base de données SAM varie entre les modèles de groupe de travail (Workgroup) et de domaine.

## Workgroup (Groupe de Travail)

Dans un modèle de groupe de travail, chaque ordinateur a sa propre base de données SAM locale. Cette base de données stocke les informations relatives aux comptes d'utilisateurs et aux groupes locaux sur cet ordinateur spécifique. Chaque machine gère ses propres comptes d'utilisateurs et leurs droits d'accès.

## Domaine

Dans un modèle de domaine, la base de données SAM locale est remplacée par l'Active Directory (AD). L'AD fonctionne comme une base de données centralisée et partagée qui stocke les informations de compte d'utilisateur, de groupe et d'autres objets du réseau. L'AD utilise le protocole LDAP (Lightweight Directory Access Protocol) pour permettre l'accès et la gestion des informations contenues dans la base de données.

## Rôle de la Base de Données SAM

1. **Stockage des Comptes d'Utilisateurs :** La base de données SAM conserve les informations telles que les noms d'utilisateur, les mots de passe (sous forme de hachage), les droits d'accès et d'autres paramètres liés aux comptes d'utilisateurs.
    
2. **Authentification :** La base de données SAM est utilisée lors du processus d'authentification, où les utilisateurs soumettent leurs identifiants (nom d'utilisateur et mot de passe) pour accéder à une machine ou à des ressources réseau.
    
3. **Politiques de Sécurité :** Elle stocke également des informations sur les politiques de sécurité locales, telles que les verrouillages de compte après un certain nombre de tentatives infructueuses de connexion.
    
4. **Groupes Locaux :** Dans le contexte d'un groupe de travail, la base de données SAM gère les groupes locaux qui définissent les autorisations sur une machine spécifique.
    

En résumé, la base de données SAM est fondamentale pour la gestion des comptes d'utilisateurs et de groupes, jouant un rôle central dans l'authentification et la gestion des autorisations, que ce soit au niveau local dans un groupe de travail ou de manière centralisée dans un domaine à travers l'Active Directory.