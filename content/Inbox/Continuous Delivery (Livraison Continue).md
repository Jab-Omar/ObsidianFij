---
tags:
  - DevOps
date: 2023-10-31
---
# Continuous Delivery (Livraison Continue)

La Continuous Delivery (CD) est une composante essentielle du DevOps visant à automatiser le processus de livraison de logiciels de manière rapide, fiable et efficace. Elle s'étend naturellement à partir de la Continuous Integration (Intégration Continue) et garantit que le logiciel est toujours prêt à être déployé sur les serveurs de production.

## Processus de la Livraison Continue

Après la phase de Continuous Integration (CI), l'artefact généré est stocké dans un référentiel de logiciels (software repository). La Continuous Delivery englobe les étapes clés suivantes :

- **Provisionnement du Serveur :** Cette étape concerne la configuration des serveurs de production, y compris le provisionnement matériel et logiciel requis pour exécuter le logiciel.

- **Gestion des Dépendances :** Les dépendances logicielles nécessaires au fonctionnement du logiciel sont gérées pour garantir la compatibilité et la stabilité.

- **Changements de Configuration :** Les modifications de configuration sont appliquées pour adapter le logiciel à l'environnement de production.

- **Changements Réseau :** Les modifications réseau sont gérées pour assurer la connectivité, les performances et la sécurité nécessaires.

- **Déploiement de l'Artefact :** L'artefact généré lors de la CI est déployé sur les serveurs de production, permettant ainsi la mise en service du logiciel.

L'objectif principal de la Continuous Delivery est d'automatiser chaque étape du processus de déploiement, réduisant ainsi les erreurs humaines et accélérant le cycle de livraison.

## Outils de la Livraison Continue

Plusieurs outils et technologies sont associés à la Continuous Delivery. Parmi les outils couramment utilisés, on retrouve :

- **Outils de Configuration :** Des outils tels qu'Ansible, Puppet et Chef sont employés pour gérer la configuration des serveurs de production.

- **Terraform :** Il est utilisé pour provisionner et gérer l'infrastructure de manière automatisée.

- **Outils de CI/CD :** Des plateformes comme Jenkins, Octopus et d'autres outils spécifiques à la gestion du déploiement sont employés pour automatiser le processus de livraison.

- **Helm Chart :** Cet outil est utile pour gérer les applications Kubernetes.

- **Code Deploy :** Des solutions telles qu'AWS CodeDeploy permettent le déploiement automatisé d'applications sur les serveurs.

## Tests Automatisés

La Continuous Delivery comprend également une variété de tests automatisés pour garantir la qualité et la fiabilité du logiciel déployé. Ces tests incluent :

- **Tests Fonctionnels :** Ils vérifient que le logiciel fonctionne conformément aux spécifications et aux cas d'utilisation.

- **Tests de Charge :** Ils évaluent les performances du logiciel en conditions de charge élevée.

- **Tests de Performance :** Ils s'assurent que le logiciel répond aux exigences de performance établies.

- **Tests de Base de Données (DB) :** Ils garantissent l'intégrité des données et la performance de la base de données.

- **Tests Réseau :** Ils vérifient la connectivité et la sécurité du réseau dans l'environnement de production.

- **Tests de Sécurité :** Ils identifient et corrigent les vulnérabilités potentielles pour garantir la sécurité du logiciel.

La Continuous Delivery garantit que le logiciel est toujours prêt à être mis en production, ce qui réduit les délais et les risques associés aux déploiements.

