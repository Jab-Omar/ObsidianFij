## Introduction
MBR (Master Boot Record) et GPT (GUID Partition Table) sont deux méthodes de partitionnement de disque utilisées pour organiser et gérer les partitions sur un disque dur ou un SSD. Ils jouent un rôle crucial dans le démarrage du système d'exploitation et la gestion des données.

## MBR (Master Boot Record)

### Caractéristiques de MBR
- MBR est un ancien système de partitionnement qui utilise une structure de 512 octets située au début d'un disque dur. Il peut gérer jusqu'à quatre partitions primaires, ou trois partitions primaires et une partition étendue avec des sous-partitions logiques à l'intérieur de celle-ci.

### Limitations de MBR
- MBR présente certaines limitations, notamment :
  - Prise en charge limitée des disques de grande capacité (2 To ou moins).
  - Incapacité à gérer plus de quatre partitions principales (nécessité de créer des partitions étendues pour dépasser cette limite).
  - Manque de redondance et de tolérance aux pannes en cas de corruption du secteur de démarrage.

## GPT (GUID Partition Table)

### Caractéristiques de GPT
- GPT est une technologie de partitionnement plus récente et plus avancée. Il repose sur une structure de 512 octets ou plus (généralement 4 Ko) au début du disque. Il peut gérer un grand nombre de partitions (jusqu'à 128) et prend en charge les disques de grande capacité.

### Avantages de GPT
- GPT offre plusieurs avantages, notamment :
  - Prise en charge des disques de grande capacité (plus de 2 To).
  - Gestion de nombreuses partitions sans recourir à des partitions étendues.
  - Redondance intégrée pour résister à la corruption des données de partition.
  - Prise en charge de la technologie UEFI (Unified Extensible Firmware Interface) pour un démarrage sécurisé et rapide.

## Utilisations Courantes
- MBR a été largement utilisé dans le passé, mais il est désormais principalement utilisé sur les systèmes plus anciens ou avec des disques de petite capacité. GPT est de plus en plus courant, en particulier sur les systèmes modernes et les disques de grande capacité.

## Choix entre MBR et GPT
- Le choix entre MBR et GPT dépend des besoins du système et de la capacité du disque. Pour les disques de grande capacité et les systèmes modernes, GPT est généralement recommandé en raison de ses fonctionnalités avancées et de sa résilience.

## Conclusion
MBR et GPT sont deux méthodes de partitionnement de disque utilisées pour organiser et gérer les partitions de stockage. Alors que MBR est plus ancien et présente des limitations, GPT est une option moderne offrant une meilleure prise en charge des disques de grande capacité, une gestion avancée des partitions et une plus grande résilience. Le choix entre les deux dépend des besoins spécifiques du système et du matériel utilisé.
