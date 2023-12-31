---
date: 2023-11-14
---
# Proxy et Proxy Transparent

En milieu professionnel, l'utilisation d'un serveur proxy est fréquente, souvent dédié au filtrage Web pour sécuriser la navigation sur Internet des utilisateurs, particulièrement dans les établissements scolaires. Cela permet, par exemple, de restreindre l'accès à des sites à contenu inapproprié.

## 1. Proxy Classique

Un serveur proxy classique nécessite une configuration explicite sur le poste client. Ce dernier doit être paramétré pour utiliser le proxy lors de l'envoi de requêtes, plutôt que de contacter directement l'hôte distant. En l'absence de configuration, la requête est directement transmise au serveur distant, contournant ainsi le proxy.

Il existe plusieurs façons d'intégrer un serveur proxy dans une infrastructure, notamment en le positionnant dans une DMZ. Les postes clients contactent alors le serveur proxy isolé, qui se connecte à Internet à leur place. Dans certains cas, la fonction de proxy est assurée directement par le pare-feu, éliminant ainsi la nécessité d'une DMZ.

## 2. Proxy Transparent

Le proxy transparent, également appelé proxy implicite, ne requiert aucune configuration explicite sur le poste client. Ce dernier utilise le proxy comme passerelle sans en avoir conscience, facilitant ainsi le filtrage du trafic émis par les postes clients.

Dans ce scénario, la fonction de pare-feu et de serveur proxy transparent sont souvent regroupées sur un même serveur ou équipement. Il est possible de positionner le serveur proxy transparent sous le pare-feu, permettant ainsi le relais des trames entre le proxy et le pare-feu. Cette configuration est considérée comme idéale pour filtrer le trafic émis par les postes clients de manière transparente.