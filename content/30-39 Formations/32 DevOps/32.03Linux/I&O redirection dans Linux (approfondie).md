# I&O redirection dans Linux
## Quelques commandes bonus

- **`uptime`** : Cette commande affiche depuis combien de temps le système fonctionne, le nombre d'utilisateurs connectés et la charge moyenne du système pendant différentes périodes de temps.
    
- **`free -m`** : Cette commande affiche la quantité de mémoire RAM utilisée et disponible sur le système, en mégaoctets. L'option `-m` affiche les résultats en mégaoctets.
    
- **`df -h`** : Cette commande affiche l'utilisation de l'espace disque sur le système. L'option `-h` permet de présenter les résultats de manière lisible pour l'homme (en utilisant des unités telles que kilo, méga, giga, etc.) plutôt qu'en octets.
    
- **`echo`** : La commande `echo` est utilisée pour afficher du texte passé en argument sur la sortie standard (généralement, le terminal). Par exemple, `echo "Bonjour"` affichera simplement "Bonjour" dans le terminal.
    
- **`wc -l`** : Cette commande compte le nombre de lignes dans un fichier donné. L'option `-l` spécifie de ne compter que les lignes.
    
- **`find`** : La commande `find` est utilisée pour rechercher des fichiers et répertoires dans un système de fichiers en fonction de divers critères tels que le nom, la date de modification, la taille, etc.
    
- **`locate`** : La commande `locate` est utilisée pour trouver des fichiers en utilisant une base de données pré-construite. Pour l'installer, vous pouvez généralement utiliser `sudo apt install mlocate` sur les systèmes basés sur Debian/Ubuntu. Par rapport à `find`, `locate` est généralement plus rapide car il recherche dans une base de données préindexée au lieu de parcourir le système de fichiers en temps réel. Cependant, la base de données de `locate` doit être régulièrement mise à jour pour refléter les changements récents dans le système de fichiers.

---
## Output redirection ou redirection de sortie
Ces instructions utilisent la redirection de sortie pour rediriger les résultats de différentes commandes vers un fichier spécifique, `/tmp/sysinfo.txt`, dans le répertoire temporaire.

1. Exécute la commande suivante : 
```bash
uptime > /tmp/sysinfo.txt
```
Cela permettra de rediriger la sortie de la commande vers le fichier `sysinfo.txt` dans le répertoire `/tmp`. L'affichage des résultats se fera dans ce fichier plutôt qu'à l'écran. Pour consulter le contenu de ce fichier, utilise la commande `cat /tmp/sysinfo.txt`."

2. Effectue la commande suivante : 
```bash
ls > /tmp/sysinfo.txt
```
Cela écrasera le contenu précédent de `/tmp/sysinfo.txt` avec la sortie de la commande `ls`. Pour vérifier le contenu mis à jour, utilise la commande `cat /tmp/sysinfo.txt`.

3. Exécute la commande suivante : 
```bash
uptime >> /tmp/sysinfo.txt
```
L'opérateur `>>` permet d'ajouter les informations à la fin du fichier spécifié. Pour vérifier les données ajoutées, utilise la commande `cat /tmp/sysinfo.txt`.
  
4. Effectue la commande suivante : 
```bash
date > /tmp/sysinfo.txt`.
```


5. Voici la commande à exécuter : 
```bash
echo "##################################" >> /tmp/sysinfo.txt
```
  
6. Exécute la commande suivante : 
```bash
uptime >> /tmp/sysinfo.txt
```

7. Exécute la commande suivante :
```bash
echo "##################################" >> /tmp/sysinfo.txt
```

8. Exécute la commande suivante : 
```bash
free -m >> /tmp/sysinfo.txt
```

9. Exécute la commande suivante: 
```
echo "##################################" >> /tmp/sysinfo.txt
```

10. Exécute la commande suivante : 
```bash
df -h >> /tmp/sysinfo.txt
```

11. Exécute la commande suivante :
```bash
echo "##################################" >> /tmp/sysinfo.txt
```


12. Pour consulter le contenu du fichier, utilise la commande suivante : 
```bash
cat /tmp/sysinfo.txt.
```


### /dev/null

`/dev/null` est un périphérique spécial dans les systèmes Unix et Linux. C'est une destination pour les données, mais tout ce qui y est envoyé est simplement jeté, ce qui signifie que les données écrites dans `/dev/null` sont effectivement supprimées. C'est souvent utilisé pour supprimer des sorties ou des données sans les stocker.

#### Quelques exemples pour /dev/null
Dans l'exemple :
```bash
yum install vim -y > /dev/null
```
la commande `yum install vim -y` installe le programme Vim avec l'option `-y` pour répondre "oui" à toutes les questions posées par le gestionnaire de paquets yum. En ajoutant `> /dev/null` à la fin, cela redirige toute la sortie (comme les messages d'installation ou de confirmation) vers `/dev/null`, donc aucune sortie n'est affichée à l'écran.

Pour vider le contenu du fichier `/tmp/sysinfo.txt`, la commande 
```bash
cat /dev/null > /tmp/sysinfo.txt
```
est utilisée. Elle utilise `cat` pour lire le contenu de `/dev/null`, qui est vide, et ensuite redirige cette sortie vide vers `/tmp/sysinfo.txt`, ce qui remplace tout contenu précédent dans ce fichier par une sortie vide. Ainsi, le fichier `/tmp/sysinfo.txt` est vidé de son contenu.

Bien sûr, voici une note expliquant les opérateurs de redirection `1>`, `2>`, et `&>` utilisés dans les systèmes Linux/Unix pour la gestion des sorties.

---

## Opérateurs de redirection de sortie dans les commandes Linux/Unix

Lors de l'exécution de commandes dans un terminal Linux/Unix, il est possible de rediriger la sortie vers différents emplacements en utilisant des opérateurs spécifiques. Voici trois opérateurs couramment utilisés :

### `1>` (Redirection de la sortie standard - stdout)

L'opérateur `1>` est utilisé pour rediriger la sortie standard (stdout) d'une commande vers un fichier ou un périphérique spécifié. Par exemple :

```bash
commande > fichier.txt
```

Cela enregistrera la sortie normale de la commande `commande` dans le fichier `fichier.txt`.

### `2>` (Redirection de la sortie d'erreur standard - stderr)

L'opérateur `2>` est utilisé pour rediriger la sortie d'erreur standard (stderr) d'une commande vers un fichier ou un périphérique spécifié. Par exemple :

```bash
commande_inconnue 2> erreur.txt
```

Cela enregistrera les messages d'erreur générés par la commande inconnue dans le fichier `erreur.txt`.

### `&>` (Redirection de la sortie standard et de la sortie d'erreur)

L'opérateur `&>` est utilisé pour rediriger à la fois la sortie standard et la sortie d'erreur vers un fichier ou un périphérique spécifié. Par exemple :

```bash
commande &> sortie_erreur.txt
```

Cela enregistrera à la fois la sortie normale et les messages d'erreur de la commande dans le fichier `sortie_erreur.txt`.

Ces opérateurs permettent de contrôler où les résultats de la commande sont dirigés, que ce soit vers des fichiers pour une utilisation future ou vers `/dev/null` pour supprimer les sorties non nécessaires.

Dans le contexte des lignes de commande Linux/Unix, le pipe (`|`) est utilisé pour rediriger la sortie d'une commande vers l'entrée d'une autre. Cela permet de combiner les résultats de plusieurs commandes pour effectuer des opérations plus complexes.

--- 
## Utilisation du Pipe (`|`) pour la Redirection des Sorties dans Linux/Unix

Le pipe (`|`) est un opérateur utilisé dans les systèmes Linux/Unix pour rediriger la sortie d'une commande vers l'entrée d'une autre commande. Il permet de chaîner plusieurs commandes ensemble, utilisant la sortie d'une comme entrée pour une autre.

### Syntaxe :
```bash
commande1 | commande2
```

### Exemples :

#### 1. Compter les lignes dans un fichier :
```bash
cat fichier.txt | wc -l
```
- `cat fichier.txt` : Affiche le contenu du fichier `fichier.txt`.
- `|` : Le pipe transmet la sortie de `cat` à l'entrée de `wc -l`.
- `wc -l` : Compte le nombre de lignes de la sortie de `cat`, fournissant ainsi le nombre total de lignes dans `fichier.txt`.

#### 2. Filtrer les résultats d'une commande :
```bash
ls -l | grep "monFichier"
```
- `ls -l` : Liste les fichiers et dossiers dans le répertoire courant avec des détails.
- `|` : Le pipe transmet la sortie de `ls -l` à l'entrée de `grep`.
- `grep "monFichier"` : Filtre la sortie de `ls -l` pour afficher uniquement les lignes contenant "monFichier".

#### 3. Chaining multiple commands :
```bash
ps aux | grep "chrome" | wc -l
```
- `ps aux` : Affiche toutes les informations sur les processus en cours d'exécution.
- `|` : Le pipe transmet la sortie de `ps aux` à l'entrée de `grep`.
- `grep "chrome"` : Filtre les lignes contenant "chrome" parmi les processus.
- `|` : Un autre pipe transmet la sortie de `grep` à l'entrée de `wc -l`.
- `wc -l` : Compte le nombre de lignes résultant de la recherche, indiquant ainsi le nombre de processus associés à "chrome".

### Fonctionnalités clés :
- **Chainer les commandes :** Permet de combiner les résultats de différentes commandes pour des opérations complexes.
- **Traitement de flux :** Facilite le traitement continu des données, idéal pour filtrer, compter, ou modifier la sortie des commandes.

Le pipe (`|`) est un outil puissant pour manipuler les flux de données dans les environnements Linux/Unix, offrant une grande flexibilité dans l'exécution des commandes et la manipulation des résultats.

---

