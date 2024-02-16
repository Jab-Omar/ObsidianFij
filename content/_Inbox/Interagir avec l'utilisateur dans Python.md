---
date: 17-02-2024
Time: 00:22
---

# Interagir avec l'utilisateur dans Python

Il est courant dans un script d'avoir besoin de demander des informations à l'utilisateur, comme la taille d'une image à modifier, une URL de site web, ou un chemin de dossier où écrire des données.

## La fonction `input()`

La fonction `input()` est utilisée pour cela en Python. Elle accepte un argument correspondant au texte à afficher à l'utilisateur.

Exemple :
```python
age = input("Quel âge avez-vous ? ")
```

L'utilisateur peut alors répondre après le texte affiché.

La saisie de l'utilisateur est ensuite retournée par la fonction `input()` :

```python
age = input("Quel âge avez-vous ? ")
print(age)
```

Depuis Python 3, `input()` retourne **toujours** une chaîne de caractères. Ainsi, pour traiter les nombres entrés comme des nombres, vous devez les convertir en utilisant `int()` ou `float()` :

```python
age = input("Quel âge avez-vous ? ")
age = int(age)
```

## Python 2 vs Python 3

Dans Python 2, il existait deux fonctions pour récupérer les données de l'utilisateur : `input()` et `raw_input()`.

- `raw_input()` était l'équivalent de `input()` dans Python 3.
- `input()` dans Python 2 interprétait la saisie de l'utilisateur comme Python le ferait normalement.

Python 3 a conservé `raw_input()` mais l'a renommée en `input()`. Maintenant, `input()` retourne toujours une chaîne de caractères.

Cela peut sembler contraignant, mais cela donne plus de contrôle au développeur pour valider et manipuler les données entrées par l'utilisateur.
