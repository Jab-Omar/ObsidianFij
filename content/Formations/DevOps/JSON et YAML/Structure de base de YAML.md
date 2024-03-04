---
date: 01-03-2024
Time: 13:57
---
# Structure de base de YAML

La structure de base de YAML repose sur des concepts simples et intuitifs pour représenter les données de manière lisible et organisée. Voici un aperçu des principaux éléments de la structure de base de YAML :

## 1. Syntaxe basée sur l'indentation et les espaces blancs

Dans YAML, l'indentation et les espaces blancs sont utilisés pour définir la structure hiérarchique des données. Les éléments de données de niveau supérieur sont définis à la racine du document, tandis que les éléments de données imbriqués sont indentés avec des espaces pour indiquer leur relation hiérarchique.

Exemple :

```yaml
livre:
  titre: "Le Seigneur des Anneaux"
  auteur: "J.R.R. Tolkien"
  chapitres:
    - Chapitre 1
    - Chapitre 2
```

Dans cet exemple, les éléments `titre`, `auteur` et `chapitres` sont des sous-éléments du `livre`, et leur indentation montre leur relation hiérarchique.

## 2. Utilisation des délimiteurs de données

Les données peuvent être délimitées par des signes spécifiques pour indiquer leur type. Par exemple, les chaînes de caractères peuvent être délimitées par des guillemets (`"`), les tableaux peuvent être délimités par des crochets (`[]`), et les objets peuvent être délimités par des accolades (`{}`).

Exemple :

```yaml
titre: "Le Seigneur des Anneaux"
chapitres:
  - Chapitre 1
  - Chapitre 2
```

Dans cet exemple, `"Le Seigneur des Anneaux"` est une chaîne de caractères délimitée par des guillemets, et `[Chapitre 1, Chapitre 2]` est un tableau délimité par des crochets.

## 3. Commentaires

YAML prend en charge les commentaires, qui peuvent être ajoutés en utilisant le symbole `#`. Les commentaires sont ignorés lors de la lecture des données YAML et sont utilisés pour fournir des explications ou des notes dans le document.

Exemple :

```yaml
# Informations sur le livre
titre: "Le Seigneur des Anneaux"  # Titre du livre
auteur: "J.R.R. Tolkien"  # Auteur du livre
```

Dans cet exemple, les commentaires ont été ajoutés pour expliquer le contenu des données YAML.

La structure de base de YAML est simple mais puissante, offrant une manière flexible et lisible pour représenter une grande variété de données dans différents contextes.