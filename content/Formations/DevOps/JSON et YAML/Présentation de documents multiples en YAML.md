---
date: 01-03-2024
Time: 14:11
---

# Présentation de documents multiples en YAML

YAML permet de représenter plusieurs documents dans un seul fichier en utilisant une syntaxe spécifique pour séparer les documents. Cela peut être utile dans des situations où vous souhaitez regrouper plusieurs ensembles de données connexes dans un seul fichier YAML. Voici comment présenter des documents multiples en YAML :

## 1. Délimiteur de documents

Pour séparer plusieurs documents YAML dans un seul fichier, vous utilisez un délimiteur de documents. Ce délimiteur est constitué de trois tirets (`---`) placés sur une ligne séparée entre chaque document.

Exemple :

```yaml
# Document 1
nom: "Jean Dupont"
age: 30

---
# Document 2
nom: "Alice Smith"
age: 25
```

Dans cet exemple, nous avons deux documents YAML séparés par `---`. Chaque document représente des informations sur une personne, avec un nom et un âge.

## 2. Traitement des documents

Lors de la lecture d'un fichier YAML contenant plusieurs documents, chaque document est traité individuellement comme s'il s'agissait d'un fichier YAML distinct. Cela signifie que vous pouvez accéder à chaque document séparément et le manipuler comme bon vous semble.

Exemple (en Python) :

```python
import yaml

# Charger le fichier YAML contenant plusieurs documents
with open('fichier.yaml') as f:
    documents = yaml.safe_load_all(f)

    # Parcourir chaque document
    for doc in documents:
        print(doc)
```

Dans cet exemple Python, nous utilisons la méthode `safe_load_all()` pour charger tous les documents YAML du fichier `fichier.yaml`, puis nous parcourons chaque document individuellement et les affichons.

En utilisant la présentation de documents multiples en YAML, vous pouvez organiser vos données de manière modulaire et regrouper des ensembles de données connexes dans un seul fichier YAML.
