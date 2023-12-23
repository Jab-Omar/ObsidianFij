## Objectif

Simuler l'analyse d'un fichier de logs fictif en utilisant les commandes d'I&O Redirections sous Linux.

## Étapes du Laboratoire

### 1. Création d'un Fichier de Logs Fictif

- **Objectif** : Créer un fichier de logs fictif pour simuler des données de logs.
- **Instructions** :
    - Ouvrez un terminal.
    - Utilisez la commande suivante pour créer un nouveau fichier de logs :
        `nano logs.txt`
    - Ajoutez des lignes fictives de logs. Exemple de contenu :
		```yaml
		 2023-12-23 10:00:00 INFO: User logged in successfully. 
	     2023-12-23 10:05:00 ERROR: Page not found - 404. 
	     2023-12-23 10:10:00 WARNING: High CPU usage detected.
	     ```
        

### 2. Extraction et Filtrage d'Informations

- **Objectif** : Utiliser `grep`, `sort`, et d'autres commandes pour extraire des informations spécifiques du fichier de logs.
- **Instructions** :
    - Utilisez `grep` pour rechercher des lignes spécifiques dans le fichier de logs. Exemple :
        `grep 'ERROR' logs.txt > errors.log`
    - Utilisez `sort` pour trier les résultats. Exemple :
        `grep 'WARNING' logs.txt | sort`
### 3. Analyse des Données

- **Objectif** : Utiliser `awk`, des pipes et d'autres commandes pour analyser et extraire des données pertinentes.
- **Instructions** :
    - Utilisez `awk` pour sélectionner et afficher des colonnes spécifiques. Exemple :
        `awk '{print $1, $5}' logs.txt`
    - Combinez des commandes avec des pipes pour un filtrage avancé. Exemple :
        `cat logs.txt | grep 'INFO' | awk '{print $2}'`

### 4. Conclusion

- **Objectif** : Résumez vos découvertes et identifiez les commandes utilisées pour analyser les logs.
- **Instructions** :
    - Faites une synthèse des informations extraites.
    - Identifiez et commentez les commandes utilisées pour chaque type d'analyse.