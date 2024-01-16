---
date: 2024-01-16
---
# Notion de Forêt dans Active Directory
La notion de forêt dans Active Directory (AD) représente une collection de domaines interconnectés au sein d'une structure arborescente. Voici quelques éléments clés pour comprendre cette notion :

- **Définition :** Une forêt Active Directory est une collection de domaines qui partagent une relation de confiance bidirectionnelle et partagent un catalogue global. Elle est la plus haute unité de regroupement dans la structure d'AD.
    
- **Domaine Racine :** Chaque forêt commence par un domaine racine, qui est le premier domaine créé lors de la mise en place de l'AD. Ce domaine racine définit le nom de la forêt.
    
- **Relations de Confiance :** Tous les domaines au sein d'une forêt ont une relation de confiance mutuelle implicite. Cela signifie que les utilisateurs et les ressources dans un domaine peuvent accéder aux ressources dans tous les autres domaines de la forêt sans nécessiter de configuration de confiance supplémentaire.
    
- **Partage du Catalogue Global :** Les forêts partagent un catalogue global, également appelé catalogue global de forêt, qui contient des informations sur tous les objets de la forêt. Cela facilite les recherches et les accès transforestiers.
    
- **Isolation des Schémas :** Chaque forêt a son propre schéma Active Directory, qui définit la structure et les types d'objets qui peuvent être stockés dans la forêt.
    
- **Séparation des Noms de Domaine :** Chaque forêt a son propre espace de noms DNS, garantissant l'unicité des noms de domaine complets (FQDN) au niveau de la forêt.
    
- **Indépendance des Politiques et des Comptes :** Chaque domaine au sein d'une forêt peut avoir ses propres politiques de groupe, comptes d'utilisateurs et autres paramètres, offrant une certaine autonomie administrative.
    
- **Extension Potentielle :** La mise en place d'une forêt permet d'ajouter de nouveaux domaines de manière indépendante, offrant ainsi une extensibilité pour répondre aux besoins évolutifs de l'organisation.
    

La notion de forêt dans Active Directory offre une structure organisationnelle puissante, permettant la gestion centralisée tout en préservant une certaine autonomie au niveau des domaines. Elle est particulièrement adaptée aux organisations complexes nécessitant une segmentation logique et une gestion modulaire de leurs ressources informatiques.