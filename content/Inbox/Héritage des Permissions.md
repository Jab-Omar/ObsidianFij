---
tags:
  - Windows
date: 2023-10-30
---
# Héritage des Permissions

L'héritage des permissions est un concept essentiel en matière de gestion des autorisations dans les systèmes d'exploitation Windows. Il définit la manière dont les autorisations sont transmises automatiquement des objets parents aux objets enfants, tels que les dossiers, les fichiers ou les sous-dossiers. Comprendre comment fonctionne l'héritage des permissions est crucial pour maintenir un environnement informatique sécurisé et efficace.

## Comment fonctionne l'héritage des permissions ?

Lorsque vous créez un nouvel objet, tel qu'un dossier, il hérite généralement des autorisations de son objet parent. L'objet parent est l'objet au niveau supérieur de la hiérarchie, tel qu'un répertoire racine ou un dossier parent. Les autorisations accordées à l'objet parent sont automatiquement transmises à l'objet enfant, à moins que l'héritage ne soit explicitement désactivé.

## Options courantes liées à l'héritage :

1. **Désactiver l'héritage** : Vous avez la possibilité de désactiver complètement l'héritage des autorisations pour un objet spécifique. Cela signifie que l'objet enfant n'héritera plus des autorisations de l'objet parent. Vous devrez définir des autorisations spécifiques pour cet objet et ses sous-objets, s'il y en a.

2. **Rendre l'héritage explicite** : Au lieu de désactiver l'héritage, vous pouvez choisir de rendre l'héritage explicite. Cela signifie que l'objet enfant conserve toujours les autorisations héritées de l'objet parent, mais il reçoit également des autorisations spécifiques. Ainsi, il a des autorisations explicites en plus des autorisations héritées.

## Utilisation de l'héritage des permissions

L'héritage des permissions simplifie la gestion des autorisations en garantissant une cohérence dans les règles d'accès aux ressources. Par exemple, si un groupe d'utilisateurs a l'autorisation de lire un dossier parent, tous les sous-dossiers et fichiers qu'il contient hériteront de cette autorisation. Cela permet d'éviter de définir des autorisations pour chaque objet individuellement, ce qui serait fastidieux et difficile à gérer dans des environnements complexes.

Cependant, il est important de comprendre que l'héritage des permissions peut parfois créer des vulnérabilités potentielles. Si un utilisateur ou un groupe obtient des autorisations sur un objet parent au-delà de ce qui est nécessaire, ces autorisations peuvent être involontairement héritées par des objets enfants, donnant ainsi un accès inapproprié. Il est donc essentiel de surveiller et de gérer régulièrement les autorisations pour maintenir la sécurité du système.

Gérer l'héritage des permissions est une compétence fondamentale pour les administrateurs système et les responsables de la sécurité, car elle garantit que les autorisations sont correctement attribuées, maintenues et contrôlées dans un environnement informatique.

