---
date: 25-02-2024
Time: 14:39
---
Bien sûr ! Voici un exercice où vous allez écrire un fichier JSON pour représenter une liste de tâches à faire (todo list) :

## Exercice : Création d'une liste de tâches en JSON

Imaginez que vous êtes en train de développer une application de gestion de tâches à faire. Votre tâche est de créer un fichier JSON qui représente une liste de tâches à faire pour un utilisateur. Chaque tâche doit contenir un titre, une description, une date de création et un état (terminée ou non terminée).

### Instructions :

1. Créez un fichier JSON nommé `tasks.json`.
2. Remplissez le fichier JSON avec une liste de tâches à faire. Chaque tâche doit contenir les champs suivants :
   - "title" : Le titre de la tâche.
   - "description" : Une description de la tâche.
   - "created_at" : La date de création de la tâche.
   - "completed" : Un booléen indiquant si la tâche est terminée ou non (true pour terminée, false pour non terminée).
3. Ajoutez au moins 3 tâches à la liste.

### Exemple de structure JSON à remplir :

```json
[
  {
    "title": "Faire les courses",
    "description": "Acheter des fruits, du lait et du pain.",
    "created_at": "2024-02-25",
    "completed": false
  },
  {
    "title": "Répondre aux e-mails",
    "description": "Répondre aux e-mails des clients et des collègues.",
    "created_at": "2024-02-25",
    "completed": false
  },
  {
    "title": "Préparer la présentation",
    "description": "Finaliser la présentation pour la réunion de demain.",
    "created_at": "2024-02-24",
    "completed": true
  }
]
```

### Consignes supplémentaires :

- Assurez-vous que le fichier JSON est bien formé, avec la syntaxe correcte.
- Choisissez des titres et des descriptions pertinents pour chaque tâche.
- Utilisez des dates de création réalistes (aujourd'hui ou hier, par exemple).
- Indiquez si une tâche est terminée ou non en ajustant la valeur du champ "completed".

### Réalisation :

Une fois que vous avez rempli votre fichier JSON avec la liste de tâches à faire, vous pouvez vérifier sa validité en utilisant un validateur JSON en ligne ou en lisant le fichier à l'aide d'un script Python pour vous assurer qu'il est correctement structuré.

Bon exercice !