---
date: 2023-11-14
---
# Reverse Proxy : Explication et Fonctionnement

À la différence du proxy, le reverse proxy opère dans le sens inverse en permettant aux utilisateurs externes d'accéder à des ressources du réseau interne. Lorsque vous accédez à une ressource protégée par un reverse proxy, c'est ce dernier que vous contactez. Il gère la requête en contactant le serveur cible à votre place, puis retourne la réponse. Les serveurs réels derrière le reverse proxy restent invisibles pour le client, créant ainsi une barrière de protection pour les serveurs internes et assurant une publication sécurisée des ressources.

## Utilisation Courante et Avantages

Un cas d'usage fréquent du reverse proxy est d'avoir plusieurs serveurs Web derrière lui. Il répartit la charge entre ces serveurs, assurant une utilisation efficace des ressources. En cas de panne d'un serveur, le reverse proxy redirige automatiquement les requêtes vers d'autres serveurs, offrant une continuité de service sans impact perceptible pour l'utilisateur. Voici une représentation schématique d'une infrastructure Web avec un reverse proxy intégré au pare-feu :


Si le serveur reverse proxy est indépendant, il peut être positionné en DMZ (zone démilitarisée). Dans ce scénario, les serveurs Web sont connectés au réseau local, et le reverse proxy agit comme intermédiaire pour les flux externes.

## Fonctionnalités du Reverse Proxy

Similaire à un proxy classique, le reverse proxy peut mettre en cache des ressources pour soulager les serveurs Web et améliorer les performances grâce à la compression des données. Par exemple, il peut mettre en cache des ressources statiques telles que des scripts JavaScript.

## Analogie avec les Jeux de Table

Pour illustrer le concept, on peut faire une analogie avec un croupier dans un casino. Le croupier, ou le reverse proxy, distribue les cartes (les connexions) aux joueurs (serveurs) autour de la table (réseau local) participant à la partie. Cette analogie suggère le rôle central du reverse proxy dans la distribution et la gestion des connexions.

En conclusion, le reverse proxy joue un rôle crucial dans la sécurisation et l'optimisation des accès aux ressources internes depuis l'extérieur. Son utilisation intelligente permet une gestion efficace de la charge, une haute disponibilité des services, et une protection accrue des serveurs internes contre les menaces potentielles.