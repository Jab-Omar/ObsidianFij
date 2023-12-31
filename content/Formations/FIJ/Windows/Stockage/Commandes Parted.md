---
date: 2023-10-29
---

## 1. **Afficher des Informations**

- `print devices`: Affiche la liste des disques disponibles.
- `print free`: Affiche les espaces non alloués sur le disque.
- `print list`: Affiche la liste des partitions sur le disque.

## 2. **Sélectionner un Disque**

- `select /dev/sdX`: Sélectionne un disque particulier (remplacez "X" par la lettre du disque, par exemple, /dev/sda).

## 3. **Créer une Partition**

- `mkpart primary [fs-type] start end`: Crée une nouvelle partition primaire avec un système de fichiers (facultatif) entre les positions "start" et "end".
- `mkpart logical [fs-type] start end`: Crée une nouvelle partition logique avec un système de fichiers (facultatif) entre les positions "start" et "end".
- `mkpart extended start end`: Crée une partition étendue entre les positions "start" et "end" (utilisée pour contenir des partitions logiques).

## 4. **Supprimer une Partition**

- `rm [partition number]`: Supprime la partition spécifiée par son numéro.

## 5. **Redimensionner une Partition**

- `resize [partition number] start end`: Redimensionne la partition spécifiée par son numéro entre les positions "start" et "end".

## 6. **Définir le Système de Fichiers**

- `set [partition number] [fs-type]`: Définit le type de système de fichiers sur une partition spécifiée par son numéro.

## 7. **Afficher l'État des Opérations en Attente**

- `print all`: Affiche l'état des opérations en attente avant d'appliquer les modifications.

## 8. **Appliquer les Modifications**

- `quit`: Applique les modifications et quitte Parted.

## Exemples d'Utilisation

1. Créer une partition primaire avec un système de fichiers ext4 sur /dev/sda de 10 Go à 20 Go :
   ```
   mkpart primary ext4 10GB 20GB
   ```

2. Supprimer la partition numéro 2 sur /dev/sdb :
   ```
   rm 2
   ```

3. Redimensionner la partition numéro 1 sur /dev/sdc de 30 Go à 40 Go :
   ```
   resize 1 30GB 40GB
   ```

N'oubliez pas que l'utilisation de Parted peut entraîner la perte de données si elle n'est pas effectuée avec précaution. Assurez-vous de sauvegarder vos données importantes avant de manipuler les partitions avec Parted.