---
tags:
  - Windows
date: 2023-10-30
---
# Gestion des liens de GPO

Les liens de GPO vous permettent d'appliquer les paramètres d'une GPO à un domaine, une unité d'organisation (OU) ou un groupe d'utilisateurs.

**Lien d'une GPO**

Pour lier une GPO, procédez comme suit :

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur le domaine, l'OU ou le groupe d'utilisateurs auquel vous souhaitez lier la GPO.
3. Dans le menu contextuel, cliquez sur **Lien d'un objet de stratégie de groupe**.
4. Dans la boîte de dialogue **Sélectionnez des objets**, sélectionnez la GPO que vous souhaitez lier.
5. Cliquez sur **OK**.

**Désactivation d'un lien de GPO**

Pour désactiver un lien de GPO, procédez comme suit :

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur le lien de GPO que vous souhaitez désactiver.
3. Dans le menu contextuel, cliquez sur **Désactiver**.

**Suppression d'un lien de GPO**

Pour supprimer un lien de GPO, procédez comme suit :

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur le lien de GPO que vous souhaitez supprimer.
3. Dans le menu contextuel, cliquez sur **Supprimer**.

**Exemple**

Supposons que vous souhaitez appliquer les paramètres de sécurité d'une GPO à tous les utilisateurs de votre domaine. Pour ce faire, vous devez lier la GPO à votre domaine.

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur votre domaine.
3. Dans le menu contextuel, cliquez sur **Lien d'un objet de stratégie de groupe**.
4. Dans la boîte de dialogue **Sélectionnez des objets**, sélectionnez la GPO que vous souhaitez lier.
5. Cliquez sur **OK**.

Une fois que vous avez lié la GPO, les paramètres de sécurité seront appliqués à tous les utilisateurs de votre domaine.
