# Laboratoire : Manipulation de Données avec I/O Redirections sous Linux

## Objectif

Ce laboratoire vise à pratiquer la manipulation de données dans un fichier en utilisant diverses commandes Linux et les I/O redirections pour gérer les entrées et sorties.

## Étapes du Laboratoire

### 1. Création du Fichier de Données

- **Objectif** : Créer un fichier de données pour les manipulations.
- **Instructions** :
    - Ouvrez un terminal.
    - Utilisez la commande suivante pour créer un nouveau fichier de données :
        `nano data.txt`
    - Ajoutez des lignes de données variées. Exemple :
	```yaml
	Nom,Âge,Ville,Profession
	Alice,25,Paris,Ingénieur
	Bob,30,Londres,Analyste
	Charlie,22,Berlin,Développeur
	Dave,28,New York,Consultant
	Emily,35,Los Angeles,Designer
	Frank,40,Sydney,Architecte
	Grace,27,Tokyo,Data Scientist
	Hannah,32,Rome,Manager
	Isaac,29,Barcelone,Ingénieur logiciel
	Julia,26,Moscou,Analyste financier
	Kevin,31,Amsterdam,Administrateur système
	Laura,24,San Francisco,Designer UX
	Michael,33,Berlin,Data Analyst
	Nina,29,Paris,Développeur web
	Olivia,36,Londres,Consultant en stratégie
	Patrick,39,New York,Ingénieur système
	Rachel,28,Los Angeles,Architecte logiciel
	Samuel,34,Sydney,Data Engineer
	Tina,31,Tokyo,Responsable de projet
	Ursula,27,Rome,Ingénieur en sécurité
	Victor,25,Barcelone,Designer industriel
	Wendy,30,Moscou,Analyste commercial
	Xavier,28,Amsterdam,Architecte réseau
	Yvonne,35,San Francisco,Analyste de données
	Zack,29,Berlin,Ingénieur logiciel
	```

### 2. Visualisation et Filtrage

- **Objectif** : Utiliser `cat`, `head`, `tail`, `grep`, et `find` pour visualiser et filtrer les données.
- **Instructions** :
    - Utilisez `cat` pour afficher le contenu du fichier de données :
        `cat data.txt`
    - Utilisez `head` et `tail` pour afficher les premières et dernières lignes du fichier :
        `head data.txt` 
        `tail data.txt`
    - Utilisez `grep` pour filtrer des lignes spécifiques. Exemple :
        `grep 'Paris' data.txt`

### 3. Manipulation des Données avec I/O Redirections

- **Objectif** : Utiliser `sed`, `sort`, `awk`, et les I/O redirections pour manipuler les données.
- **Instructions** :
    - Utilisez `sed` pour remplacer des valeurs spécifiques et rediriger la sortie vers un nouveau fichier. Exemple :
        `sed 's/Bob/Robert/' data.txt > modified_data.txt`
    - Utilisez `sort` pour trier les données par ordre alphabétique et rediriger la sortie vers un nouveau fichier. Exemple :
        `sort -k 2 -t',' data.txt > sorted_data.txt`
    - Utilisez `awk` pour effectuer des calculs sur les données et rediriger la sortie vers un fichier. Exemple :
        `awk -F',' '{sum+=$2} END {print "Moyenne d'âge :", sum/NR}' data.txt > stats.txt`

### 4. Utilisation de Pipes et Redirections Avancées

- **Objectif** : Appliquer des pipes, des redirections multiples et des redirections spéciales pour manipuler les données.
- **Instructions** :
    - Utilisez des pipes (`|`) pour combiner des commandes. Exemple :
        `cat data.txt | grep 'Paris' | sort -k 2 -t',' > sorted_paris.txt`
    - Utilisez les redirections multiples (`>2`) pour gérer les sorties multiples. Exemple :
        `grep 'Bob' data.txt > bob_info.txt 2> bob_error.txt`
    - Utilisez des redirections spéciales (`<<`) pour manipuler les entrées. Exemple :
        `wc -l <<EOF $(cat data.txt) EOF`


### 5. Conclusion
Imaginez-vous dans une bibliothèque ancestrale, entouré de piles de livres gigantesques représentant des données brutes. Chaque livre est une collection d'histoires sur des personnes du monde entier, avec leurs noms, âges, villes et professions. Vous êtes un maître de la bibliothèque, utilisant des lunettes magiques appelées I/O redirections pour extraire les histoires qui vous intéressent.

Lorsque vous lisez ces histoires, les commandes telles que `cat`, `grep`, `sed` et `awk` deviennent vos outils littéraires. Avec `cat`, vous ouvrez les livres et lisez les histoires de manière linéaire. `grep` devient votre guide, vous aidant à trouver des histoires spécifiques sur des villes ou des professions. `sed` agit comme un stylo magique, vous permettant de modifier les noms des personnages. Et `awk`, tel un savant, calcule des statistiques fascinantes sur les âges et les professions.

Chaque commande est une clé vers une histoire différente, vous permettant de découvrir des aspects uniques de ce monde littéraire de données. À la fin de chaque journée dans cette bibliothèque, vous partez avec une compréhension plus profonde de ces histoires, prêt à les partager et à les analyser avec confiance.