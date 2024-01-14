# Laboratoire : Surveillance Système avec Redirections d'E/S

## Objectif

Ce laboratoire a pour objectif de vous familiariser avec le système de surveillance sous Linux en utilisant diverses techniques de redirection d'E/S, des méthodes simples aux plus avancées, ainsi que des combinaisons de redirections pour gérer les entrées et sorties.

## Étapes du Laboratoire

### 1. Surveillance Système Basique

- **Objectif** : Utiliser des commandes simples pour surveiller l'utilisation du système.
- **Instructions** :
    - Utilisez `free` pour afficher la mémoire système :
    - Redirigez la sortie de `free` vers un fichier pour une analyse future 
        `free -h > memory_usage.txt`

### 2. Surveillance Avancée avec Redirections Spéciales

- **Objectif** : Utiliser des redirections spéciales pour surveiller et filtrer les données système.
- **Instructions** :
    - Utilisez `journalctl` pour afficher les journaux du système :
        `journalctl`
    - Recherchez des messages spécifiques liés à un service et redirigez-les vers un fichier :
        `journalctl -u nom_du_service > service_logs.txt`

### 3. Combinaison de Redirections et Surveillance

- **Objectif** : Combiner plusieurs commandes de surveillance avec des redirections avancées.
- **Instructions** :
    - Utilisez `df` pour afficher l'espace disque utilisé :
        `df -h`
    - Trouvez les systèmes de fichiers les plus utilisés et redirigez-les vers un fichier :
        `df -h --output=target,pcent | sort -k 2 -h > disk_usage.txt`

### 4. Redirection Avancée avec Surveillance en Temps Réel

- **Objectif** : Surveiller en temps réel avec des redirections avancées.
- **Instructions** :
    - Utilisez `tail` pour surveiller un fichier journal en temps réel :
        `tail -f /chemin/vers/fichier_journal.log`
    - Redirigez la sortie vers un fichier pour enregistrer les données consultées :
        `tail -f /chemin/vers/fichier_journal.log > log_monitoring.txt`

### 5. Analyse Complète avec Combinaison de Redirections

- **Objectif** : Combiner plusieurs commandes avec des redirections pour une analyse approfondie.
- **Instructions** :
    - Utilisez `ps` pour afficher les processus et leurs informations :
        `ps aux` 
    - Triez et filtrez les processus pour trouver les plus consommateurs de mémoire et redirigez-les vers un fichier :
        `ps aux --sort=-%mem | head -n 10 > high_memory_processes.txt`

### 6. Conclusion
ce laboratoire est pertinent car il vous permet d'explorer en profondeur la surveillance système sous Linux tout en maîtrisant les techniques de redirections d'E/S. Cette expertise est cruciale pour gérer efficacement les ressources système, assurer la sécurité et optimiser les performances dans des environnements professionnels réels