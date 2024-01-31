---
date: 31-01-2024
Time: 23:26
---
# Paramètres de Configuration DHCP

Les paramètres de configuration DHCP (Dynamic Host Configuration Protocol) sont des éléments essentiels définis par le serveur DHCP et attribués aux clients lors de l'attribution dynamique d'adresses IP. Voici une liste des paramètres de configuration couramment définis par le serveur DHCP :

**Paramètres Principaux :**
- **Adresse IP :**
   - L'adresse IP attribuée au client pour la durée de location spécifiée.
- **Masque de Sous-Réseau :**
   - Définit la portée du réseau en spécifiant le masque de sous-réseau à utiliser avec l'adresse IP attribuée.
- **Passerelle par Défaut (Gateway) :**
   - Indique l'adresse IP de la passerelle par défaut que le client doit utiliser pour accéder à des réseaux distants.
- **Serveur DNS Primaire et Secondaire :**
   - Fournit les adresses IP des serveurs DNS que le client doit utiliser pour la résolution des noms de domaine.
- **Serveur WINS (Windows Internet Naming Service) :**
   - Pour les environnements Windows, spécifie l'adresse IP du serveur WINS utilisé pour la résolution des noms NetBIOS.
- **Durée de Location (Lease Time) :**
   - Indique la période pendant laquelle l'adresse IP attribuée est valide. Le client doit renouveler ou demander une nouvelle adresse avant l'expiration de cette durée.

**Options de Configuration Supplémentaires :**
- **Domaine DNS :**
   - Spécifie le domaine DNS auquel le client appartient.
- **Serveur NTP (Network Time Protocol) :**
   - Fournit l'adresse IP du serveur NTP que le client peut utiliser pour synchroniser l'horloge.
- **Options de Routage :**
   - Pour des réseaux complexes, le serveur DHCP peut fournir des informations de routage pour permettre au client d'atteindre des réseaux distants.
- **Options Personnalisées :**
    - Le serveur DHCP peut être configuré pour inclure des options personnalisées en fonction des besoins spécifiques du réseau, telles que des configurations spéciales pour des services particuliers.

**Configuration de Plages d'Adresses IP :**
- **Plages d'Adresses IP :**
    - Définit les plages d'adresses IP disponibles pour attribution aux clients.
- **Sous-réseaux Supplémentaires :**
    - Pour les réseaux segmentés, le serveur DHCP peut être configuré avec des plages d'adresses IP spécifiques pour chaque sous-réseau.

La configuration précise de ces paramètres dépend des besoins spécifiques du réseau et de la politique de gestion des adresses IP. La personnalisation des paramètres DHCP contribue à assurer une connectivité réseau efficace et adaptée à l'environnement spécifique.