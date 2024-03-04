---
date: 25-02-2024
Time: 14:24
---
# Types de données JSON

Le JSON (JavaScript Object Notation) prend en charge plusieurs types de données pour représenter une variété d'informations. Voici les principaux types de données JSON :

## Chaînes de caractères

Les chaînes de caractères sont des séquences de caractères Unicode délimitées par des guillemets doubles (`"`). Elles peuvent contenir n'importe quel caractère Unicode, y compris des espaces, des symboles, et des caractères spéciaux.

Exemple :
```json
"Bonjour, monde!"
```

## Nombres

Les nombres peuvent être des entiers ou des décimaux et sont écrits sans guillemets.

Exemples :
```json
42
3.14
```

## Booléens

Les valeurs booléennes représentent la vérité (`true`) ou le faux (`false`), et sont écrites sans guillemets.

Exemple :
```json
true
```

## Tableaux

Les tableaux sont des collections ordonnées de valeurs, séparées par des virgules et entourées de crochets (`[]`). Les valeurs peuvent être de n'importe quel type JSON, y compris d'autres tableaux ou objets.

Exemple :
```json
[1, 2, 3, "quatre", true]
```

## Objets JSON

Les objets sont des collections non ordonnées de paires clé-valeur, où les clés sont des chaînes de caractères et les valeurs peuvent être de n'importe quel type JSON. Ils sont entourés d'accolades (`{}`). Chaque paire clé-valeur est séparée par une virgule.

Exemple :
```json
{
  "nom": "Jean",
  "age": 30,
  "estEtudiant": false
}
```

## Valeur nulle

La valeur `null` représente l'absence de valeur ou la valeur indéfinie.

Exemple :
```json
null
```

En résumé, le JSON prend en charge une variété de types de données pour représenter différentes informations de manière structurée et flexible.