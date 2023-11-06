---
tags:
  - Windows
date: 2023-11-06
---
# Exercice Avancé : Planification d'une Tâche avec Options Personnalisées

**Objectif :** Planifiez une tâche qui effectue une sauvegarde quotidienne automatique de tous les fichiers modifiés dans un dossier spécifique vers un emplacement de sauvegarde.

**Étapes à Suivre :**

1. **Création d'un Dossier de Travail :** Créez un nouveau dossier sur votre bureau et nommez-le "MonDossier". Placez-y quelques fichiers texte pour simuler un ensemble de fichiers que vous souhaitez sauvegarder. Assurez-vous que le dossier "MonDossier" contient au moins un fichier texte.
    
2. **Planification de la Tâche :** Utilisez le Planificateur de Tâches pour planifier une tâche avec des options personnalisées :
    
    - Ouvrez le Planificateur de Tâches en appuyant sur la touche `Windows` + `S` et en recherchant "Planificateur de Tâches".
    - Cliquez sur "Créer une Tâche de Base..." dans le panneau droit.
    - Donnez un nom à votre tâche (par exemple, "Sauvegarde Quotidienne").
    - Configurez la tâche pour qu'elle s'exécute quotidiennement à une heure spécifique.
    - Sélectionnez "Démarrer un Programme" comme action.
    - Choisissez un utilitaire de sauvegarde de fichiers, tel que `robocopy`, qui est inclus avec Windows.
    - Dans les arguments, spécifiez les options de sauvegarde personnalisées. Par exemple :
        
        `/MIR /XO /R:1 /W:1 C:\Chemin\vers\MonDossier\ D:\Sauvegarde\`
        
        - `/MIR` : Miroiter (copier les fichiers, supprimer les fichiers inutiles dans la destination).
        - `/XO` : Exclure les fichiers déjà existants dans la destination.
        - `/R:1` : Nombre de tentatives de copie en cas d'échec.
        - `/W:1` : Temps d'attente entre les tentatives en secondes.
3. **Test de la Tâche :** Attendez l'heure planifiée ou exécutez manuellement la tâche depuis le Planificateur de Tâches. Vérifiez si les fichiers de "MonDossier" sont copiés avec succès dans le dossier de sauvegarde.
    

**Bonus :**

Après avoir créé et planifié la tâche avec des options avancées, Windows exécutera automatiquement la copie des fichiers du dossier "MonDossier" vers le dossier de sauvegarde. Les options `/MIR`, `/XO`, `/R`, et `/W` garantissent que seuls les fichiers modifiés sont copiés, et les tentatives de copie sont limitées en cas d'échec.

Cet exercice vous permet d'explorer des options avancées de planification de tâches avec Windows Task Scheduler, adaptées à des scénarios de sauvegarde plus complexes. Vous pouvez personnaliser davantage ces options en fonction de vos besoins spécifiques.