---
date: 2023-11-06
---
# Exercice : Création d'un Script .bat pour Redémarrer la Machine

**Objectif :** Créez un script .bat pour redémarrer la machine, puis planifiez une tâche qui l'exécute chaque vendredi à 16h00.

**Étapes à Suivre :**

1. **Création du Script .bat :** Ouvrez un éditeur de texte, tel que le Bloc-notes, et saisissez la commande pour redémarrer la machine. Le contenu du script doit être : `shutdown /r /f /t 0`
    
    - `shutdown` : Commande de redémarrage.
    - `/r` : Redémarrer l'ordinateur.
    - `/f` : Forcer la fermeture des applications en cours d'exécution.
    - `/t 0` : Délai de 0 secondes avant le redémarrage.
    
    Enregistrez le fichier avec une extension .bat, par exemple "RedemarrerMachine.bat".
    
2. **Création de la Tâche Planifiée :**
    
    - Ouvrez le Planificateur de Tâches en appuyant sur la touche `Windows` + `S` et en recherchant "Planificateur de Tâches".
    - Cliquez sur "Créer une Tâche de Base..." dans le panneau droit.
    - Donnez un nom à votre tâche (par exemple, "Redémarrage Hebdomadaire").
    - Configurez la tâche pour qu'elle s'exécute une fois par semaine, chaque vendredi à 16h00 :
        - Dans l'onglet "Déclencheurs", cliquez sur "Nouveau" et configurez le déclencheur pour qu'il se produise chaque semaine, un vendredi, à 16h00.
    - Sélectionnez "Démarrer un Programme" comme action.
    - Cliquez sur "Parcourir" et sélectionnez le fichier de script .bat que vous avez créé précédemment.
3. **Test de la Tâche :** Attendez l'heure planifiée ou exécutez manuellement la tâche depuis le Planificateur de Tâches. Vérifiez si la machine redémarre avec succès.
    

**Bonus :**

Après avoir suivi ces étapes, la machine redémarrera automatiquement chaque vendredi à 16h00 en exécutant le script .bat que vous avez créé. Cette tâche planifiée simplifie le processus de redémarrage périodique de la machine, ce qui peut être utile pour la maintenance et l'optimisation du système.

N'oubliez pas de sauvegarder tous les travaux en cours avant l'heure prévue pour le redémarrage, car cette opération fermera toutes les applications en cours d'exécution.