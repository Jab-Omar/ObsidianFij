---
date: 2023-11-09
---
Le routage est le processus qui permet de diriger les données d'un réseau à un autre, en choisissant le meilleur chemin possible à travers le réseau. Voici comment fonctionne le routage de manière générale :

## 1. **Détermination de la Destination :**
   - Lorsqu'un périphérique souhaite envoyer des données à un autre périphérique sur un réseau différent, il utilise une adresse IP de destination pour identifier le destinataire.

## 2. **Table de Routage :**
   - Chaque périphérique connecté à un réseau possède une table de routage. Cette table contient des informations sur les réseaux voisins et les chemins pour les atteindre.

## 3. **Masque de Sous-Réseau :**
   - Le masque de sous-réseau est utilisé pour déterminer à quel réseau appartient l'adresse IP de destination. Cela aide à filtrer la table de routage pour trouver le chemin approprié.

## 4. **Recherche du Chemin Optimal :**
   - La table de routage est consultée pour trouver le chemin optimal vers la destination. La meilleure correspondance est basée sur la combinaison de l'adresse IP de destination et du masque de sous-réseau.

## 5. **Routage Statique ou Dynamique :**
   - Le routage peut être statique, où les itinéraires sont configurés manuellement par l'administrateur, ou dynamique, où les routeurs échangent des informations pour déterminer les meilleurs itinéraires automatiquement.

### a. **Routage Statique :**
   - Les administrateurs définissent manuellement les itinéraires dans la table de routage. C'est courant dans les réseaux plus petits avec une topologie stable.

### b. **Routage Dynamique :**
   - Les protocoles de routage, tels que RIP, OSPF, ou BGP, sont utilisés pour permettre aux routeurs de partager des informations sur les itinéraires disponibles. Cela est souvent utilisé dans des réseaux plus importants et plus complexes.

## 6. **Transmission des Paquets :**
   - Une fois l'itinéraire déterminé, les paquets de données sont envoyés du périphérique source vers le périphérique destination à travers les routeurs et les réseaux intermédiaires.

## 7. **Routage Interne et Externe :**
   - Le routage interne concerne les itinéraires à l'intérieur d'un même système autonome, tandis que le routage externe concerne les itinéraires entre différents systèmes autonomes.

## 8. **Mise à Jour de la Table de Routage :**
   - Les tables de routage peuvent être mises à jour dynamiquement à mesure que la topologie du réseau change. Les routeurs échangent des informations pour s'adapter aux nouvelles conditions du réseau.

## 9. **Protocoles de Routage :**
   - Les protocoles de routage définissent comment les routeurs communiquent entre eux pour échanger des informations sur les itinéraires disponibles. Certains protocoles communs incluent OSPF, RIP, BGP, et EIGRP.

## Conclusion

Le routage est une fonction fondamentale des réseaux informatiques qui permet de diriger efficacement les données d'un point à un autre à travers un réseau. Il utilise des tables de routage, des itinéraires statiques ou dynamiques, des protocoles de routage, et adapte ses itinéraires en fonction de la topologie du réseau.