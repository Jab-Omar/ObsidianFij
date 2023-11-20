---
date: 2023-10-29
---
# Sauvegarde Différentielle

La sauvegarde différentielle est une méthode de sauvegarde qui capture toutes les données modifiées depuis la dernière sauvegarde complète. Contrairement à la sauvegarde incrémentielle, qui sauvegarde uniquement les données modifiées depuis la dernière sauvegarde (qu'elle soit complète ou différentielle), la sauvegarde différentielle sauvegarde les données modifiées depuis la dernière sauvegarde complète uniquement.

## Caractéristiques de la Sauvegarde Différentielle

- **Sauvegarde des Changements depuis la Dernière Sauvegarde Complète** : La sauvegarde différentielle capture toutes les données modifiées depuis la dernière sauvegarde complète.

- **Restauration en Deux Étapes** : Pour restaurer les données, vous devez d'abord restaurer la dernière sauvegarde complète, suivie de la sauvegarde différentielle la plus récente.

- **Utilisation d'Espace de Stockage** : La sauvegarde différentielle nécessite moins d'espace que la sauvegarde complète, car elle sauvegarde uniquement les données modifiées depuis la dernière sauvegarde complète.

- **Planification de Sauvegarde** : La planification des sauvegardes différentielles dépend de la fréquence des sauvegardes complètes et du volume des données modifiées.

## Utilisation de la Sauvegarde Différentielle

La sauvegarde différentielle est utile lorsque vous souhaitez capturer les modifications depuis la dernière sauvegarde complète, sans avoir à effectuer une sauvegarde incrémentielle qui pourrait potentiellement être plus volumineuse en termes de données à sauvegarder.

## Planification de la Sauvegarde Différentielle

La planification des sauvegardes différentielles dépend de la fréquence des sauvegardes complètes et des besoins de récupération des données. Elle peut être planifiée pour être effectuée régulièrement, par exemple tous les jours ou toutes les semaines, en fonction de l'environnement informatique.

