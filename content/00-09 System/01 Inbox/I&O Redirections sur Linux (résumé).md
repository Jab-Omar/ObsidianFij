# Redirection d'E/S (Entrée/Sortie) sous Linux ou (Input/Output)

## Introduction
Les redirections d'E/S (Entrée/Sortie) sous Linux sont essentielles pour gérer le flux d'informations entre les commandes et les fichiers. Comprendre ces redirections permet de manipuler efficacement les flux de données dans le terminal.

## Flux Standards
### 1. Entrée Standard (stdin)
- Représente l'entrée depuis le clavier ou un fichier.
- Symbole : `<`

### 2. Sortie Standard (stdout)
- Représente la sortie normale d'une commande.
- Symboles : `>`, `>>`

### 3. Erreur Standard (stderr)
- Représente les messages d'erreur.
- Symbole : `2>`

## Redirections Basiques
- **`>`**: Redirige stdout vers un fichier, en écrasant le contenu existant.
  - Exemple : `commande > fichier.txt`

- **`>>`**: Ajoute stdout à un fichier.
  - Exemple : `commande >> fichier.txt`

- **`<`**: Prend une entrée depuis un fichier.
  - Exemple : `commande < fichier.txt`

## Redirections Spéciales
- **`2>`**: Redirige stderr vers un fichier.
  - Exemple : `commande 2> erreurs.log`

- **`&>`**: Redirige à la fois stdout et stderr vers un fichier.
  - Exemple : `commande &> sortie_et_erreurs.txt`

- **`/dev/null`**: Supprime la sortie.
  - Exemple : `commande > /dev/null`

## Combinaison de Redirections
- **`2>&1`**: Redirige stderr vers stdout.
  - Exemple : `commande 2>&1`

- **`|` (Pipe)**: Connecte la sortie d'une commande à l'entrée d'une autre.
  - Exemple : `commande1 | commande2`

## Redirections Avancées
- **Descripteurs de Fichier (`>&`, `<&`)**: Manipule les descripteurs de fichier pour la redirection.
  - Exemple : `commande 2>&1`

## Conclusion
Maîtriser les redirections d'E/S sous Linux est crucial pour une utilisation efficace de la ligne de commande. La pratique et l'expérimentation approfondiront votre compréhension et amélioreront votre capacité à gérer les flux de données de manière efficace.
