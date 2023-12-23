# Laboratoire d'Apprentissage des Redirections d'E/S sous Linux

## 1. Redirection de la Sortie
- **Exercice 1**: Ouvrez un terminal et utilisez la commande `ls > list.txt` pour enregistrer la liste des fichiers du répertoire actuel dans un fichier nommé `list.txt`.

- **Exercice 2**: Utilisez la commande `date >> list.txt` pour ajouter la date et l'heure actuelles à la fin du fichier `list.txt`.

## 2. Redirection de l'Entrée
- **Exercice 3**: Utilisez `cat < input.txt` pour afficher le contenu du fichier `input.txt` dans le terminal.

## 3. Gestion des Erreurs
- **Exercice 4**: Utilisez la commande `grep 'mot_cle' fichier_inexistant 2> errors.log` pour rediriger les erreurs de la commande `grep` vers un fichier nommé `errors.log`.

## 4. Combinaison de Redirections
- **Exercice 5**: Exécutez `commande_inconnue &> output.txt` pour rediriger à la fois la sortie normale et les erreurs vers un fichier `output.txt`.

## 5. Utilisation de Pipes
- **Exercice 6**: Utilisez `ls | grep '.txt'` pour lister seulement les fichiers `.txt` du répertoire.

## 6. Manipulation des Descripteurs de Fichier
- **Exercice 7**: Redirigez la sortie standard vers `output.txt` avec `ls > output.txt`, puis restaurez-la vers le terminal avec `cat <&1`.

## 7. Défi Avancé
- **Exercice 8**: Créez un script Bash (`script.sh`) combinant `grep`, `sort`, et `uniq` avec des redirections pour filtrer, trier et enregistrer la sortie de différentes commandes.

---

_Ces exercices pratiques vous permettront de vous familiariser avec les redirections d'E/S sous Linux. Suivez les instructions dans votre terminal pour une meilleure compréhension pratique._
