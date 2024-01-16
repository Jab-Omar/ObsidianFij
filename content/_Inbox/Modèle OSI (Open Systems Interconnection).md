---
date: 2024-01-17
---
  

---

# Modèle OSI (Open Systems Interconnection)

Le modèle OSI est un cadre de référence conceptuel utilisé pour concevoir des protocoles de communication réseau. Il divise le processus de communication en sept couches, chacune offrant des services spécifiques et interagissant avec les couches adjacentes. Voici une exploration détaillée de chaque couche du modèle OSI :

![[imgOSI.png]]
## **1. Couche Physique (1) :**

- Gère les aspects physiques de la transmission de données, tels que le câblage, les signaux électriques et les dispositifs matériels.

## **2. Couche Liaison de Données (2) :**

- Assure la communication directe entre des dispositifs sur un même réseau local. Gère la détection et la correction d'erreurs.

## **3. Couche Réseau (3) :**

- Responsable du routage des données entre différents réseaux. Utilise des adresses logiques pour diriger les paquets vers leur destination.

## **4. Couche Transport (4) :**

- Assure un flux de données fiable et efficace entre les applications sur des dispositifs différents. Gère le contrôle de flux, la segmentation des données et la correction d'erreurs.

## **5. Couche Session (5) :**

- Établit, maintient et termine les sessions de communication entre les applications sur des dispositifs différents. Gère la synchronisation entre les processus d'application.

## **6. Couche Présentation (6) :**

- Traite la représentation des données, leur encodage et leur compression. Assure une présentation compréhensible entre différentes applications.

## **7. Couche Application (7) :**

- Fournit une interface pour les applications réseau. Gère la communication entre les logiciels applicatifs, offrant des services tels que l'authentification, la gestion des sessions et la conversion de formats de données.

## **Points Importants :**

- Chaque couche offre des services à la couche supérieure et utilise les services de la couche inférieure, créant ainsi une architecture modulaire.
- La communication entre les couches se fait par le biais de protocoles standard, définissant les règles et le format des échanges d'informations.

## **Avantages du Modèle OSI :**

- Modularité : Permet le développement indépendant de chaque couche.
- Flexibilité : Peut être adapté à divers environnements réseau.
- Compréhension Conceptuelle : Facilite la compréhension des interactions entre les composants du réseau.

Bien que le modèle OSI serve de référence conceptuelle, dans la pratique, il est souvent utilisé comme guide plutôt que comme un modèle strictement suivi. Son importance réside dans sa capacité à fournir un cadre conceptuel pour la compréhension et la conception des systèmes de communication réseau.