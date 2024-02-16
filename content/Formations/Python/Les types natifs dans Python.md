---
date: 14-02-2024
Time: 00:36
---

# Les Types Natifs en Python

Python offre plusieurs types de données natifs pour représenter différentes sortes de valeurs. Parmi ces types, on retrouve les chaînes de caractères, les nombres et les booléens, qui sont fondamentaux dans de nombreux programmes.

## Les chaînes de caractères

Les chaînes de caractères sont utilisées pour représenter du texte. Elles peuvent être définies en utilisant des guillemets simples ou doubles. Attention aux apostrophes dans le texte, elles peuvent causer des erreurs si elles ne sont pas gérées correctement.

```python
texte1 = "Bonjour, je m'appelle Thibault"
texte2 = 'Bonjour, je m\'appelle Thibault'
```

## Les nombres

Les nombres sont divisés en deux catégories principales : les entiers et les nombres à virgule flottante. Ils permettent de représenter divers types de données numériques, comme le solde d'un compte en banque, l'âge d'une personne, ou le nombre d'habitants dans une ville.

```python
entier = 42
flottant = 3.14
```

## Les booléens

Les booléens représentent les valeurs de vérité, c'est-à-dire vrai (`True`) ou faux (`False`). Bien que simples en apparence, ils sont fondamentaux pour la logique de contrôle dans les programmes. Ils permettent de prendre des décisions en fonction des résultats d'expressions logiques.

```python
vrai = True
faux = False
```

## Les constructeurs de types natifs

Python propose également des classes pour créer et convertir des objets de différents types. Ces classes sont utiles pour la conversion d'un type à un autre, par exemple de chaînes de caractères en nombres, ou vice versa.

```python
# Convertir une chaîne en nombre
nombre = int("42")

# Convertir un nombre en chaîne
chaine = str(3.14)
```

Ces constructeurs sont utiles lorsque vous avez besoin de manipuler des données dans différents formats ou types.
