---
date: 01-03-2024
Time: 14:07
---

# Gestion des données non scalaires en YAML

En plus des types de données scalaires tels que les chaînes de caractères, les nombres et les booléens, YAML prend également en charge les données non scalaires, telles que les listes, les objets et les données complexes. Voici comment gérer ces types de données non scalaires en YAML :

## 1. Collections ordonnées (Listes)

Les collections ordonnées sont représentées sous forme de listes en YAML. Les listes sont délimitées par des tirets (-) et peuvent contenir une séquence d'éléments de données.

Exemple :

```yaml
tâches:
  - Acheter du lait
  - Aller à la poste
  - Faire les courses
```

Dans cet exemple, `tâches` est une liste contenant trois éléments de données.

## 2. Collections non ordonnées (Objets)

Les collections non ordonnées sont représentées sous forme d'objets en YAML. Les objets sont délimités par des accolades ({ }) et contiennent des paires clé-valeur.

Exemple :

```yaml
personne:
  nom: "Jean Dupont"
  age: 30
  ville: "Paris"
```

Dans cet exemple, `personne` est un objet contenant des informations sur une personne, telles que le nom, l'âge et la ville.

## 3. Données complexes

YAML permet également de représenter des données complexes en combinant des listes et des objets. Par exemple, vous pouvez avoir une liste d'objets ou un objet contenant une liste.

Exemple :

```yaml
personnes:
  - nom: "Jean Dupont"
    age: 30
    ville: "Paris"
  - nom: "Alice Smith"
    age: 25
    ville: "New York"
```

Dans cet exemple, `personnes` est une liste d'objets, chaque objet représentant une personne avec un nom, un âge et une ville.

En utilisant ces techniques, YAML offre une manière flexible et lisible de représenter une variété de données, y compris les données non scalaires telles que les listes et les objets.
