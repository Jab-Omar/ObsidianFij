---
date: 18-02-2024
Time: 00:55
---
# Les Protocol Data Unit (PDU)

Les Protocol Data Unit (PDU) sont des entités de données utilisées dans les communications réseau pour encapsuler et transporter des informations entre les couches du modèle OSI (Open Systems Interconnection) ou du modèle TCP/IP. Chaque couche du modèle réseau a son propre PDU.

## Modèle OSI:

1. **Couche Physique (1)**:
    
    - PDU: Bits
    - Description: Les bits sont les unités de données de la couche physique. Ils représentent des signaux électriques, lumineux ou radioélectriques physiques sur le support de transmission.
2. **Couche Liaison de Données (2)**:
    
    - PDU: Trame
    - Description: Les trames sont des paquets de données structurées qui incluent des en-têtes et des pieds de trame, ainsi que les données elles-mêmes. Elles sont utilisées pour délimiter les données et identifier les adresses physiques.
3. **Couche Réseau (3)**:
    
    - PDU: Paquet
    - Description: Les paquets sont des unités de données qui contiennent des informations de routage, telles que les adresses IP source et destination, ainsi que les données à transmettre. Ils sont utilisés pour transporter des données entre des hôtes sur des réseaux différents.
4. **Couche Transport (4)**:
    
    - PDU: Segment (TCP) ou Datagramme (UDP)
    - Description: Les segments (pour TCP) et les datagrammes (pour UDP) sont des unités de données qui encapsulent les données de la couche application, ainsi que des informations de contrôle de flux, de séquençage et de vérification d'erreurs.
5. **Couche Session (5)**, **Couche Présentation (6)**, et **Couche Application (7)**:
    
    - PDU: Données
    - Description: Les données, au niveau de ces couches, sont les informations fournies par l'application, telles que le texte, les images, les fichiers, etc. Ces données sont encapsulées dans les PDUs des couches inférieures pour être transmises sur le réseau.

## Modèle TCP/IP:

1. **Couche Accès au Réseau (ou Interface Réseau) (1)**:
    
    - PDU: Trame
    - Description: Similaire à la couche Liaison de Données du modèle OSI, cette couche utilise des trames pour transporter des données entre les dispositifs sur le même réseau physique.
2. **Couche Internet (2)**:
    
    - PDU: Paquet
    - Description: Correspondant à la couche Réseau du modèle OSI, cette couche utilise des paquets pour acheminer des données entre différents réseaux IP.
3. **Couche Transport (3)**:
    
    - PDU: Segment (TCP) ou Datagramme (UDP)
    - Description: Équivalent à la couche Transport du modèle OSI, cette couche segmente les données provenant de la couche application en segments (pour TCP) ou datagrammes (pour UDP) pour le transport sur le réseau.
4. **Couche Application (4)**:
    
    - PDU: Message
    - Description: Les messages sont les données brutes de l'application. Ils sont encapsulés dans les PDUs des couches inférieures et sont finalement délivrés à l'application de destination.

Les PDU jouent un rôle crucial dans le processus de communication réseau en encapsulant, transportant et délivrant les données entre les différentes couches du modèle OSI ou TCP/IP. Chaque type de PDU est conçu pour répondre aux besoins spécifiques de sa couche respective, assurant ainsi un fonctionnement fluide et efficace du réseau.