---
date: 2023-11-20
---
### Exercice : Partage de Fichiers entre Windows et Linux

#### Objectif :

Partager un dossier entre un système Windows et un système Linux pour permettre l'accès aux fichiers de l'un à l'autre.

#### Prérequis :

- Deux machines virtuelles fonctionnelles : une sous Windows et une sous Linux.
- Les deux machines virtuelles doivent être sur le même réseau virtuel.

#### Étapes :

1. **Configuration des Machines Virtuelles** :
    
    - Assurez-vous que les deux machines virtuelles sont allumées et connectées au même réseau virtuel.
2. **Création d'un Dossier à Partager sur Windows** :
    
    - Sur la machine Windows, créez un dossier (par exemple, "PartageWin") contenant des fichiers à partager.
3. **Configuration du Partage sur Windows** :
    
    - Sur la machine Windows, configurez le dossier "PartageWin" pour le partager avec la machine Linux :
        - Clic droit sur le dossier, allez dans "Propriétés" > "Partage" > "Partager" et définissez les autorisations pour permettre l'accès à la machine Linux.
4. **Accès depuis Linux** :
    
    - Sur la machine Linux, accédez au dossier partagé sur la machine Windows :
        - Utilisez l'outil de gestion de fichiers ou le terminal pour accéder au partage Windows via le protocole SMB (`smb://adresse_IP_de_la_machine_Windows/PartageWin`).
5. **Vérification de l'Accès** :
    
    - Essayez d'ouvrir et de manipuler les fichiers du dossier partagé depuis Linux pour vérifier l'accès.

#### Remarques :

- Assurez-vous que le partage sur Windows est configuré avec des autorisations appropriées pour permettre l'accès depuis Linux.
- Vérifiez que les deux machines virtuelles peuvent se voir mutuellement sur le réseau virtuel et que les paramètres de partage sont correctement configurés.
- Si nécessaire, vérifiez les paramètres de pare-feu des deux systèmes pour autoriser le partage de fichiers.

Cet exercice vous permettra de pratiquer le partage de fichiers entre un système Windows et un système Linux, en vous guidant à travers les étapes de configuration et en mettant l'accent sur la compatibilité entre les deux systèmes d'exploitation pour un partage réussi.