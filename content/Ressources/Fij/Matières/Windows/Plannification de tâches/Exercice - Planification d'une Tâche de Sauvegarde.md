---
tags:
  - Windows
date: 2023-11-06
---
# Exercice : Planification d'une Tâche de Sauvegarde

**Objectif :** Planifiez une tâche qui effectue une copie de sauvegarde d'un fichier sur votre ordinateur.

**Étapes à Suivre :**

1. **Créez un Fichier à Sauvegarder :** Créez un fichier texte vide sur votre bureau ou dans un dossier de votre choix. Nommez-le "mon_fichier.txt".
    
2. **Planification de la Tâche :** Utilisez le Planificateur de Tâches pour planifier une tâche qui copie ce fichier vers un autre emplacement. Suivez ces étapes :
    
    - Ouvrez le Planificateur de Tâches en appuyant sur la touche `Windows` + `S` et en recherchant "Planificateur de Tâches".
    - Cliquez sur "Créer une Tâche de Base..." dans le panneau droit.
    - Donnez un nom à votre tâche (par exemple, "Sauvegarde de mon_fichier").
    - Choisissez de l'exécuter "Quotidiennement".
    - Spécifiez l'heure à laquelle vous souhaitez que la sauvegarde ait lieu.
    - Sélectionnez "Démarrer un Programme" comme action.
    - Parcourez et choisissez un programme de copie de fichiers, comme `xcopy` ou `robocopy`. Si vous n'avez pas de programme spécifique, vous pouvez utiliser `robocopy`, qui est inclus avec Windows.
    - Configurez les arguments pour copier votre fichier dans un autre dossier. Par exemple, `C:\Chemin\vers\Dossier\Sauvegarde\ mon_fichier.txt`.
    - Cliquez sur "Suivant" et terminez la configuration de la tâche.
3. **Testez la Tâche :** Attendez l'heure planifiée ou exécutez manuellement la tâche depuis le Planificateur de Tâches. Vérifiez si le fichier est copié avec succès dans le dossier de sauvegarde.