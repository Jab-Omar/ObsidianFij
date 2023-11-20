---
date: 2023-10-29
---
# Sauvegarde Incrémentielle

La sauvegarde incrémentielle est une méthode de sauvegarde qui consiste à copier uniquement les données qui ont été modifiées depuis la dernière sauvegarde, qu'il s'agisse d'une sauvegarde complète ou d'une sauvegarde précédente. Cette approche permet de réduire la quantité de données sauvegardées, le temps nécessaire pour effectuer la sauvegarde, ainsi que l'espace de stockage requis pour les sauvegardes.

## Caractéristiques de la Sauvegarde Incrémentielle

- **Sauvegarde des Changements** : Une sauvegarde incrémentielle sauvegarde uniquement les données qui ont été modifiées ou ajoutées depuis la dernière sauvegarde.

- **Temps de Sauvegarde Réduit** : Par rapport à une sauvegarde complète, une sauvegarde incrémentielle nécessite généralement moins de temps, car elle se concentre sur les modifications récentes.

- **Économie d'Espace** : Puisque seules les modifications sont sauvegardées, les sauvegardes incrémentielles utilisent moins d'espace de stockage.

- **Restauration en Plusieurs Étapes** : Pour restaurer les données, il est souvent nécessaire de restaurer la dernière sauvegarde complète, suivie de toutes les sauvegardes incrémentielles successives.

- **Fréquence de Sauvegarde** : Les sauvegardes incrémentielles sont souvent effectuées fréquemment, par exemple quotidiennement, pour capturer les changements les plus récents.

## Planification de la Sauvegarde Incrémentielle

La planification des sauvegardes incrémentielles dépend de la fréquence des sauvegardes et du volume des données modifiées. Les utilisateurs et les administrateurs système doivent décider de la fréquence des sauvegardes incrémentielles en fonction des besoins en récupération.

## Utilisation de la Sauvegarde Incrémentielle

Les sauvegardes incrémentielles sont couramment utilisées pour capturer les modifications quotidiennes ou horaires des données, en minimisant le temps nécessaire pour effectuer la sauvegarde. Elles sont souvent associées à une sauvegarde complète initiale, de sorte que la restauration puisse être effectuée en combinant la sauvegarde complète avec les sauvegardes incrémentielles successives.
