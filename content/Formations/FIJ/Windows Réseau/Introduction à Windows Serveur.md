# Intro à windows serveur

## C'est quoi windows serveur

Windows Server est un système d'exploitation conçu par Microsoft pour fonctionner sur des serveurs. Il offre un ensemble de fonctionnalités spécifiquement adaptées à la gestion des réseaux, des applications, du stockage de données et de la sécurité dans un environnement professionnel. Voici quelques points clés à savoir sur Windows Server :

-  **Gestion des serveurs et des ressources** : Windows Server permet de gérer plusieurs serveurs à partir d'une console centrale, offrant des outils pour administrer les ressources, surveiller les performances et configurer les rôles des serveurs.
    
-  **Services et rôles** : Il propose une gamme de services et de rôles, tels que Active Directory pour la gestion des identités et des accès, DNS pour la résolution de noms, DHCP pour l'attribution automatique des adresses IP, entre autres.
    
- **Sécurité** : Windows Server inclut des fonctionnalités de sécurité avancées telles que la gestion des stratégies de groupe, des pare-feu intégrés, des mécanismes d'authentification renforcés et des outils de surveillance des événements.
    
- **Stockage et virtualisation** : Il propose des fonctionnalités de stockage avancées comme le stockage dédupliqué, la gestion des espaces de stockage, ainsi que des capacités de virtualisation via Hyper-V pour exécuter des machines virtuelles.

-  **Versions spécialisées** : Il existe différentes versions de Windows Server adaptées à différents besoins, telles que Windows Server Standard, Datacenter, Essentials, et d'autres versions spécialisées pour des tâches spécifiques.

En somme, Windows Server est conçu pour fournir une plateforme solide et sécurisée pour gérer les réseaux d'entreprise, offrant des outils et des fonctionnalités spécifiquement adaptés aux besoins des serveurs.
## Versions avec et sans GUI
Le choix entre une installation avec ou sans interface graphique dépend des besoins spécifiques de l'environnement et des préférences de gestion. Le mode sans GUI offre une empreinte plus légère et une sécurité potentiellement renforcée, tandis que le mode avec GUI offre une expérience d'administration plus traditionnelle et conviviale pour certains utilisateurs.
### Windows Server sans GUI (Core) :
    
- Les versions Standard et Datacenter offrent une option d'installation sans interface utilisateur graphique, souvent appelée "Core" ou "Server Core".
- Cette version est axée sur une utilisation en ligne de commande et à distance, offrant une empreinte plus légère et moins de vulnérabilités potentielles liées à une surface d'attaque réduite.
- Elle est optimisée pour les charges de travail où une GUI n'est pas nécessaire, comme les serveurs d'infrastructure, les machines virtuelles ou les serveurs de domaine.
### Windows Server avec GUI :
    
- Les versions Standard et Datacenter proposent également une installation avec interface utilisateur graphique (Desktop Experience) pour ceux qui préfèrent une interface traditionnelle similaire à celle de Windows de bureau.
- Cette version est adaptée aux administrateurs ou utilisateurs qui sont plus à l'aise avec une interface graphique pour gérer et surveiller le serveur.
- Elle fournit un bureau, un gestionnaire de fichiers et une expérience utilisateur plus familière pour la configuration et la gestion du serveur.

## Versions Standard et Datacenter 
|Fonctionnalité|Standard|Datacenter|
|---|---|---|
|**Nombre de machines virtuelles (VMs) ou de conteneurs Hyper-V**|Permet d'exécuter jusqu'à 2 machines virtuelles ou conteneurs Hyper-V|Offre une licence pour exécuter autant de machines virtuelles ou de conteneurs Hyper-V que nécessaire, selon la capacité matérielle.|
|**Licences pour les conteneurs Windows**|Permet l'exécution de deux conteneurs Windows|Autorise l'exécution illimitée de conteneurs Windows|
|**Stockage Software Defined**|Inclus|Inclus|
|**Failover Clustering**|Disponible|Disponible|
|**Shielded Virtual Machines**|Disponible|Disponible|
|**Réseaux définis par logiciel (SDN)**|Pris en charge|Pris en charge|
|**Storage Spaces Direct**|Non inclus|Inclus, permet de construire des espaces de stockage partagés et hautement disponibles à partir des disques locaux.|
|**Réplica de stockage**|Non inclus|Inclus, permet la réplication des volumes de stockage entre serveurs.|

**En résumé**, si vous avez besoin de gérer beaucoup de machines virtuelles ou de conteneurs sur un seul serveur, des fonctionnalités avancées de stockage et de réplication, alors la version Datacenter est plus adaptée. La version Standard conviendrait davantage à des besoins plus modestes en virtualisation et en fonctionnalités avancées de stockage.