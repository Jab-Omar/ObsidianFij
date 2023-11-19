---
tags:
  - Windows
date: 2023-11-14
---
# Ports Utilisés par un Serveur Proxy

Les serveurs proxy ne sont pas associés à un port spécifique obligatoire, car le proxy lui-même n'est pas un protocole défini. Cependant, il est courant de rencontrer certains numéros de port, dont les plus répandus sont le 3128 et le 8080. Voici quelques explications sur ces choix de ports :

## 1. Port 3128
- **Association avec Squid :** Le port 3128 est souvent associé à Squid, l'un des serveurs proxy les plus populaires. Squid utilise le port 3128 par défaut pour écouter les connexions entrantes. La popularité de Squid a contribué à l'association fréquente du port 3128 avec la notion de proxy.

## 2. Port 8080
- **Utilisation Fréquente :** Le port 8080 est un autre port couramment utilisé pour les serveurs proxy. Bien que cela ne soit pas un standard, il est souvent choisi en raison de sa disponibilité et de sa simplicité d'utilisation. De nombreux serveurs proxy utilisent le port 8080 comme alternative au port 3128.

## Flexibilité : Port 80
- **Utilisation du Port 80 :** Il est tout à fait possible de monter un serveur proxy et d'utiliser le port 80 comme port d'écoute. Cette approche est parfois adoptée pour tirer parti de la familiarité et de la facilité d'accès associées au port 80, généralement utilisé pour le trafic HTTP.

En résumé, bien que le port 3128 soit souvent lié à Squid et que le port 8080 soit largement utilisé, il n'y a pas de restriction sur le choix du port pour un serveur proxy. L'utilisation du port 80 est également une option, offrant une flexibilité dans la configuration du proxy en fonction des besoins spécifiques de l'environnement et des préférences de l'administrateur système.