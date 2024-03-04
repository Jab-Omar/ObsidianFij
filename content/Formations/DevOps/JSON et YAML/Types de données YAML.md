---
date: 01-03-2024
Time: 14:00
---
# Types de données YAML

YAML prend en charge différents types de données pour représenter une variété d'informations. Voici une liste des types de données les plus courants en YAML :

## 1. Chaînes de caractères

Les chaînes de caractères sont utilisées pour représenter du texte. Elles peuvent être délimitées par des guillemets simples ('), des guillemets doubles ("), ou même sans guillemets dans certains cas.

Exemple :

```yaml
nom: "Jean Dupont"
adresse: '123 rue Principale'
email: jean.dupont@example.com
```

## 2. Nombres

Les nombres entiers et décimaux sont représentés sans guillemets et sont simplement écrits comme des nombres.

Exemple :

```yaml
age: 30
taille: 1.75
```

## 3. Booléens

Les valeurs booléennes sont représentées par les mots-clés `true` et `false`, en minuscules.

Exemple :

```yaml
est_actif: true
est_admin: false
```

## 4. Null

La valeur null est représentée par le mot-clé `null`, en minuscules.

Exemple :

```yaml
commentaire: null
```

## 5. Tableaux (Listes)

Les tableaux sont utilisés pour représenter une collection ordonnée d'éléments. Ils sont délimités par des crochets `[ ]` et les éléments sont séparés par des virgules.

Exemple :

```yaml
nombres:
  - 1
  - 2
  - 3
```

## 6. Objets (Dictionnaires)

Les objets sont utilisés pour représenter une collection non ordonnée d'éléments avec des clés associées. Ils sont délimités par des accolades `{ }` et chaque paire clé-valeur est séparée par des deux-points `:`.

Exemple :

```yaml
personne:
  nom: "Jean Dupont"
  age: 30
  ville: "Paris"
```

En utilisant ces types de données, YAML offre une grande flexibilité pour représenter une variété d'informations de manière structurée et lisible.
