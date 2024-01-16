---
date: 2024-01-16
---


# Principales Classes dans Active Directory

**Utilisateur (user) :**

- Représente un compte utilisateur dans Active Directory. Contient des informations telles que le nom d'utilisateur, le mot de passe et d'autres attributs liés à l'utilisateur.

**Groupe (group) :**

- Un groupe est une collection d'utilisateurs et d'autres groupes. Il simplifie la gestion des autorisations et des droits en permettant d'appliquer des permissions à plusieurs utilisateurs simultanément.

**Ordinateur (computer) :**

- Représente un ordinateur ou un périphérique connecté au domaine Active Directory. Les ordinateurs rejoignent le domaine pour bénéficier de fonctionnalités centralisées et d'une gestion simplifiée.

**Imprimante (printer) :**

- Représente une imprimante partagée sur le réseau. Les utilisateurs peuvent se connecter à des imprimantes partagées via Active Directory pour simplifier l'impression.

**Contact (contact) :**

- Utilisé pour représenter des contacts externes à l'organisation, tels que des partenaires commerciaux ou des clients. Les contacts peuvent être associés à des utilisateurs internes.

**Unité d'Organisation (organizationalUnit) :**

- Une Unité d'Organisation (OU) est une unité logique utilisée pour organiser et hiérarchiser les objets dans Active Directory. Elle simplifie la gestion en permettant une structuration personnalisée.

**Contrôleur de Domaine (domainController) :**

- Représente un serveur sur lequel s'exécute le service Active Directory Domain Services (AD DS). Les contrôleurs de domaine stockent la base de données AD et fournissent des services d'authentification.

**Site (site) :**

- Un site représente un ou plusieurs réseaux IP bien connectés. Il est utilisé pour optimiser la réplication des données entre les contrôleurs de domaine et pour définir des politiques de réplication.

**Stratégie de Groupe (groupPolicyContainer) :**

- Contient les paramètres de stratégie de groupe qui peuvent être appliqués à des utilisateurs, des ordinateurs ou des groupes. Les stratégies de groupe permettent de définir des configurations et des restrictions.

**Boîte aux Lettres (mailbox) :**

- Dans le contexte de Microsoft Exchange Server intégré à Active Directory, la classe boîte aux lettres représente la boîte de réception électronique associée à un utilisateur.

**Partage (share) :**

- Représente un partage de fichier ou de dossier sur le réseau. Les partages simplifient l'accès aux ressources partagées au sein de l'environnement AD.

**Objet de Configuration (configuration) :**

- Contient des informations de configuration globale pour l'ensemble de l'infrastructure AD, y compris des détails sur les sites, les domaines et les partitions d'annuaire.

Ces classes représentent une sélection des principales entités dans Active Directory. Chaque classe joue un rôle spécifique dans l'organisation, la gestion et la configuration de l'environnement réseau au sein d'un domaine Windows.