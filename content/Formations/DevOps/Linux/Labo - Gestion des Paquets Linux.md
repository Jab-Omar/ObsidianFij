---
date: 2023-12-30
---
# Laboratoire : Gestion des Paquets Linux avec RPM sur CentOS 7
## Objectif

Comprendre et utiliser le gestionnaire de paquets `rpm` pour gérer l'installation, la mise à jour et la désinstallation des logiciels sous CentOS 7. De plus, installer un logiciel en utilisant `curl`.

## Prérequis

- Accès à un système CentOS 7.
- Connaissance de base en lignes de commande.

## Étapes

### Utilisation de `rpm` (gestionnaire de paquets basique)

1. **Lister les paquets installés :**
    
    - Utilise `rpm -qa` pour lister tous les paquets installés sur le système CentOS 7.
2. **Vérifier l'installation d'un paquet :**
    
    - Choisis un paquet (par exemple `wget`) et vérifie s'il est installé avec `rpm -q nom_du_paquet`.
3. **Lister les fichiers d'un paquet installé :**
    
    - Utilise `rpm -ql nom_du_paquet` pour lister les fichiers installés par le paquet sélectionné (`wget`).
4. **Obtenir des informations sur un paquet installé :**
    
    - Utilise `rpm -qi nom_du_paquet` pour obtenir des informations détaillées sur un paquet déjà installé (`wget`).
5. **Installer un logiciel avec `rpm` :**
    
    - Télécharge un fichier RPM via `curl` ou tout autre moyen (par exemple `curl -O http://lien_vers_le_paquet.rpm`).
    - Installe ce paquet avec `rpm -i nom_du_paquet.rpm`.
6. **Désinstaller un paquet avec `rpm` :**
    
    - Utilise `rpm -e nom_du_paquet` pour désinstaller un paquet spécifique.

## Conclusion

Résume l'expérience en mettant en évidence l'utilisation exclusive de `rpm` pour la gestion des logiciels sur CentOS 7, y compris l'installation d'un logiciel via `curl`. Souligne l'importance et les limites de cette méthode dans la gestion des logiciels.