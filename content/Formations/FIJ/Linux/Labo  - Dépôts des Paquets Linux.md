---
date: 2023-12-30
---
# Laboratoire Pratique : Gestion des Paquets Linux

## APT (Debian/Ubuntu)

1. **Vérification et Maintenance :**
    
    - Mettre à jour la liste des paquets : `sudo apt update`
    - Vérifier les mises à jour disponibles : `sudo apt list --upgradable`
    - Vérifier les informations d'un paquet : `apt show nom_paquet`
2. **Installation et Mise à Jour :**
    
    - Installer un paquet : `sudo apt install nom_paquet`
    - Mettre à jour un paquet : `sudo apt upgrade nom_paquet`
    - Mettre à jour tous les paquets : `sudo apt upgrade`
3. **Désinstallation :**
    
    - Désinstaller un paquet : `sudo apt remove nom_paquet`
    - Purger un paquet (suppression complète) : `sudo apt purge nom_paquet`

## YUM / DNF (Fedora, CentOS)

1. **Recherche et Gestion :**
    
    - Rechercher un paquet : `yum search nom_paquet`
    - Afficher des informations sur un paquet : `yum info nom_paquet`
2. **Installation et Mise à Jour :**
    
    - Installer un paquet : `sudo yum install nom_paquet`
    - Mettre à jour un paquet : `sudo yum update nom_paquet`
3. **Désinstallation :**
    
    - Désinstaller un paquet : `sudo yum remove nom_paquet`

## Autres Gestionnaires de Paquets

1. **Pacman (Arch Linux) :**
    - Installer un paquet : `pacman -S nom_paquet`
    - Mettre à jour la base de données : `pacman -Sy`
2. **Emerge (Gentoo) :**
    - Installer un paquet : `emerge nom_paquet`
    - Mettre à jour le système : `emerge --sync && emerge --update --deep --with-bdeps=y @world`
3. **Opkg (OpenWrt) :**
    - Installer un paquet : `opkg install nom_paquet`
    - Mettre à jour la liste des paquets : `opkg update`