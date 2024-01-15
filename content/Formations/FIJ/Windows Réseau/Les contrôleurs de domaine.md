---
date: 2024-01-15
---
# Les contrôleurs de domaine
Les contrôleurs de domaine (DC, pour Domain Controllers) jouent un rôle central dans les environnements utilisant le modèle de domaine, particulièrement dans le contexte de l'Active Directory (AD) de Microsoft. Voici une explication détaillée sur les contrôleurs de domaine :
## Définition :
Un contrôleur de domaine est un serveur exécutant le service Active Directory sur un réseau Windows. Il joue un rôle essentiel dans la gestion des comptes d'utilisateurs, des groupes, des politiques de sécurité, et fournit des services d'authentification et d'autorisation.
## Rôles et Fonctions :
### Stockage de l'Active Directory :
- Les contrôleurs de domaine stockent une copie de la base de données Active Directory, qui contient des informations sur les utilisateurs, les groupes, les ordinateurs, les politiques de groupe, etc.
### Authentification :
- Ils sont responsables de l'authentification des utilisateurs et des ordinateurs dans le domaine. Lorsqu'un utilisateur se connecte au réseau, le contrôleur de domaine vérifie les informations d'identification.
### Réplication :
- Les contrôleurs de domaine travaillent en réseau pour assurer la réplication des informations Active Directory. Cela garantit que chaque contrôleur de domaine dispose d'une copie à jour de la base de données.
### Émission de Tickets TGT :

- Lorsqu'un utilisateur se connecte, le contrôleur de domaine délivre un Ticket de Toute Première Session (TGT) qui est utilisé pour demander des tickets de service pour accéder à différentes ressources du réseau.
### Gestion des Politiques de Groupe :

- Les contrôleurs de domaine appliquent les politiques de groupe définies dans l'Active Directory, garantissant une configuration cohérente pour les utilisateurs et les ordinateurs du domaine.
## Types de Contrôleurs de Domaine :

### Contrôleur de Domaine Principal (PDC) :
- Historiquement, le PDC était crucial, mais dans les versions récentes de Windows Server, la fonction PDC est partagée entre plusieurs contrôleurs de domaine.
### Contrôleur de Domaine Secondaire :
- Contient une copie en lecture seule de la base de données Active Directory. Il peut être utilisé pour répartir la charge et améliorer la résilience du réseau.
### Contrôleur de Domaine Global Catalog (GC) :
- Contient des informations partielles sur tous les objets de l'AD dans l'ensemble de la forêt. Il facilite les recherches et les authentifications transforestières.
## Sécurité :
- Les contrôleurs de domaine sont des éléments critiques en termes de sécurité. Des mesures telles que la sauvegarde régulière, la sécurisation physique, et la protection des communications sont essentielles.

En résumé, les contrôleurs de domaine sont des composants clés dans les réseaux utilisant le modèle de domaine, offrant des services cruciaux pour la gestion des identités, l'authentification, la réplication des données, et la mise en œuvre des politiques de sécurité à l'échelle du réseau.