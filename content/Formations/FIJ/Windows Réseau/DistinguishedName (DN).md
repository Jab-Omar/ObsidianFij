---
date: 2024-01-17
---
---
# DistinguishedName (DN) dans Active Directory

Le DistinguishedName (DN) est un élément fondamental de l'annuaire Active Directory (AD), utilisé pour identifier de manière unique la position d'un objet au sein de la structure hiérarchique de l'annuaire. Le DN offre une référence complète et ordonnée, décrivant le chemin depuis la racine de l'annuaire jusqu'à l'objet spécifique. Voici une exploration plus approfondie des composants et de l'importance du DistinguishedName :

1. **Composants du DN :**
   - Le DN est composé de paires attribut-valeur, séparées par des virgules. Les attributs couramment utilisés incluent :
     - `CN` (Common Name) : Représente le nom commun de l'objet, tel que le nom d'utilisateur pour un utilisateur.
     - `OU` (Organizational Unit) : Indique une unité organisationnelle, permettant une organisation logique des objets.
     - `DC` (Domain Component) : Identifie un composant de domaine, spécifiant le nom de domaine dans le chemin.

2. **Exemple de DN :**
   - Un exemple typique de DN pourrait être :
     ```
     CN=John Doe,OU=Ventes,DC=entreprise,DC=com
     ```
     Dans cet exemple, l'objet (probablement un utilisateur) nommé "John Doe" est situé dans l'unité organisationnelle "Ventes" du domaine "entreprise.com".

3. **Hiérarchie et Organisation :**
   - Le DN suit la structure hiérarchique de l'arborescence AD. Chaque composant du DN indique un niveau de la hiérarchie, fournissant une organisation logique et ordonnée des objets au sein de l'annuaire.

4. **Unicité et Identification :**
   - Chaque objet dans Active Directory a un DN unique. Même si deux objets partagent le même nom commun, leur emplacement dans la hiérarchie, défini par le DN, garantit leur unicité.

5. **Stabilité et Déplacement :**
   - Le DN reste constant tout au long de la vie d'un objet, sauf en cas de déplacement. Lorsqu'un objet est déplacé vers un autre conteneur, son DN est mis à jour pour refléter son nouvel emplacement.

6. **Référence et Utilisation :**
   - Le DN est couramment utilisé pour référencer des objets lors de la recherche, de la modification ou de la suppression. Il offre une méthode précise et structurée pour localiser des entités au sein de l'annuaire.

En conclusion, le DistinguishedName est un identifiant essentiel dans Active Directory, offrant une référence unique et hiérarchique pour chaque objet. Sa structure bien définie facilite la gestion, la localisation et la compréhension des emplacements des objets au sein de l'environnement AD.