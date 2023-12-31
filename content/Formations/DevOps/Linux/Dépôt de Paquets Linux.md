---
date: 2023-12-30
---
# Dépôt de Paquets Linux

## Principe de Fonctionnement

- Un dépôt de paquets représente une source où sont stockés les logiciels (souvent déjà compilés) accessibles par un gestionnaire de paquets.
- Il peut s'agir de sources locales comme des CD/DVD, des serveurs HTTP/FTP, des miroirs de dépôts locaux ou distants (sur Internet).
- La définition d'un dépôt dépend de la distribution, de l'architecture matérielle et de la nature des sources officielles ou tierces.

## Gestion via les Gestionnaires de Paquets Avancés (APT, YUM/DNF)

- Un gestionnaire de paquets avancé comme APT ou YUM gère les sources logicielles, récupère les paquets à partir de ces sources, gère les dépendances et réalise les installations, mises à jour et désinstallations.
- APT (Advanced Package Tool) : utilisé principalement sur les distributions Debian/Ubuntu, automatisant la récupération de paquets à partir des sources APT.
- YUM (Yellowdog Updater Modified) / DNF (Dandified YUM) : utilisé sur des distributions telles que Fedora et Red Hat Enterprise Linux, gérant les installations et mises à jour.

## Configuration des Dépôts

- Dans APT, les sources des paquets sont définies dans le fichier `/etc/apt/sources.list`.
    - Les lignes commençant par `deb` spécifient les URLs des dépôts et leurs composants (main, universe, multiverse, etc.) pour différentes distributions (Debian, Ubuntu).
- Dans YUM/DNF, les configurations de dépôts se trouvent dans le répertoire `/etc/yum.repos.d/`.
    - Les fichiers `.repo` contiennent des déclarations de dépôts avec des informations comme le nom, l'URL du dépôt, les clés de vérification, etc.

## Utilisation des Dépôts via Commandes

- **Mise à jour de la liste des paquets :**
    - APT : `sudo apt update`
    - YUM/DNF : `sudo yum/dnf update`
- **Recherche de paquets :**
    - APT : `apt search nom_paquet`
    - YUM/DNF : `yum search nom_paquet`
- **Installation d'un paquet :**
    - APT : `sudo apt install nom_paquet`
    - YUM/DNF : `sudo yum install nom_paquet`
- **Suppression d'un paquet :**
    - APT : `sudo apt remove nom_paquet`
    - YUM/DNF : `sudo yum remove nom_paquet`

## Authentification des Paquets (Debian)

- Mécanisme de signature pour assurer l'authenticité des paquets installés, géré par APT via GnuPG.
- Les fichiers `Release` sur les miroirs Debian contiennent des listes de paquets et leurs sommes de contrôle pour garantir leur intégrité.
- La gestion des clés GPG se fait avec `apt-key`, assurant que les paquets proviennent des mainteneurs officiels.

## Autres Gestionnaires de Paquets

- **Pacman** (Arch Linux) : Gestionnaire de paquets pour Arch Linux, utilisé avec des commandes telles que `pacman -S nom_paquet`.
- **Emerge** (Gentoo) : Utilisé pour installer des logiciels sur Gentoo via `emerge nom_paquet`.
- **Opkg** (OpenWrt) : Gestionnaire de paquets pour OpenWrt, utilisé avec des commandes telles que `opkg install nom_paquet`.