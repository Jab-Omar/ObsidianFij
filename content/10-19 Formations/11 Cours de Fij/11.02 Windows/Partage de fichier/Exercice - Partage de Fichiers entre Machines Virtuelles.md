---
date: 2023-11-20
---
### Exercice : Partage de Fichiers entre Machines Virtuelles

#### Objectif :

Partager un dossier entre deux machines virtuelles pour permettre l'accès aux fichiers de l'une à l'autre.

#### Prérequis :

- Deux machines virtuelles fonctionnelles (par exemple, sous VirtualBox ou VMware).
- Les machines doivent être sur le même réseau virtuel.

#### Étapes :

1. **Configuration des Machines Virtuelles** :
    
    - Assurez-vous que les deux machines virtuelles sont allumées et connectées au même réseau virtuel.
2. **Création d'un Dossier à Partager** :
    
    - Sur la machine A, créez un dossier (par exemple, "PartageVM") contenant des fichiers que vous souhaitez partager.
3. **Configuration du Partage sur la Machine A** :
    
    - Sur la machine A, configurez le dossier "PartageVM" pour le partager avec la machine B :
        - Dans les paramètres de partage ou les propriétés du dossier, activez le partage et définissez les autorisations pour permettre l'accès à la machine B.
4. **Accès depuis la Machine B** :
    
    - Sur la machine B, accédez au dossier partagé depuis la machine A :
        - Ouvrez l'explorateur de fichiers et accédez au réseau ou utilisez l'adresse IP de la machine A (`\\adresse_IP_de_la_machine_A\PartageVM`).
5. **Vérification de l'Accès** :
    
    - Essayez d'ouvrir et de modifier les fichiers du dossier partagé depuis la machine B pour vérifier l'accès.

#### Remarques :

- Assurez-vous que les paramètres de partage et les autorisations sont correctement configurés sur la machine A pour permettre l'accès depuis la machine B.
- Vérifiez les paramètres réseau des machines virtuelles pour garantir qu'elles sont sur le même sous-réseau et peuvent se voir mutuellement.
- Pour dépanner, assurez-vous que les pare-feux des machines virtuelles autorisent le partage de fichiers.

Cet exercice simple devrait vous permettre de pratiquer le partage de fichiers entre deux machines virtuelles, vous aidant à comprendre les étapes de configuration et les points à vérifier pour assurer un partage réussi.