---
tags:
  - Windows
date: 2023-10-30
---
## Création et Gestion des GPO

Les stratégies de groupe (GPO) sont un outil puissant qui permet aux administrateurs de Windows de gérer de manière centralisée les paramètres de configuration des ordinateurs et des utilisateurs.

**Exercices**

### Création d'une nouvelle GPO

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur le domaine ou l'unité d'organisation (OU) où vous souhaitez créer la GPO.
3. Dans le menu contextuel, cliquez sur **Nouveau**, puis sur **Objet de stratégie de groupe**.
4. Dans la boîte de dialogue **Nouvel objet de stratégie de groupe**, tapez un nom pour la GPO.
5. Cliquez sur **Créer**.

### Édition des paramètres de GPO

1. Ouvrez la GPO que vous souhaitez modifier.
2. Dans l'onglet **Paramètres**, sélectionnez la catégorie de paramètres que vous souhaitez modifier.
3. Double-cliquez sur le paramètre que vous souhaitez modifier pour ouvrir la boîte de dialogue de configuration.
4. Modifiez les valeurs du paramètre.
5. Cliquez sur **OK** pour appliquer les modifications.

### Gestion des liens de GPO

1. Ouvrez la GPO que vous souhaitez lier ou supprimer.
2. Dans l'onglet **Lien**, cliquez sur **Ajouter** pour lier la GPO à un domaine, une OU ou un groupe d'utilisateurs.
3. Cliquez sur **Désactiver** pour désactiver la GPO.
4. Cliquez sur **Supprimer** pour supprimer la GPO.

### Filtrage de sécurité pour les GPO

1. Ouvrez la GPO à laquelle vous souhaitez appliquer un filtre de sécurité.
2. Dans l'onglet **Filtrage de sécurité**, cliquez sur **Ajouter** pour créer un filtre de sécurité.
3. Sélectionnez les objets auxquels vous souhaitez appliquer la GPO.
4. Cliquez sur **OK**.

**Exemples**

* **Créer une GPO pour configurer la complexité des mots de passe**

1. Créez une nouvelle GPO et nommez-la "Complexité des mots de passe".
2. Dans la catégorie **Configuration de l'utilisateur**, double-cliquez sur le paramètre **Complexité des mots de passe**.
3. Dans la boîte de dialogue de configuration, définissez la valeur **Exigences de complexité des mots de passe** sur **Au moins 12 caractères**.
4. Cliquez sur **OK**.
5. Liez la GPO à votre domaine ou à une OU contenant les utilisateurs auxquels vous souhaitez appliquer la configuration.

* **Éditer une GPO pour désactiver la barre des tâches**

1. Ouvrez la GPO "Complexité des mots de passe" que vous avez créée précédemment.
2. Dans la catégorie **Configuration de l'ordinateur**, double-cliquez sur le paramètre **Barre des tâches**.
3. Dans la boîte de dialogue de configuration, définissez la valeur **Afficher la barre des tâches** sur **Non**.
4. Cliquez sur **OK**.

* **Supprimer une GPO**

1. Ouvrez la GPO "Complexité des mots de passe" que vous avez créée précédemment.
2. Dans l'onglet **Lien**, cliquez sur **Supprimer**.
3. Cliquez sur **Oui** pour confirmer la suppression.

**Conseils**

* Nommez vos GPO de manière descriptive afin de pouvoir les identifier facilement.
* Créez des GPO distinctes pour différents domaines, OU et groupes d'utilisateurs.
* Utilisez des filtres de sécurité pour limiter l'application des paramètres d'une GPO à un groupe spécifique d'utilisateurs ou d'ordinateurs.
* Testez vos GPO avant de les mettre en production.
