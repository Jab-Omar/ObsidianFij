---
date: 01-03-2024
Time: 14:09
---

# Personnalisation des types de données en YAML

YAML offre la possibilité de personnaliser les types de données pour répondre à des besoins spécifiques. Cela peut être réalisé en utilisant des balises personnalisées ou en définissant des types de données spécifiques dans le document YAML lui-même. Voici comment procéder :

## 1. Utilisation de balises personnalisées

Les balises personnalisées permettent de spécifier le type d'une donnée d'une manière spécifique à l'application. Elles sont représentées par le signe '!' suivi d'un identifiant unique qui définit le type de données.

Exemple :

```yaml
prix: !euro 10.50
```

Dans cet exemple, `!euro` est une balise personnalisée qui indique que le nombre 10.50 représente un prix en euros.

## 2. Définition de types de données spécifiques

YAML permet également de définir des types de données spécifiques en utilisant la directive `%TAG`. Cela permet de mapper des préfixes à des URI qui définissent des types de données personnalisés.

Exemple :

```yaml
%TAG !myapp! tag:myapp.com,2010:app/
prix: !myapp!euro 10.50
```

Dans cet exemple, `%TAG !myapp!` définit le préfixe `!myapp!` comme étant associé à l'URI `tag:myapp.com,2010:app/`. Ensuite, `!myapp!euro` est utilisé comme balise personnalisée pour représenter un prix en euros.

## 3. Utilisation de types de données spécifiques

Une fois que des balises personnalisées ou des types de données spécifiques ont été définis, ils peuvent être utilisés pour représenter des données dans le document YAML.

Exemple :

```yaml
prix: !euro 10.50
```

Dans cet exemple, `!euro` est une balise personnalisée qui représente un prix en euros.

La personnalisation des types de données en YAML offre une grande flexibilité pour représenter des données de manière précise et adaptée à des besoins spécifiques d'application.
