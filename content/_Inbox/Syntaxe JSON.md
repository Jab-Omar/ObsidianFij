---
date: 25-02-2024
Time: 14:23
---
# Syntaxe JSON

Le JSON (JavaScript Object Notation) utilise une syntaxe simple pour représenter des données structurées. Voici les principaux éléments de sa syntaxe :

## Objets JSON

Un objet JSON est une collection non ordonnée de paires clé-valeur. Il est délimité par des accolades `{}`. Chaque paire clé-valeur est séparée par une virgule `,`.

Exemple d'objet JSON :

```json
{
  "nom": "Jean",
  "age": 30,
  "ville": "Paris",
  "estEtudiant": false
}
```

## Clés et valeurs

- **Clés** : Les noms de clés sont des chaînes de caractères placées entre guillemets doubles.
- **Valeurs** : Les valeurs peuvent être de différents types : chaînes de caractères, nombres, booléens, tableaux, objets JSON, ou null.

## Tableaux JSON

Un tableau JSON est une collection ordonnée de valeurs. Il est délimité par des crochets `[]`. Les valeurs sont séparées par des virgules `,`.

Exemple de tableau JSON :

```json
["Marc", "Sophie", "Pierre"]
```

## Exemple de Syntaxe JSON complète

```json
{
  "personne": {
    "nom": "Jean",
    "age": 30,
    "ville": "Paris",
    "estEtudiant": false
  },
  "amis": ["Marc", "Sophie", "Pierre"]
}
```

Dans cet exemple, "personne" est un objet JSON contenant les informations sur une personne, tandis que "amis" est un tableau JSON contenant une liste d'amis.

En résumé, la syntaxe JSON est simple et intuitive, ce qui en fait un format de données populaire pour l'échange d'informations sur le web.
