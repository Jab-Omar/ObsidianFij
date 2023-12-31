---
date: 2023-11-20
---
# Cryptage de Partages

Le cryptage des partages sous Windows est une méthode essentielle pour sécuriser les données sensibles partagées sur un réseau. Voici comment crypter vos partages :

## Utilisation du Cryptage EFS (Encrypting File System)

1. **Sélectionnez le dossier à crypter** et faites un clic droit dessus.
2. Choisissez "Propriétés" et allez dans l'onglet "Général".
3. Cochez la case "Crypter le contenu pour sécuriser les données".
4. Appliquez les changements en suivant les instructions.

## Gestion des Clés de Cryptage

1. **Sauvegardez les clés de récupération** EFS pour accéder aux données en cas de problème avec les clés d'accès.
2. Assurez-vous que seuls les utilisateurs autorisés ont **accès aux clés de cryptage**.

## Surveillance et Maintenance

1. **Surveillez régulièrement** l'état du cryptage pour vous assurer qu'il est toujours actif.
2. Envisagez de **changer périodiquement les clés** pour renforcer la sécurité.

## Limitations du Cryptage

- Le cryptage EFS est spécifique à chaque fichier ou dossier crypté et ne s'applique pas à l'ensemble du partage.
- Il peut y avoir des problèmes d'accès aux fichiers cryptés si les clés sont perdues.

## Alternative: Utilisation de Logiciels de Cryptage Tierce-Partie

- Certains logiciels tiers offrent un **cryptage plus étendu** pour les partages complets, ajoutant une couche de protection supplémentaire.

Le cryptage des partages sous Windows avec EFS ou des outils tiers est crucial pour protéger les données confidentielles contre tout accès non autorisé, mais il est important de comprendre les limitations et de gérer soigneusement les clés de cryptage pour éviter toute perte d'accès.
