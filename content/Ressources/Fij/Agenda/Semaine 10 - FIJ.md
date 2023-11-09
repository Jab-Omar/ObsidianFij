---
tags:
  - fij
date: 2023-11-06
---
---
## Lundi 06/11/2023

##### Emploi
- Les compétences.
- Savoir ; savoir-faire ; savoir-être.
- Hard skills vs soft skills
- Ikigai
- MBTI (nous avons passé le test)
- Les valeurs
- Devoirs :
  - Faire le test modèle de Schwartz : psychomedia.qc.ca
  - Lire le fichier de compétences (S4 annexe)
  - Connaître ses 4 lettres MBTI.
  - Pas obligatoire : Lire le "Happiness Center" de l'université de Pennsylvanie.
##### Windows
- Les tâches planifiées (Task Scheduler)
- Laboratoire sur les tâches planifiées
- Exercice bonus :
  - Création d'un script restart.bat
  - Trouver le code pour redémarrer le PC via CMD.
  - L'intégrer dans le script.
  - Tâche planifiée qui lance ce script chaque vendredi à 17h sur le secteur.
##### Anglais
- Correction de l'évaluation formative.
- Théorie sur le futur simple.
- Les compléments de temps.
- Règle : Dans une subordonnée de temps, jamais le futur mais le présent.
- Construction de 3 phrases en anglais au futur simple.
---
## Mardi 07/11/2023

##### Hardware
- Retour d'évalutaion.
- Tp installation windows + Pilotes(drivers)
	- Il faut être particulièrement attentif au pilotes pour le display.
##### Français
- Distinguer un fait, une opinion, un sentiment. 
	- Exercices en groupe.
	- Création de 5 phrases. 
##### Communication
- Arnaud est venu présenter l'Espacit, et introduire les 2 prochains cours de communication
- L'estime de soi.

---

## Mercredi 08/11/2023

##### Word
- Présentations
- Exercices sur La mise en forme des paragraphes et sur l'alignement.
- Exercices sur l'alignement des paragraphes.
- Exercice mise en forme d'un texte brut.
##### Outlook
- Exercice sur les protocoles : Trouver les numéros de ports + acronymes.
- Correction de l'exercice.
##### Mathématiques 
- La notation scientifique.
- La notation ingénieur.
- Théorie sur le calcul littéral. 

 ---
## Jeudi 09/11/2023
##### Outlook
- Théorie sur les protocoles HTTP, RPC, POP3, IMAP4.
- Configuration d'un client outlook en pop3s.
##### Français
- Explication de la visite d'entreprise et du rapport de visite.
- Exercice en groupe : réforme scolaire. 
##### Hardware

- Les puissances de 2 jusqu'à 1024 :
    - 2
    - 4
    - 8
    - 16
    - 32
    - 64
    - 128
    - 256
    - 512
    - 1024

**IP**

- **Adressage logique**
    
    - L'adresse IP est une adresse logique qui permet d'identifier un ordinateur sur un réseau. Elle est composée de 4 octets, soit 32 bits.
    - On peut modifier l'adresse IP d'un ordinateur.
- **Adressage physique**
    
    - L'adresse MAC est une adresse physique qui permet d'identifier de manière unique un périphérique réseau. Elle est composée de 6 octets, soit 48 bits.
    - L'adresse MAC est gravée sur le périphérique réseau et ne peut pas être modifiée.
- **ipconfig**
    
    - La commande `ipconfig` permet d'afficher les informations de configuration réseau d'un ordinateur.
    - Elle permet notamment d'afficher l'adresse IP et l'adresse MAC de l'ordinateur.
- **Types d'IP**
    
    - Il existe deux types d'adresses IP :
        - L'adresse IPv4 est le type d'adresse IP le plus courant. Elle est représentée sous forme décimale.
        - L'adresse IPv6 est un nouveau type d'adresse IP qui permet de résoudre le problème de saturation des adresses IPv4. Elle est représentée sous forme hexadécimale.

**Adresse IP sous forme binaire**

- Une adresse IPv4 est composée de 4 octets, soit 32 bits.
- Chaque octet est représenté par un nombre binaire de 8 bits.
- Par exemple, l'adresse IP `192.168.1.1` est représentée sous forme binaire par :

```
11000000 10101000 00000001 00000001
```

- Les valeurs décimales des octets de l'adresse IP `192.168.1.1` sont :

```
192 = 11000000 = 2^7 + 2^6 + 2^5 + 2^4 = 128 + 64 + 32 + 16 = 232
168 = 10101000 = 2^7 + 2^6 + 2^5 + 2^3 = 128 + 64 + 32 + 8 = 232
1 = 00000001 = 2^0 = 1
1 = 00000001 = 2^0 = 1
```

**Classes d'adresses IP**

- Les adresses IP sont divisées en classes, en fonction du premier octet de l'adresse.
- Il existe 5 classes d'adresses IP :
    - Classe A : le premier octet est compris entre 0 et 127.
    - Classe B : le premier octet est compris entre 128 et 191.
    - Classe C : le premier octet est compris entre 192 et 223.
    - Classe D : le premier octet est compris entre 224 et 239.
    - Classe E : le premier octet est compris entre 240 et 255.
- Les classes A, B et C sont utilisées pour les adresses publiques.
- Les classes D et E sont réservées pour des usages spécifiques.

**Le netmask**

- Le netmask est une valeur binaire qui permet de déterminer la partie réseau et la partie hôte d'une adresse IP.
- Par exemple, le netmask de la classe A est `255.0.0.0`.
- Cela signifie que les 32 premiers bits de l'adresse IP correspondent à la partie réseau et que les 8 derniers bits correspondent à la partie hôte.

**Adresses privées**

- Les adresses privées sont des adresses IP qui ne sont pas utilisées sur Internet.
- Elles sont utilisées pour les réseaux locaux.

---
- appendre par Coeur les puissance de 2 jusqu'à 1024
- Ip
	- Adressage logique : on peut la modifier (adresse Ip)
	- Adressage physique : On ne peut pas la modifier elle est gravé (MAC)
	- ipconfig : donne l'IP de la machine
	- Il y'as deux type d'IP v4 et v6. v4 est en décimal et la v6 est en hexadecimal.
- Adresse Ip sous forma binaire :
	- une adresse ipv4 = 32bits
	- soit 2\*\*32 et donc 4 octet.
	- soit 42.949.672.296 adresses possibles.
	- ABCD : chaque case 1octet (8bit) A = le premier octet
		- 192.168.256.5 ne peux être une adresse ip car la valeur décimale maximale et 255.
	Classes A B C D D'adresse Ip :
		- on a un probléme de saturation
		- Ip public donné par un ISP vs Ip privée pas ouvert à internet.
		- on prend le 1et octet si elle est entre 0 et 127 elle sera dans la classe a. etc......
		- Les classe D et E sont réservées
		- Le netmask associé ou sub netmask à developer 
		- adresse privée de 10.0.0.0 à 10.255.255.255 pour classe a
		-  pourquoi à ton ajouter le network ?
		- nom  de famille : 
		- on peut se trouver dans la même classe ça veut pas dire qu'on est dans le même réseau: 
		- comment trouve ton le nom d'un réseau
		- pas la même adresse réseau impossible de communiquer
		- adresse réseau et adresse hôte.

- Les adresses spécfiques :
	- il y'as des adresses ip reservées.
	- pour communiquer avec elle même la machine dispose de la boucle local 127.0.0.1. Pourquoi cette adresse est importante ?
	- c'est quoi l'adresse Apipa ? Pourquoi elle pose probléme ? Signale un probléme de dhcp ? Que sous windows ? 
	- Comment trouver l'adresse réseau ? grâce au netmask ?
	- c'est quoi l'adresse broadcast ? comment la trouver ?
	- combien de machine sont adressable au sein de ce réseau : 10.0.0.0 ? 2 puissance 24 moins2 ? pourquoi ? le moins deux correspond à quoi .
- Reconnaître une Ip à partir du binaire :
	- Comment reconnaître une ip à partir d'ubn binaire ? Des astuces ?
	- 