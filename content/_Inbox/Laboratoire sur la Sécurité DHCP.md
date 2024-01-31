---
date: 31-01-2024
Time: 23:43
---
# Laboratoire sur la Sécurité DHCP

## Objectif du Laboratoire
Ce laboratoire a pour objectif de renforcer la sécurité du service DHCP en activant l'authentification DHCP et en configurant le filtrage des adresses MAC. Nous allons également effectuer des tests pour vérifier que seuls les périphériques autorisés peuvent obtenir une adresse IP.

## Prérequis
- Un serveur DHCP configuré et fonctionnel.
- Liste des adresses MAC des périphériques autorisés.
- Accès administratif au serveur DHCP.

## Étapes du Laboratoire

### Étape 1: Activation de l'Authentification DHCP
1. Ouvrez le Gestionnaire DHCP sur le serveur.
2. Cliquez avec le bouton droit sur le nom du serveur dans l'arborescence et sélectionnez "Propriétés".
3. Allez dans l'onglet "Authentification" et cochez l'option "Activer l'authentification DHCP".
4. Configurez les options d'authentification selon vos besoins (par exemple, utilisez "Protocole de base" pour commencer).

### Étape 2: Configuration du Filtrage des Adresses MAC
1. Dans le Gestionnaire DHCP, sélectionnez la portée d'adresses IP que vous souhaitez filtrer.
2. Cliquez avec le bouton droit et choisissez "Filtrage des adresses MAC".
3. Ajoutez les adresses MAC des périphériques autorisés à la liste.

### Étape 3: Tests de Sécurité
1. Connectez un périphérique non autorisé au réseau.
2. Observez s'il obtient une adresse IP en utilisant la commande `ipconfig /renew`.
   - Si l'authentification DHCP est correctement configurée, le périphérique non autorisé ne devrait pas obtenir d'adresse IP.
   - Si le filtrage des adresses MAC est correctement configuré, le serveur DHCP ne devrait pas attribuer d'adresse IP au périphérique non autorisé.

### Étape 4: Tests de Périphériques Autorisés
1. Connectez un périphérique autorisé au réseau.
2. Vérifiez que le périphérique obtient correctement une adresse IP en utilisant la commande `ipconfig /renew`.
   - Le périphérique autorisé devrait recevoir une adresse IP valide.

### Étape 5: Affinement de la Configuration
1. Explorez les options d'authentification DHCP pour des configurations plus avancées.
2. Ajoutez ou supprimez des adresses MAC de la liste de filtrage en fonction des besoins.

## Points à Noter
- L'activation de l'authentification DHCP et la configuration du filtrage des adresses MAC peuvent varier en fonction du serveur DHCP utilisé.
- Assurez-vous que les adresses MAC dans la liste de filtrage correspondent aux périphériques autorisés.
- Lors de la configuration avancée de l'authentification DHCP, assurez-vous que les clients sont également configurés pour l'authentification.

Ce laboratoire vise à renforcer la sécurité du service DHCP en s'assurant que seuls les périphériques autorisés peuvent obtenir une adresse IP. La combinaison de l'authentification DHCP et du filtrage des adresses MAC contribue à prévenir l'accès non autorisé au réseau.