---
date: 01-03-2024
Time: 14:10
---
# Utilisation de balises en YAML

Les balises en YAML permettent de spécifier le type d'une donnée de manière précise, notamment pour des cas où les types de données standard ne suffisent pas à représenter correctement l'information. Voici comment utiliser les balises en YAML :

## 1. Syntaxe des balises

Les balises sont représentées par le symbole '!' suivi d'un identifiant qui spécifie le type de données. Elles sont généralement placées avant la valeur qu'elles décrivent.

Exemple :

```yaml
date: !date 2024-03-01
```

Dans cet exemple, `!date` est une balise qui indique que la valeur `2024-03-01` représente une date.

## 2. Utilisation des balises prédéfinies

YAML définit un certain nombre de balises prédéfinies pour les types de données courants tels que les chaînes de caractères, les nombres, les booléens, etc. Ces balises peuvent être utilisées directement sans nécessiter de définition supplémentaire.

Exemple :

```yaml
prix: !float 10.50
```

Dans cet exemple, `!float` est une balise prédéfinie pour représenter un nombre flottant.

## 3. Définition de balises personnalisées

Il est également possible de définir des balises personnalisées pour des types de données spécifiques à une application. Cela permet d'étendre les fonctionnalités de YAML pour répondre à des besoins particuliers.

Exemple :

```yaml
produit:
  nom: "Ordinateur portable"
  prix: !euro 999.99
```

Dans cet exemple, `!euro` est une balise personnalisée qui représente un prix en euros.

En utilisant les balises en YAML, il est possible de représenter une grande variété de types de données de manière précise et flexible.
