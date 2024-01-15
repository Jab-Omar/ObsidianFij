---
date: 2024-01-15
---
## Classes et Attributs

### Classes
L'Active Directory utilise un modèle objet pour représenter les différents types d'objets stockés dans l'annuaire. Ces types d'objets sont définis par des classes. Les classes déterminent les propriétés qu'un objet peut avoir et les actions qu'il peut effectuer. Par exemple, une classe "utilisateur" peut avoir des attributs tels que "nom", "prénom" et "mot de passe".
### Attributs
Les attributs sont les propriétés spécifiques à une classe. Ils définissent les caractéristiques et les informations associées à un objet. Dans l'exemple de la classe "utilisateur", les attributs peuvent inclure des détails comme l'adresse e-mail, le numéro de téléphone, etc.
## Schéma
Le schéma de l'Active Directory définit la structure des classes et des attributs utilisés dans l'annuaire. Il s'agit d'un ensemble de règles qui déterminent la façon dont les objets peuvent être créés et les informations qu'ils peuvent stocker. Le schéma est crucial pour assurer la cohérence et la compatibilité des données dans l'ensemble de l'environnement AD.
## Partitions d'Annuaire
L'annuaire Active Directory est divisé en partitions, chacune stockant des informations spécifiques. Les trois principales partitions sont :
- **Configuration :** Contient des informations sur la configuration globale de l'AD, y compris la topologie du réseau et les paramètres de fonctionnement.
- **Schéma :** Stocke la définition du schéma AD, indiquant les classes et les attributs disponibles dans l'annuaire.
- **Domaine :** Représente la partition spécifique à un domaine et contient des informations sur les objets tels que les utilisateurs, les groupes, les ordinateurs, etc.