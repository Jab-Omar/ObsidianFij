---
tags:
  - Windows
date: 2023-10-30
---
# Filtrage de sécurité pour les GPO

Le filtrage de sécurité pour les GPO vous permet de limiter l'application des paramètres d'une GPO à un groupe spécifique d'utilisateurs ou d'ordinateurs.

**Filtre de sécurité**

Un filtre de sécurité est un ensemble de règles qui déterminent si une GPO s'applique à un objet. Les règles sont basées sur les propriétés de l'objet, telles que son nom, son groupe d'appartenance ou son emplacement.

**Création d'un filtre de sécurité**

Pour créer un filtre de sécurité, procédez comme suit :

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur la GPO à laquelle vous souhaitez appliquer le filtre.
3. Dans le menu contextuel, cliquez sur **Propriétés**.
4. Dans l'onglet **Filtrage de sécurité**, cliquez sur **Ajouter**.
5. Dans la boîte de dialogue **Sélectionnez des objets**, sélectionnez les objets auxquels vous souhaitez appliquer la GPO.
6. Cliquez sur **OK**.

**Exemple**

Supposons que vous souhaitez appliquer une GPO aux utilisateurs qui appartiennent au groupe "Administrateurs". Pour ce faire, vous devez créer un filtre de sécurité qui sélectionne tous les utilisateurs qui appartiennent au groupe "Administrateurs".

1. Ouvrez la console de gestion des stratégies de groupe (GPMC).
2. Dans l'arborescence de la console, cliquez avec le bouton droit sur la GPO à laquelle vous souhaitez appliquer le filtre.
3. Dans le menu contextuel, cliquez sur **Propriétés**.
4. Dans l'onglet **Filtrage de sécurité**, cliquez sur **Ajouter**.
5. Dans la boîte de dialogue **Sélectionnez des objets**, cliquez sur **Groupes**.
6. Dans la liste **Groupes**, sélectionnez le groupe "Administrateurs".
7. Cliquez sur **OK**.

Une fois que vous avez créé le filtre de sécurité, la GPO ne s'appliquera qu'aux utilisateurs qui appartiennent au groupe "Administrateurs".

**Conseils**

* Utilisez des filtres de sécurité pour limiter l'application des paramètres d'une GPO à un groupe spécifique d'utilisateurs ou d'ordinateurs.
* Créez des filtres de sécurité simples et faciles à comprendre.
* Testez vos filtres de sécurité avant de les mettre en production.
