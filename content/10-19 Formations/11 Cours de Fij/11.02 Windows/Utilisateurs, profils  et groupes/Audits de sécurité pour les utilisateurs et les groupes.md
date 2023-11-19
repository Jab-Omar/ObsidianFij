---
date: 2023-10-29
---

La sécurité des systèmes d'exploitation Windows repose en partie sur la capacité à surveiller les activités des utilisateurs et des groupes, ainsi que sur la capacité à détecter les comportements suspects. Les audits de sécurité sont des mécanismes clés pour atteindre ces objectifs.

## Audits de Connexion

Les audits de connexion permettent de suivre les tentatives de connexion, les réussites et les échecs. Ils peuvent révéler des activités suspectes ou des tentatives d'accès non autorisées.

Pour configurer les audits de connexion :

1. Accédez à la "Stratégie de sécurité locale" via "secpol.msc".
2. Naviguez jusqu'à "Stratégies de sécurité locale" > "Stratégie de sécurité locale" > "Stratégies d'audit" > "Auditer la réussite de la connexion" et "Auditer l'échec de la connexion".
3. Activez ces audits en conséquence.

## Audits d'Accès aux Fichiers et aux Objets

Les audits d'accès aux fichiers et aux objets permettent de suivre qui accède à quels fichiers et objets, ainsi que les actions effectuées (lecture, écriture, suppression, etc.). Cela peut aider à détecter les intrusions ou les comportements inappropriés.

Pour configurer les audits d'accès aux fichiers et aux objets :

1. Accédez aux "Propriétés de l'objet" (par exemple, un dossier ou un fichier).
2. Allez dans l'onglet "Sécurité" et cliquez sur "Avancé".
3. Naviguez jusqu'à l'onglet "Auditer" et configurez les autorisations d'audit pour les actions souhaitées.

## Audits des Modifications de Groupes

Les audits des modifications de groupes permettent de suivre les changements apportés aux groupes, tels que l'ajout ou la suppression d'utilisateurs. Cela aide à garantir la sécurité et la conformité.

Pour configurer les audits des modifications de groupes :

1. Accédez à la "Stratégie de sécurité locale" via "secpol.msc".
2. Naviguez jusqu'à "Stratégies de sécurité locale" > "Stratégie de sécurité locale" > "Stratégies d'audit" > "Auditer les modifications de membres de groupe".
3. Activez cet audit en conséquence.

## Suivi des Événements d'Audit

Une fois les audits configurés, les événements d'audit sont enregistrés dans le journal des événements Windows. Vous pouvez utiliser l'Observateur d'événements pour examiner ces journaux et rechercher des activités suspectes.

## Bonnes Pratiques

Pour des audits de sécurité efficaces :

- Définissez clairement les objectifs d'audit et les scénarios à surveiller.
- Effectuez régulièrement des audits pour détecter les anomalies.
- Documentez les procédures d'audit et les résultats.
- Éduquez les utilisateurs sur l'importance de la sécurité et des audits.

## Conclusion

Les audits de sécurité pour les utilisateurs et les groupes sont essentiels pour maintenir la sécurité et la conformité dans un environnement Windows. Ils permettent de détecter les comportements suspects, de surveiller les accès aux ressources et de garantir que seules les activités autorisées ont lieu. En suivant les bonnes pratiques d'audit, vous pouvez renforcer la sécurité de votre système.
