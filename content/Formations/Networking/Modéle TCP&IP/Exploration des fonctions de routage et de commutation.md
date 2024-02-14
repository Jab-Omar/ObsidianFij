---
date: 14-02-2024
Time: 23:08
---
## Routage

Le routage consiste à déterminer le meilleur chemin pour acheminer les données d'un point à un autre à travers un réseau. Voici les principaux aspects du routage :

1. **Principe :** Le routage utilise des tables de routage configurées sur les routeurs pour déterminer la meilleure route à prendre pour acheminer les données. Ces tables de routage sont basées sur des algorithmes de routage qui prennent en compte des facteurs tels que la distance, la bande passante, la charge du réseau et d'autres métriques pour choisir le chemin optimal.
    
2. **Types de routage :**
    
    - Routage statique : Les routes sont configurées manuellement par l'administrateur réseau.
    - Routage dynamique : Les routes sont apprises automatiquement par les routeurs en échangeant des informations de routage avec d'autres routeurs via des protocoles de routage tels que OSPF (Open Shortest Path First) ou BGP (Border Gateway Protocol).
3. **Hiérarchie de routage :** Les réseaux sont généralement organisés en hiérarchies de routage, avec des réseaux locaux connectés à des réseaux régionaux, qui sont ensuite connectés à des réseaux nationaux et internationaux. Cette hiérarchie facilite la gestion et le contrôle du trafic sur le réseau.
    
4. **Redondance et tolérance aux pannes :** Le routage peut également être utilisé pour fournir une redondance et une tolérance aux pannes en configurant plusieurs chemins de secours pour acheminer les données en cas de panne d'un lien ou d'un périphérique.
    

## Commutation

La commutation consiste à transférer les données d'un port d'entrée à un port de sortie sur un commutateur réseau. Voici les principaux aspects de la commutation :

1. **Principe :** Les commutateurs utilisent des tables de commutation pour déterminer le port de sortie approprié pour acheminer les trames de données. Ces tables sont remplies par l'apprentissage des adresses MAC des périphériques connectés à chaque port.
    
2. **Types de commutation :**
    
    - Commutation de couche 2 (commutation MAC) : Les trames sont transférées en fonction des adresses MAC des périphériques.
    - Commutation de couche 3 (commutation IP) : Les paquets sont transférés en fonction des adresses IP des périphériques.
3. **Apprentissage des adresses :** Les commutateurs apprennent les adresses MAC des périphériques en observant le trafic sur chaque port. Ils construisent ainsi une table de correspondance entre les adresses MAC et les ports de sortie.
    
4. **Routage versus commutation :** Les commutateurs sont généralement utilisés pour acheminer le trafic au sein d'un réseau local, tandis que les routeurs sont utilisés pour acheminer le trafic entre des réseaux différents. Les routeurs opèrent à des niveaux plus élevés du modèle OSI et prennent en compte des informations telles que les adresses IP, tandis que les commutateurs opèrent au niveau de la couche liaison de données et utilisent les adresses MAC pour acheminer le trafic.
    

En résumé, le routage et la commutation sont deux fonctions fondamentales dans les réseaux informatiques, permettant le transfert efficace et fiable des données à travers le réseau. Leur compréhension est essentielle pour concevoir, déployer et gérer des réseaux informatiques performants.