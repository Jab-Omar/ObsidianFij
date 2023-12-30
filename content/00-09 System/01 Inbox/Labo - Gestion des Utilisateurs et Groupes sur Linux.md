# Labo - Gestion des Utilisateurs et Groupes sur Linux
## Scénario : Gestion des Utilisateurs et Groupes pour une Entreprise en Expansion

Bienvenue dans ce laboratoire dédié à la gestion des utilisateurs et des groupes pour une entreprise fictive, "TechCo". En tant que technicien informatique débutant chez TechCo, tu es chargé de mettre en place et de gérer les comptes utilisateurs ainsi que les groupes pour les différents départements de l'entreprise.

---

## Exercices :

1. **Création d'Utilisateurs :**
    
    - Crée un utilisateur nommé "JohnDoe" avec le mot de passe "secure123".
    - Crée trois autres utilisateurs : "Alice", "Bob", et "Charlie", en leur attribuant des mots de passe sécurisés.
2. **Création de Groupes :**
    
    - Crée un groupe nommé "Marketing".
    - Crée un groupe nommé "Développement".
3. **Ajout et Suppression d'Utilisateurs dans des Groupes :**
    
    - Ajoute l'utilisateur "JohnDoe" au groupe "Marketing".
    - Ajoute "Alice", "Bob", et "Charlie" au groupe "Développement".
    - Supprime l'utilisateur "Charlie" du groupe "Développement".
4. **Suppression d'Utilisateurs et de Groupes :**
    
    - Supprime l'utilisateur "Alice".
    - Supprime le groupe "Marketing".
5. **Gestion des Mots de Passe :**
    
    - Change le mot de passe de l'utilisateur "Bob" pour un nouveau mot de passe sécurisé de ton choix.
6. **Connexion à des Comptes Utilisateurs :**
    
    - Connecte-toi au compte utilisateur "JohnDoe" depuis la ligne de commande.


---

## Pour t'aider

1. **Création d'Utilisateurs :**

   Pour créer un utilisateur nommé "JohnDoe" avec le mot de passe "secure123":
   ```bash
   sudo useradd JohnDoe                   # Crée l'utilisateur JohnDoe
   sudo passwd JohnDoe                    # Définit le mot de passe pour JohnDoe
   ```

   Pour créer les autres utilisateurs ("Alice", "Bob", et "Charlie") avec des mots de passe sécurisés, utilise la même structure de commandes que pour JohnDoe.

2. **Création de Groupes :**

   Pour créer un groupe nommé "Marketing":
   ```bash
   sudo groupadd Marketing                # Crée le groupe Marketing
   ```

   Crée un autre groupe nommé "Développement" en utilisant une structure similaire.

3. **Ajout et Suppression d'Utilisateurs dans des Groupes :**

   Pour ajouter un utilisateur à un groupe :
   ```bash
   sudo usermod -aG Marketing JohnDoe     # Ajoute JohnDoe au groupe Marketing
   sudo usermod -aG Développement Alice  # Ajoute Alice au groupe Développement
   ```

   Pour supprimer un utilisateur d'un groupe :
   ```bash
   sudo deluser Charlie Développement    # Supprime Charlie du groupe Développement
   ```

4. **Suppression d'Utilisateurs et de Groupes :**

   Pour supprimer un utilisateur :
   ```bash
   sudo userdel -r Alice                  # Supprime l'utilisateur Alice
   ```

   Pour supprimer un groupe :
   ```bash
   sudo groupdel Marketing                # Supprime le groupe Marketing
   ```

5. **Gestion des Mots de Passe :**

   Pour changer le mot de passe de l'utilisateur "Bob" :
   ```bash
   sudo passwd Bob                        # Change le mot de passe pour l'utilisateur Bob
   ```

6. **Connexion à des Comptes Utilisateurs :**

   Pour te connecter au compte utilisateur "JohnDoe" :
   ```bash
   su JohnDoe                             # Se connecte au compte JohnDoe
   ```

---

**Vérification :**

- Utilise ces commandes pour vérifier chaque action :
  - Pour vérifier l'existence des utilisateurs : `grep` dans `/etc/passwd`.
  - Pour vérifier l'appartenance aux groupes : `groups [utilisateur]`.
  - Pour vérifier la suppression : utilise `grep` pour rechercher dans les fichiers système si l'utilisateur ou le groupe existe toujours.

Chaque exercice te permettra de pratiquer différentes facettes de la gestion des utilisateurs et des groupes sous Linux. N'hésite pas à utiliser ces commandes pour vérifier que les actions ont été effectuées correctement !