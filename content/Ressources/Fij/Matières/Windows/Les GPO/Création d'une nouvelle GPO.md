---
tags:
  - Windows
date: 2023-10-30
---
# Création d'une nouvelle GPO

Pour créer une nouvelle GPO, procédez comme suit :

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur le domaine ou l'unité d'organisation (OU) où vous souhaitez créer la GPO.
3. Dans le menu contextuel, cliquez sur **Nouveau**, puis sur **Objet de stratégie de groupe**.
4. Dans la boîte de dialogue **Nouvel objet de stratégie de groupe**, tapez un nom pour la GPO.
5. Cliquez sur **Créer**.

Une fois que vous avez créé une nouvelle GPO, vous pouvez commencer à configurer ses paramètres. Pour ce faire, ouvrez la GPO et naviguez vers l'onglet **Paramètres**.

**Paramètres**

L'onglet **Paramètres** contient tous les paramètres de configuration que vous pouvez configurer pour une GPO. Les paramètres sont organisés en catégories, telles que **Configuration de l'ordinateur**, **Configuration de l'utilisateur** et **Stratégies de sécurité**.

Pour configurer un paramètre, double-cliquez dessus pour ouvrir la boîte de dialogue de configuration. Dans la boîte de dialogue, vous pouvez modifier les valeurs du paramètre.

**Lien**

Une fois que vous avez configuré les paramètres de la GPO, vous devez la lier à un domaine, une OU ou un groupe d'utilisateurs. Lorsque vous liez une GPO à un objet, les paramètres de la GPO sont appliqués à tous les ordinateurs et utilisateurs associés à cet objet.

Pour lier une GPO, ouvrez la GPO et naviguez vers l'onglet **Lien**. Dans la liste **Objets liés**, cliquez sur **Ajouter**.

Dans la boîte de dialogue **Sélectionnez des objets**, sélectionnez le domaine, l'OU ou le groupe d'utilisateurs auquel vous souhaitez lier la GPO.

**Application**

Une fois que vous avez lié une GPO, vous devez la propager aux ordinateurs et utilisateurs associés à cet objet. La propagation d'une GPO peut prendre plusieurs heures, en fonction de la taille de votre environnement.

Pour propager une GPO, cliquez avec le bouton droit sur la GPO dans l'arborescence de la console et sélectionnez **Propager**.

**Validation**

Une fois que vous avez propagé une GPO, vous devez la valider pour vous assurer qu'elle fonctionne correctement. Pour valider une GPO, ouvrez la GPO et naviguez vers l'onglet **Analyse**. Cliquez sur **Analyser** pour lancer l'analyse.

**Résolution des problèmes**

Si vous rencontrez des problèmes avec une GPO, vous pouvez utiliser l'onglet **Journal** pour afficher les journaux de l'analyse et de l'application de la GPO.

**Conseils**

* Nommez vos GPO de manière descriptive afin de pouvoir les identifier facilement.
* Créez des GPO distinctes pour différents domaines, OU et groupes d'utilisateurs.
* Utilisez l'onglet **Analyse** pour valider vos GPO avant de les propager.
* Consultez la documentation officielle des stratégies de groupe pour plus d'informations.
