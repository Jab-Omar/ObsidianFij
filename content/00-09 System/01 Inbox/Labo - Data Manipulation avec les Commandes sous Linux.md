# Laboratoire : Data Manipulation avec les Commandes sous Linux

## Objectif

Exécuter des opérations de manipulation de données sur des fichiers en utilisant des commandes courantes sous Linux.

## Étapes du Laboratoire

### 1. Création d'un Fichier de Données Fictif

- **Objectif** : Créer un fichier de données fictif pour simuler des données à manipuler.
- **Instructions** :
    - Ouvrez un terminal.
    - Utilisez la commande suivante pour créer un nouveau fichier de données :
        `nano data.txt`
    - Ajoutez des lignes fictives de données. Exemple de contenu :
        ```
        Nom,Âge,Ville 
        Alice,25,Paris 
        Bob,30,Londres 
        Charlie,22,Berlin
        ```
        

### 2. Visualisation et Filtrage des Données

- **Objectif** : Utiliser `cat`, `head`, `tail`, et `grep` pour visualiser et filtrer les données.
- **Instructions** :
    - Utilisez `cat` pour afficher le contenu du fichier de données :
        `cat data.txt`
    - Utilisez `head` et `tail` pour afficher les premières et dernières lignes du fichier :
        `head data.txt tail data.txt`
    - Utilisez `grep` pour filtrer des lignes spécifiques. Exemple :
        `grep 'Paris' data.txt`

### 3. Modification des Données

- **Objectif** : Utiliser `sed` pour modifier des données dans le fichier.
- **Instructions** :
    - Utilisez `sed` pour remplacer des valeurs spécifiques. Exemple :
        `sed -i 's/Bob/Robert/' data.txt`

### 4. Analyse Statistique des Données

- **Objectif** : Utiliser `awk` pour réaliser une analyse statistique simple.
- **Instructions** :
    - Utilisez `awk` pour effectuer des calculs sur les données. Exemple :
        `awk -F',' '{sum+=$2} END {print "Moyenne d'âge :", sum/NR}' data.txt`

### 5. Conclusion

- **Objectif** : Résumez vos manipulations de données et identifiez les commandes utilisées pour chaque opération.
- **Instructions** :
    - Faites une synthèse des opérations effectuées sur les données.
    - Identifiez et commentez les commandes utilisées pour chaque manipulation.