---
date: 14-02-2024
Time: 23:46
---
## Segmentation des données avec TCP :

1. **Connexion orientée :** TCP est un protocole orienté connexion, ce qui signifie qu'il établit d'abord une connexion entre l'émetteur et le récepteur avant de transmettre des données. Cette connexion permet une communication bidirectionnelle fiable.
    
2. **Segmentation :** TCP segmente les données de la couche application en unités plus petites appelées segments. La taille des segments peut varier en fonction des paramètres de la connexion TCP et des caractéristiques du réseau, mais elle est généralement adaptée aux capacités du réseau pour éviter la fragmentation excessive.
    
3. **Numéros de séquence :** Chaque segment TCP est associé à un numéro de séquence unique, qui est utilisé pour ordonner les segments à l'arrivée et pour détecter et corriger les pertes de segments ou les duplications.
    
4. **Acquittements :** Le récepteur envoie des acquittements (ACK) pour confirmer la réception des segments. Si un segment n'est pas reçu correctement, le récepteur demande une retransmission en envoyant un accusé de réception sélectif (SACK) ou en utilisant le mécanisme de retransmission de TCP.
    
5. **Contrôle de flux et de congestion :** TCP utilise des mécanismes de contrôle de flux et de contrôle de congestion pour réguler la vitesse de transmission des données. Cela inclut l'utilisation de fenêtres de réception pour contrôler le flux de données et de mécanismes de contrôle de congestion pour éviter la congestion du réseau.
    

## Segmentation des données avec UDP :

1. **Sans connexion :** Contrairement à TCP, UDP est un protocole sans connexion, ce qui signifie qu'il n'établit pas de connexion avant de transmettre des données. Il envoie simplement les données sans garantir leur réception ou leur ordre.
    
2. **Datagrammes :** UDP ne segmente pas les données en unités plus petites comme le fait TCP. Au lieu de cela, il utilise des datagrammes, qui sont des paquets de données individuels envoyés de manière indépendante. Les datagrammes UDP peuvent être de taille fixe ou variable.
    
3. **Pas de contrôle de flux ni de congestion :** Contrairement à TCP, UDP ne fournit pas de mécanismes de contrôle de flux ou de contrôle de congestion. Cela signifie que UDP peut transmettre des données à la vitesse maximale possible, sans tenir compte des limitations du réseau.
    
4. **Pas de garantie de livraison :** Comme UDP n'utilise pas de mécanismes de contrôle de flux, de contrôle de congestion ou de retransmission, il ne garantit pas la livraison des données. Les datagrammes UDP peuvent être perdus, dupliqués ou reçus dans un ordre différent de celui dans lequel ils ont été envoyés.
    

En résumé, TCP et UDP utilisent des approches différentes pour la segmentation des données dans la couche transport. TCP segmente les données en unités plus petites avec une garantie de livraison et un contrôle de flux, tandis qu'UDP envoie des datagrammes sans connexion ni garantie de livraison. Le choix entre TCP et UDP dépend des besoins spécifiques de l'application et des exigences de performance du réseau.