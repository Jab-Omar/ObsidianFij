---
date: 2023-12-30
---
# Labo - Sudo
## Objectif du laboratoire :
Configurer les autorisations Sudo pour différents utilisateurs et groupes sur un système Linux.

## Étapes à suivre :

#### 1. Création des utilisateurs et du groupe :

##### Administrateur principal :
1. Créez un utilisateur administrateur principal nommé "sysadmin".
   ```bash
   sudo adduser sysadmin
   ```

Cette commande ajoute un nouvel utilisateur à votre système. Vous serez invité à saisir un mot de passe et des informations facultatives pour l'utilisateur.

##### Utilisateur de développement :
2. Créez un utilisateur de développement nommé "devuser".
   ```bash
   sudo adduser devuser
   ```

Encore une fois, saisissez les informations nécessaires pour créer cet utilisateur.

##### Groupe de maintenance :
3. Créez un groupe "maintenance".
   ```bash
   sudo groupadd maintenance
   ```

Cela crée un groupe nommé "maintenance" qui sera utilisé pour regrouper les utilisateurs ayant des autorisations spécifiques.

#### 2. Attribution des privilèges administratifs :

##### Administrateur principal :
4. Accordez des privilèges administratifs à l'utilisateur "sysadmin".
   ```bash
   sudo usermod -aG sudo sysadmin
   ```

Cette commande ajoute l'utilisateur "sysadmin" au groupe "sudo", qui est associé aux privilèges administratifs sur les systèmes basés sur Debian (comme Ubuntu). Sur les distribution RedHat il faudra ajouter l'utillisateur au groupe "wheel". 

#### 3. Configuration des autorisations dans sudoers :

##### Éditez le fichier sudoers :
5. Ouvrez le fichier sudoers pour édition.
   ```bash
   sudo visudo
   ```

##### Autorisations pour l'utilisateur de développement :

6. Autorisez l'utilisateur "devuser" à installer des paquets logiciels sans mot de passe.
   ```bash
   devuser ALL=(ALL) NOPASSWD: /usr/bin/apt-get install *
   ```

Cette ligne dans le fichier sudoers permet à "devuser" d'utiliser la commande `apt-get install` sans être invité à saisir un mot de passe.

##### Autorisations pour le groupe de maintenance :

7. Autorisez le groupe "maintenance" à effectuer des tâches de sauvegarde et de restauration sans mot de passe.
   ```bash
   %maintenance ALL=(ALL) NOPASSWD: /usr/bin/tar, /usr/bin/restore
   ```

Cette configuration autorise tous les membres du groupe "maintenance" à utiliser les commandes `tar` et `restore` sans nécessiter de mot de passe.

#### 4. Test des autorisations :

##### Administrateur principal :
8. Connectez-vous en tant que "sysadmin" et vérifiez les autorisations accordées.
   ```bash
   su - sysadmin
   sudo apt update
   ```

Cette séquence de commandes permet de vérifier que l'utilisateur "sysadmin" peut exécuter la commande `apt update` avec les privilèges administratifs. Pour RedHat c'est `yum update`. 

##### Utilisateur de développement :
9. Connectez-vous en tant que "devuser" et testez l'installation de paquets logiciels.
   ```bash
   su - devuser
   sudo apt-get install nom_du_paquet
   ```

Cela vous permet de tester si "devuser" peut installer des paquets logiciels sans mot de passe.

##### Groupe de maintenance :
10. Créez un utilisateur factice et ajoutez-le au groupe "maintenance". Vérifiez les autorisations pour cet utilisateur.
   ```bash
   sudo adduser fakeuser
   sudo usermod -aG maintenance fakeuser
   su - fakeuser
   sudo tar -cvf /chemin/vers/destination/fichier.tar /chemin/source
   ```

Cette séquence crée un nouvel utilisateur nommé "fakeuser", l'ajoute au groupe "maintenance", et teste si cet utilisateur peut utiliser la commande `tar` sans saisir de mot de passe.
## Autotest du laboratoire :

- Assurez-vous que chaque utilisateur a les autorisations appropriées.
- Testez également l'accès aux commandes non autorisées pour vous assurer que les restrictions fonctionnent.
- Vérifiez que les autorisations accordées au groupe "maintenance" sont correctement appliquées pour tous ses membres.

Ce laboratoire vous permettra de mettre en pratique la configuration de Sudo pour différents cas d'utilisation. Assurez-vous de tester et de vérifier chaque étape pour vous assurer que les autorisations sont correctement définies pour chaque utilisateur et groupe.