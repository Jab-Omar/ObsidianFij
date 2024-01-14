---
date: 2023-12-30
---
# Gestion des Paquets Linux

## Introduction aux Gestionnaires de Paquets

Les gestionnaires de paquets simplifient l'installation, la mise à jour et la désinstallation des logiciels sous Linux. Chaque paquet contient les fichiers nécessaires à l'installation et garantit la cohérence du système.

## Utilité des Gestionnaires de Paquets

Ces outils permettent :

- Installation, mise à jour et désinstallation des logiciels.
- Utilisation de paquets depuis diverses sources (CD, dépôts en ligne, partage réseau).
- Vérification des sommes de contrôle pour garantir l'intégrité.
- Gestion des dépendances pour assurer le bon fonctionnement.

## Types de Systèmes de Paquets

Deux grandes familles :

- **RPM** : Redhat, Fedora, CentOS.
- **DPKG** : Debian, Ubuntu, Mint, Raspbian.

Quelques autres systèmes notables :

- Portage/emerge pour Gentoo.
- Pacman pour Arch Linux.
- opkg pour OpenWRT.

## Utilitaire `dpkg` (Systèmes DPKG)

Dpkg gère les paquets *.deb des distributions Debian.

- Outil de base pour installer/désinstaller les fichiers .deb.
- Privilégier des outils avancés comme aptitude ou apt-get.

### Commandes Utiles avec `dpkg`

- Liste des paquets installés : `dpkg -l` ou `dpkg --get-selections`.
- Vérification de l'installation d'un paquet : `dpkg -s wget`.
- Liste des fichiers installés par un paquet : `dpkg -L wget`.
- Reconfiguration d'un paquet : `dpkg-reconfigure locales`.

## Utilitaire `rpm` (Autres Systèmes)

RPM gère les paquets sur d'autres distributions.

- Installation, mise à jour, désinstallation, vérification et recherche de paquets avec droits root.

### Commandes Utiles avec `rpm`

- Liste des paquets installés : `rpm -qa`.
- Vérification de l'installation d'un paquet : `rpm -q wget`.
- Liste des fichiers d'un paquet installé : `rpm -ql wget`.
- Informations sur un paquet installé : `rpm -qi wget`.
- Informations sur un paquet avant l'installation : `rpm -qip fichier.rpm`.