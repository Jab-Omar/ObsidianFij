
# Commandes Vagrant

En tapant `vagrant` dans la ligne de commande, vous verrez s'afficher une liste de toutes les commandes disponibles.

Assurez-vous d'être dans le même répertoire que le fichier `Vagrantfile` lorsque vous exécutez ces commandes !

## Création d'une machine virtuelle

- `vagrant init` : initialise Vagrant avec un `Vagrantfile` et un répertoire `./.vagrant`, sans utiliser d'image de base spécifiée. Avant de pouvoir utiliser `vagrant up`, vous devrez spécifier une image de base dans le `Vagrantfile`.
- `vagrant init <chemin_de_la_boîte>` : initialise Vagrant avec une boîte spécifique. Pour trouver une boîte, consultez le catalogue public des boîtes Vagrant. Lorsque vous en trouvez une qui vous plaît, remplacez simplement son nom par le `chemin_de_la_boîte`. Par exemple, `vagrant init ubuntu/trusty64`.

## Démarrage d'une machine virtuelle

- `vagrant up` : démarre l'environnement Vagrant (provisionne également uniquement lors du PREMIER `vagrant up`).
- `vagrant resume` : reprend une machine suspendue (le `vagrant up` fonctionne également pour cela).
- `vagrant provision` : force la reprovision de la machine Vagrant.
- `vagrant reload` : redémarre la machine Vagrant, charge une nouvelle configuration `Vagrantfile`.
- `vagrant reload --provision` : redémarre la machine virtuelle et force la provision.

## Accès à une machine virtuelle

- `vagrant ssh` : se connecte à la machine via SSH.
- `vagrant ssh <nom_de_la_boîte>` : si vous donnez un nom à votre boîte dans votre `Vagrantfile`, vous pouvez vous y connecter via `nom_de_la_boîte`. Cela fonctionne depuis n'importe quel répertoire.

## Arrêt d'une machine virtuelle

- `vagrant halt` : arrête la machine Vagrant.
- `vagrant suspend` : suspend une machine virtuelle (mémoire d'état conservée).

## Nettoyage d'une machine virtuelle

- `vagrant destroy` : arrête et supprime toutes les traces de la machine Vagrant.
- `vagrant destroy -f` : pareil que ci-dessus, sans confirmation.

## Boîtes

- `vagrant box list` : voir la liste de toutes les boîtes installées sur votre ordinateur.
- `vagrant box add <nom> <URL>` : télécharger une image de boîte sur votre ordinateur.
- `vagrant box outdated` : vérifier les mises à jour `vagrant box update`.
- `vagrant box remove <nom>` : supprime une boîte de la machine.
- `vagrant package` : emballe un environnement VirtualBox en cours d'exécution dans une boîte réutilisable.

## Sauvegarde des progrès

- `vagrant snapshot save [options] [nom_de_la_vm] <nom>` : le `nom_de_la_vm` est souvent `default`. Nous permet de sauvegarder pour pouvoir revenir en arrière ultérieurement.

## Conseils

- `vagrant -v` : obtenir la version de Vagrant.
- `vagrant status` : affiche l'état de la machine Vagrant.
- `vagrant global-status` : affiche l'état de toutes les machines Vagrant.
- `vagrant global-status --prune` : pareil que ci-dessus, mais élimine les entrées invalides.
- `vagrant provision --debug` : utilisez le drapeau de débogage pour augmenter la verbosité de la sortie.
- `vagrant push` : oui, Vagrant peut être configuré pour déployer du code !
- `vagrant up --provision | tee provision.log` : lance `vagrant up`, force la provision et enregistre toute la sortie dans un fichier.

## Extensions

- `vagrant-hostsupdater` : `vagrant plugin install vagrant-hostsupdater` pour mettre à jour automatiquement votre fichier `/etc/hosts` à chaque démarrage/arrêt de votre boîte Vagrant.

## Remarques

Si vous utilisez VVV, vous pouvez activer xdebug en exécutant `vagrant ssh` puis `xdebug_on` depuis l'interface en ligne de commande de la machine virtuelle.
