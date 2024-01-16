---
date: 2024-01-16
---
# Niveau Fonctionnel dans Active Directory
Le niveau fonctionnel dans Active Directory (AD) représente le niveau de fonctionnalités pris en charge par un environnement AD, déterminant ainsi les fonctionnalités disponibles pour les domaines et les forêts. Voici une explication détaillée de cette notion :

## **Niveaux Fonctionnels :**

Active Directory prend en charge différents niveaux fonctionnels pour les domaines et les forêts. Ces niveaux déterminent les fonctionnalités spécifiques et les capacités de l'environnement AD. Les niveaux fonctionnels disponibles dépendent de la version du système d'exploitation des contrôleurs de domaine.

### **Niveau Fonctionnel du Domaine :**

Le niveau fonctionnel du domaine peut être relevé pour tirer parti des fonctionnalités spécifiques. Les niveaux fonctionnels du domaine incluent :

1. **Windows 2000 Native :**
    
    - Prise en charge des contrôleurs de domaine Windows 2000.
    - Limitations sur certaines fonctionnalités avancées.
2. **Windows Server 2003 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2003.
    - Améliorations de la réplication et de la gestion.
3. **Windows Server 2008 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2008.
    - Intégration de la stratégie de groupe améliorée et d'autres améliorations.
4. **Windows Server 2008 R2 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2008 R2.
    - Améliorations de la virtualisation, de PowerShell, etc.
5. **Windows Server 2012 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2012.
    - Intégration du Cloud, améliorations de la sécurité, etc.
6. **Windows Server 2012 R2 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2012 R2.
    - Améliorations de la gestion des appareils mobiles, etc.
7. **Windows Server 2016 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2016.
    - Améliorations de la sécurité, de la virtualisation, etc.
8. **Windows Server 2019 :**
    
    - Prise en charge des fonctionnalités de Windows Server 2019.
    - Dernier niveau fonctionnel disponible à la date de ma connaissance (janvier 2022).

### **Niveau Fonctionnel de la Forêt :**

Le niveau fonctionnel de la forêt est déterminé par le niveau fonctionnel du domaine le plus bas dans la forêt. Tous les domaines de la forêt doivent être élevés au niveau fonctionnel du domaine le plus élevé pour utiliser toutes les fonctionnalités disponibles.

## **Élévation du Niveau Fonctionnel :**

Élever le niveau fonctionnel se fait en mettant à niveau tous les contrôleurs de domaine d'un domaine ou d'une forêt vers la version minimale requise pour le niveau fonctionnel souhaité. Cela peut être réalisé en ajoutant et en promouvant de nouveaux contrôleurs de domaine avec des versions de système d'exploitation plus récentes et en retirant progressivement les anciens.

## **Impact sur les Fonctionnalités :**

L'élévation du niveau fonctionnel permet d'accéder à de nouvelles fonctionnalités, mais il est important de noter que cela peut rendre difficile ou impossible le retour à un niveau fonctionnel inférieur. Il est donc crucial de comprendre les implications avant d'élever le niveau fonctionnel.

En résumé, le niveau fonctionnel dans Active Directory détermine les fonctionnalités et les capacités disponibles pour les domaines et les forêts. Élever le niveau fonctionnel permet de tirer parti des dernières améliorations et fonctionnalités offertes par les versions récentes de Windows Server.