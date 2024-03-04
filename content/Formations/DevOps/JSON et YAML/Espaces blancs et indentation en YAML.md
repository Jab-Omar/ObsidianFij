---
date: 01-03-2024
Time: 13:59
---
# Espaces blancs et indentation en YAML

L'indentation et les espaces blancs jouent un rôle crucial dans la syntaxe YAML. Ils sont utilisés pour définir la structure hiérarchique des données et doivent être appliqués de manière cohérente pour garantir la lisibilité et l'interprétation correcte des documents YAML.

## Indentation

En YAML, l'indentation est utilisée pour définir la structure hiérarchique des données. Les éléments de données imbriqués doivent être indentés par rapport à leurs éléments parents pour indiquer leur relation hiérarchique. L'indentation est généralement réalisée en utilisant des espaces, bien que certains éditeurs puissent autoriser l'utilisation de tabulations.

Exemple :

```yaml
livre:
  titre: "Le Seigneur des Anneaux"
  auteur: "J.R.R. Tolkien"
  chapitres:
    - Chapitre 1
    - Chapitre 2
```

Dans cet exemple, les éléments `titre`, `auteur` et `chapitres` sont indentés par rapport à l'élément parent `livre`, indiquant qu'ils sont des sous-éléments de `livre`.

## Espaces blancs

Les espaces blancs sont utilisés pour séparer les éléments de données et pour améliorer la lisibilité du document YAML. Bien que YAML ne spécifie pas le nombre exact d'espaces à utiliser pour l'indentation, il est recommandé d'utiliser deux ou quatre espaces pour chaque niveau d'indentation, pour garantir la cohérence et la lisibilité du code.

Exemple :

```yaml
livre:
  titre: "Le Seigneur des Anneaux"
  auteur: "J.R.R. Tolkien"
  chapitres:
    - Chapitre 1
    - Chapitre 2
```

Dans cet exemple, les espaces blancs sont utilisés pour séparer les éléments de données et pour aligner les différents niveaux d'indentation, ce qui rend le document YAML plus lisible pour les humains.

En résumé, l'indentation et les espaces blancs sont des éléments essentiels de la syntaxe YAML, utilisés pour définir la structure hiérarchique des données et pour améliorer la lisibilité du code YAML. Il est important de les utiliser de manière cohérente pour garantir la validité et la compréhensibilité des documents YAML.
