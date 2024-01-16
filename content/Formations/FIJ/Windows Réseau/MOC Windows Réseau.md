---
date: 2024-01-09
---
# Cours Windows Réseau avec Active Directory

## Introduction à Windows Serveur
- [[Bases de Windows Serveur]]
## Configuration Réseau dans Oracle VirtualBox
- [[Configurations Réseau dans Oracle VirtualBox]]

## Windows Server : DNS
### Théorie
- Introduction sur le service DNS
- Les noms des domaines
	- hiérarchie des nom de domaine
	- Fully qualified domain name ou fqdn
### La résolution des noms
- Introduction au concept de la résolution des noms
- Les serveurs racines
- Les zones
- Le cache
- La redondance
### La résolution inverse
### Les enregistrement DNS
## Active Directory (AD)
### Théorie sur l'Active Directory
#### Un annuaire Active Directory, Pourquoi ?
- [[Active Directory (AD)]]
- [[Les intérêts d'un annuaire AD]]
- [[La structure de l'Active Directory]]
#### Contrôleur de domaine et domaine
- [[Workgroup vs domaine]]
	- [[Base de données SAM (Security Accounts Manager)]]
- [[Les contrôleurs de domaine]]
	- [[NTDS.dit]]
- [[La réplication des contrôleurs de domaine]]

#### Domaine, arbre et forêt
- [[Symbolisation d’un domaine]]
- [[Notion d'arbre]]
- Notion de forêt
- Le Niveau fonctionnel

#### Les protocoles LDAP,DNS, et Kerberos
- Le protocole LDAP dans AD
- Le proocole DNS dans AD
- Le protocole Kerberos

#### les principaux attributs d'objets dans l'active directory
- Les principales classes
- DistinguishedName et GUID
- Les attributs indispensables
#### Installation et Configuration

- [[Processus d'installation de l'Active Directory]]
- [[Configuration initiale d'un contrôleur de domaine]]

#### Gestion des Objets

- Utilisateurs
    - Création, modification, suppression
    - Attributs utilisateur
- Groupes
    - Types de groupes
    - Gestion des membres

#### Stratégies de Groupe (GPO)

- Définition des GPO
- Application des GPO
- Exemples d'utilisation

#### Authentification et Autorisation

- Protocoles d'authentification
- Contrôle d'accès basé sur les rôles (RBAC)

#### Réplication

- Réplication des données dans l'AD
- Sites et services

#### Sauvegarde et Restauration

- Stratégies de sauvegarde
- Processus de restauration

#### Dépannage

- Outils de dépannage
- Problèmes courants et solutions

#### Sécurité

- Sécurisation de l'Active Directory
- Bonnes pratiques de sécurité

#### Enrichissement des Concepts

- Le principe AAA
- Global catalogue
- Notion d'objet, classe, attribut
- On-premise
- Sysvol
- Ndts.dit
- Domain controller
- Workgroup vs Domain

#### Exercices et Labos

- Pratique des installations et configurations
- Création et gestion d'objets
- Mise en place de GPO
- Simulation de scénarios de dépannage

#### Questions Fréquentes en Entretien d'Embauche

- Réponses aux questions sur l'AD
- Scénarios pratiques d'utilisation
- Conseils pour se préparer aux entretiens

#### Ressources Supplémentaires

- Livres recommandés
- Sites web utiles
- Cours en ligne