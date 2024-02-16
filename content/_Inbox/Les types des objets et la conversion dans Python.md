---
date: 17-02-2024
Time: 00:03
---
# Les types des objets et la conversion

## Python : un langage dynamique et fortement typé

Python est un langage à la fois dynamique et fortement typé. Cela signifie que, d'une part, vous n'avez pas besoin de spécifier le type d'une variable lors de sa déclaration, car Python est capable de déduire automatiquement le type. Par exemple :

```python
a = 5  # Python déduit que 'a' est de type entier (int)
b = "Hello"  # Python déduit que 'b' est de type chaîne de caractères (str)
```

D'autre part, Python est fortement typé, ce qui signifie que les opérations entre des variables de types différents peuvent générer des erreurs, à moins qu'elles ne soient explicitement converties dans un type compatible. Par exemple :

```python
x = 5
y = "10"
z = x + y  # Cette opération générera une erreur car on ne peut pas additionner un entier et une chaîne de caractères sans conversion
```

## Les fonctions de conversion

Python fournit des fonctions intégrées pour convertir des données d'un type à un autre. Voici quelques-unes des fonctions de conversion les plus couramment utilisées :

- `int()` : Convertit une valeur en un entier.
- `float()` : Convertit une valeur en un nombre à virgule flottante.
- `str()` : Convertit une valeur en une chaîne de caractères.
- `bool()` : Convertit une valeur en un booléen.

Exemple d'utilisation de ces fonctions :

```python
num_str = "10"
num_int = int(num_str)  # Convertit la chaîne "10" en entier 10
print(num_int)  # Affiche : 10

float_num = 3.14
int_num = int(float_num)  # Convertit le nombre à virgule flottante 3.14 en entier 3
print(int_num)  # Affiche : 3

int_num = 5
str_num = str(int_num)  # Convertit l'entier 5 en chaîne de caractères "5"
print(str_num)  # Affiche : "5"

bool_val = False
int_val = int(bool_val)  # Convertit le booléen False en entier 0
print(int_val)  # Affiche : 0
```

Ces fonctions de conversion sont utiles lorsque vous avez besoin de manipuler des données dans différents types ou formats. Elles vous permettent de travailler avec les données de manière flexible et de les adapter aux besoins de votre programme.