---
date: 2024-01-15
---
#   Notion d'Arbre dans Active Directory

Lorsqu'on aborde la notion d'arbre dans le contexte d'Active Directory, on se réfère à une structure hiérarchique de domaines. Voici quelques points clés pour comprendre cette notion :

- **Domaine Racine :** L'arbre commence par un domaine racine, qui est le premier domaine créé dans la forêt Active Directory. Il sert de point de départ pour la hiérarchie.
    
- **Domaines Enfants :** Les domaines peuvent être ajoutés à la forêt en tant que sous-domaines du domaine racine. Chaque domaine enfant est autonome dans sa gestion tout en héritant des caractéristiques du domaine parent.
    
- **Relation Parent-Enfant :** Chaque domaine enfant est lié à son domaine parent par une relation parent-enfant. Cette relation permet une gestion centralisée tout en offrant une autonomie relative à chaque domaine enfant.
    
- **Partage d'Espace de Nom DNS :** Les domaines dans un arbre partagent un espace de noms DNS. Les noms de domaine complets (FQDN) des domaines enfants sont des extensions du FQDN du domaine parent.
    
- **Confiance d'Arbre :** Les domaines au sein d'un arbre ont une confiance mutuelle implicite. Cela facilite l'accès aux ressources entre les domaines sans nécessiter de configurations de confiance supplémentaires.
    
- **Réplication :** Les données Active Directory, telles que les comptes d'utilisateurs et les politiques, sont répliquées entre les domaines de l'arbre pour maintenir la cohérence.
    
- **Extension Potentielle :** L'ajout de nouveaux domaines enfants offre une extension potentielle de la forêt. Chaque domaine enfant peut, à son tour, avoir ses propres sous-domaines, créant ainsi une structure arborescente étendue.