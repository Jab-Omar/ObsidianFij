---
date: 2023-10-30
---

PowerShell est un puissant outil de gestion en ligne de commande dans Windows, et il offre une variété de commandes pour gérer les services Windows. Vous pouvez utiliser PowerShell pour démarrer, arrêter, suspendre, reprendre, configurer, obtenir des informations et gérer les dépendances entre les services. Voici comment ajouter et supprimer des dépendances entre les services :

## Afficher la Liste des Services

Pour afficher la liste des services sur votre système, utilisez la commande `Get-Service` :

```powershell
Get-Service
```

Cela affichera une liste de tous les services, y compris leur nom, leur état actuel et leur mode de démarrage.

## Démarrer un Service

Pour démarrer un service spécifique, utilisez la commande `Start-Service` en spécifiant le nom du service :

```powershell
Start-Service -Name "NomDuService"
```

Remplacez "NomDuService" par le nom du service que vous souhaitez démarrer.

## Arrêter un Service

Pour arrêter un service, utilisez la commande `Stop-Service` :

```powershell
Stop-Service -Name "NomDuService"
```

Remplacez "NomDuService" par le nom du service que vous souhaitez arrêter.

## Mettre en Pause et Reprendre un Service

Pour mettre en pause un service, utilisez la commande `Suspend-Service` :

```powershell
Suspend-Service -Name "NomDuService"
```

Pour reprendre un service en pause, utilisez la commande `Resume-Service` :

```powershell
Resume-Service -Name "NomDuService"
```

## Obtenir des Informations sur un Service

Pour obtenir des informations détaillées sur un service spécifique, utilisez la commande `Get-Service` avec le nom du service :

```powershell
Get-Service -Name "NomDuService" | Format-List *
```

Cela affichera des informations telles que le nom du service, l'état actuel, le mode de démarrage, le type de démarrage, le chemin du fichier exécutable, etc.

## Modifier le Mode de Démarrage d'un Service

Pour modifier le mode de démarrage d'un service (par exemple, le configurer pour démarrer automatiquement ou manuellement), utilisez la commande `Set-Service` :

```powershell
Set-Service -Name "NomDuService" -StartupType "Automatique"
```

Remplacez "NomDuService" par le nom du service et "Automatique" par le mode de démarrage souhaité.

## Ajouter des Dépendances entre les Services

Pour ajouter des dépendances entre les services, utilisez la commande `sc.exe` avec l'option `config` :

```powershell
sc.exe config "NomDuService" depend= "Service1/Service2"
```

Remplacez "NomDuService" par le nom du service auquel vous souhaitez ajouter des dépendances, "Service1" et "Service2" par les noms des services auxquels il doit être dépendant. Vous pouvez spécifier plusieurs services en les séparant par des barres obliques.

## Supprimer des Dépendances entre les Services

Pour supprimer des dépendances entre les services, utilisez à nouveau la commande `sc.exe` avec l'option `config` :

```powershell
sc.exe config "NomDuService" depend= ""
```

Cela supprimera toutes les dépendances du service spécifié.

Ces commandes vous permettront de gérer efficacement les dépendances entre les services Windows à l'aide de PowerShell. N'oubliez pas d'exécuter PowerShell en tant qu'administrateur pour effectuer des opérations de gestion de services.
