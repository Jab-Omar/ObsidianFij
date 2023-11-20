---
date: 2023-10-29
---
# MBR (Master Boot Record) vs GPT (GUID Partition Table)

Le MBR (Master Boot Record) et le GPT (GUID Partition Table) sont deux schémas de partitionnement utilisés sur les disques durs. Chacun présente des caractéristiques distinctes et est adapté à des besoins spécifiques.

## MBR (Master Boot Record)

Le MBR est un schéma de partitionnement plus ancien qui a été utilisé sur les disques durs pendant de nombreuses années. Voici quelques caractéristiques du MBR :

- **Limitation de la taille des partitions** : Le MBR a une limitation de 2 To (téraoctets) pour la taille maximale de la partition.

- **Prise en charge des disques hérités** : Le MBR est compatible avec les systèmes d'exploitation plus anciens et les BIOS hérités.

- **Limite du nombre de partitions** : Le MBR est limité à quatre partitions principales. Pour contourner cette limite, des partitions logiques peuvent être utilisées.

- **Pas de redondance** : Le MBR ne possède pas de mécanismes de redondance intégrés, ce qui le rend plus vulnérable aux erreurs de corruption.

## GPT (GUID Partition Table)

Le GPT est un schéma de partitionnement plus récent qui a été introduit pour surmonter certaines limitations du MBR. Voici quelques caractéristiques du GPT :

- **Prise en charge des disques de grande capacité** : Le GPT prend en charge des disques durs de plus de 2 To sans limitation de taille.

- **Redondance** : Le GPT inclut une table de secours pour améliorer la tolérance aux pannes et la récupération des données en cas de corruption.

- **Pas de limitation du nombre de partitions** : Le GPT permet un grand nombre de partitions (plus de 128) sans avoir besoin de partitions logiques.

- **Prise en charge de l'UEFI** : Le GPT est recommandé pour les systèmes utilisant l'UEFI (Unified Extensible Firmware Interface), ce qui est de plus en plus courant.

Le choix entre le MBR et le GPT dépend des besoins spécifiques du système et de la capacité du matériel. Les nouveaux systèmes et disques durs de grande capacité optent souvent pour le GPT en raison de ses avantages. Cependant, il est important de noter que la conversion entre le MBR et le GPT peut entraîner la perte de données, il est donc essentiel de planifier à l'avance en fonction des besoins du système.
