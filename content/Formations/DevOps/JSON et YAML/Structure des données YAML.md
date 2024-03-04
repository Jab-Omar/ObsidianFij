---
date: 01-03-2024
Time: 14:06
---
# Structure des données YAML

La structure des données YAML est définie par l'organisation hiérarchique des éléments de données à l'intérieur d'un document YAML. Voici les principaux aspects de la structure des données YAML :

## 1. Structure hiérarchique

YAML permet de représenter les données de manière hiérarchique en utilisant l'indentation pour indiquer la relation entre les différents éléments. Les éléments de données imbriqués sont indentés sous leurs éléments parents pour représenter leur relation hiérarchique.

Exemple :

```yaml
livre:
  titre: "Le Seigneur des Anneaux"
  auteur: "J.R.R. Tolkien"
  chapitres:
    - Chapitre 1
    - Chapitre 2
```

Dans cet exemple, les éléments `titre`, `auteur` et `chapitres` sont des sous-éléments du `livre`, et leur indentation indique leur relation hiérarchique.

## 2. Clés et valeurs

Les données YAML sont généralement représentées sous forme de paires clé-valeur, où chaque clé est suivie d'une valeur. Les clés doivent être uniques à l'intérieur d'un même niveau d'indentation et peuvent être suivies de différents types de valeurs, y compris des chaînes de caractères, des nombres, des tableaux ou des objets.

Exemple :

```yaml
livre:
  titre: "Le Seigneur des Anneaux"
  auteur: "J.R.R. Tolkien"
  chapitres:
    - Chapitre 1
    - Chapitre 2
```

Dans cet exemple, `titre`, `auteur` et `chapitres` sont des clés, et leurs valeurs sont respectivement des chaînes de caractères et un tableau.

## 3. Collection ordonnée (Liste)

YAML permet de représenter des collections ordonnées d'éléments à l'aide de listes. Les listes sont délimitées par des tirets (-) et peuvent contenir une séquence d'éléments de données.

Exemple :

```yaml
nombres:
  - 1
  - 2
  - 3
```

Dans cet exemple, `nombres` est une liste contenant les nombres 1, 2 et 3.

## 4. Collection non ordonnée (Dictionnaire)

Les collections non ordonnées d'éléments sont représentées sous forme de dictionnaires en YAML. Les dictionnaires sont délimités par des accolades ({ }) et contiennent des paires clé-valeur.

Exemple :

```yaml
personne:
  nom: "Jean Dupont"
  age: 30
  ville: "Paris"
```

Dans cet exemple, `personne` est un dictionnaire contenant des informations sur une personne, telles que le nom, l'âge et la ville.

En utilisant ces principes de structure, YAML offre une manière flexible et lisible de représenter une variété de données de manière organisée et structurée.
