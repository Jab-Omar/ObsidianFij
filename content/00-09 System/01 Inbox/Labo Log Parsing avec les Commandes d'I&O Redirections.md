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
			2023-12-23 10:00:00 INFO: Connexion de l'utilisateur réussie.
			2023-12-23 10:05:00 ERROR: Page introuvable - 404.
			2023-12-23 10:10:00 WARNING: Détection d'une utilisation élevée du processeur (CPU).
			2023-12-23 10:15:00 INFO: Processus de sauvegarde démarré.
			2023-12-23 10:20:00 ERROR: Échec de la sauvegarde - Espace de stockage insuffisant.
			2023-12-23 10:25:00 INFO: Redémarrage du serveur pour maintenance planifiée.
			2023-12-23 10:30:00 WARNING: Trafic réseau anormalement élevé.
			2023-12-23 10:35:00 ERROR: Base de données inaccessible.
			2023-12-23 10:40:00 INFO: Mise à jour du système terminée avec succès.
			2023-12-23 10:45:00 WARNING: Température du processeur critique détectée.
			2023-12-23 10:50:00 ERROR: Panne de l'alimentation électrique.
			2023-12-23 10:55:00 INFO: Restauration des données à partir d'une sauvegarde.
			2023-12-23 11:00:00 INFO: Connexion SSH établie depuis une adresse IP inconnue.
			2023-12-23 11:05:00 WARNING: Disponibilité du disque dur en dessous du seuil critique.
			2023-12-23 11:10:00 ERROR: Erreur système inattendue.
			2023-12-23 11:15:00 INFO: Terminaison du processus système.
			2023-12-23 11:20:00 ERROR: Perte de connexion au réseau.
			2023-12-23 11:25:00 WARNING: Anomalie détectée dans les logs du système.
			2023-12-23 11:30:00 INFO: Changement du mot de passe utilisateur.
			2023-12-23 11:35:00 WARNING: Activité inhabituelle sur le compte administrateur.
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