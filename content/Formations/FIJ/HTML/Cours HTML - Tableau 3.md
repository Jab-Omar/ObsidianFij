---
date: 2024-03-07
Time: 09:56
---
Crée un tableau qui reprend les prof et les cours. Le titre du tableau sera "Liste des cours".
Ajoute des colspan et rowspan si nécessaire. 

## HTML
```html
<!DOCTYPE html>

<html lang="fr">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Liste des cours</title>

    <link rel="stylesheet" href="style.css">

</head>

<body>

    <table>

        <tr>

            <th colspan="2">Liste des cours</th>

        </tr>

        <tr>

            <td>Formateurs</td>

            <td>Cours</td>

        </tr>

        <tr>

            <td rowspan="2" class="formateur">Géraldine</td>

            <td>HTML</td>

        </tr>

        <tr>

            <td>Français</td>

        </tr>

        <tr>

            <td class="formateur">Gilbert</td>

            <td>Anglais</td>

        </tr>

        <tr>

            <td class="formateur">Wassim</td>

            <td>Windows Réseau</td>

        </tr>

        <tr>

            <td rowspan="2" class="formateur">Alain</td>

            <td>Linux Réseau</td>

        </tr>

        <tr>

            <td>Méthodologie</td>

        </tr>

        <tr>

            <td class="formateur">Véronique</td>

            <td>Helpdesk</td>

        </tr>

        <tr>

            <td class="formateur">Marie</td>

            <td>Emploi</td>

        </tr>

        <tr>

            <td rowspan="2" class="formateur">Simon</td>

            <td>Math aplliquées</td>

        </tr>

        <tr>

            <td>Bases de données</td>

        </tr>

    </table>

</body>

</html>
```

Ce code HTML crée une page web qui affiche une liste de cours avec les formateurs associés dans un tableau. Voici une explication détaillée des différentes parties du code :

1. `<!DOCTYPE html>` : Déclare le type de document HTML.
    
2. `<html lang="fr">` : Définit le début du document HTML et spécifie que la langue utilisée est le français.
    
3. `<head>` : Contient des métadonnées et des liens vers d'autres fichiers, tels que des feuilles de style et des scripts.
    
    - `<meta charset="UTF-8">` : Spécifie l'encodage des caractères en UTF-8 pour prendre en charge les caractères spéciaux.
        
    - `<meta name="viewport" content="width=device-width, initial-scale=1.0">` : Permet une mise en page réactive en ajustant la largeur de la page au périphérique et en définissant le niveau initial de zoom.
        
    - `<title>Liste des cours</title>` : Définit le titre de la page affiché dans l'onglet du navigateur.
        
    - `<link rel="stylesheet" href="style.css">` : Lie le fichier de style externe "style.css" pour appliquer des styles à la page.
        
4. `<body>` : Contient le contenu visible de la page.
    
    - `<table>` : Définit le début d'un tableau.
        
        - `<tr>` : Définit une ligne dans le tableau.
            
            - `<th colspan="2">Liste des cours</th>` : Définit une cellule d'en-tête qui s'étend sur deux colonnes, affichant le titre "Liste des cours".
        - Une autre ligne `<tr>` contenant deux cellules `<td>` avec les libellés "Formateurs" et "Cours".
            
        - Les lignes suivantes `<tr>` décrivent chaque cours et formateur.
            
            - `<td rowspan="2" class="formateur">Géraldine</td>` : Définit une cellule avec la classe "formateur" et s'étend sur deux lignes.
                
            - `<td>HTML</td>` : Définit une cellule avec le nom du cours (HTML dans ce cas).
                
            - Les lignes suivantes suivent le même schéma pour chaque formateur et cours.
                
5. `</table>` : Définit la fin du tableau.
    
6. `</body>` : Définit la fin du contenu visible de la page.
    
7. `</html>` : Définit la fin du document HTML.
    

En résumé, ce code crée une page web avec un tableau organisé affichant les cours et les formateurs associés. Les styles pour la mise en forme sont définis dans le fichier externe "style.css".

## CSS
```css
table, th, td {

    border: 1px solid black;

    border-collapse: collapse;

  }

table{

    width: auto;

    margin-left: auto;

    margin-right: auto;

}

th, td {

    padding: 15px;

  }

th{

    font-size: 40px;

}

td{

    font-size: 32px;

}

.formateur{

    font-size: 34px;

}

.formateur:hover{

    color: saddlebrown;

}
```

1. **`table, th, td`** :
    
    - `border: 1px solid black;` : Ajoute une bordure d'un pixel solide de couleur noire à la table, aux cellules d'en-tête (`th`), et aux cellules de données (`td`).
    - `border-collapse: collapse;` : Indique que les bordures des cellules doivent être fusionnées (collapsed) pour éviter tout espace entre les cellules.
2. **`table`** :
    
    - `width: auto;` : Définit la largeur de la table comme automatique, s'ajustant en fonction de son contenu.
    - `margin-left: auto; margin-right: auto;` : Centre horizontalement la table en la positionnant automatiquement à gauche et à droite.
3. **`th, td`** :
    
    - `padding: 15px;` : Ajoute un remplissage interne de 15 pixels aux cellules d'en-tête (`th`) et aux cellules de données (`td`), créant de l'espace à l'intérieur de chaque cellule.
4. **`th`** :
    
    - `font-size: 40px;` : Définit la taille de la police des cellules d'en-tête (`th`) à 40 pixels.
5. **`td`** :
    
    - `font-size: 32px;` : Définit la taille de la police des cellules de données (`td`) à 32 pixels.
6. **`.formateur`** :
    
    - `font-size: 34px;` : Définit la taille de la police pour les éléments avec la classe "formateur" à 34 pixels.
7. **`.formateur:hover`** :
    
    - `color: saddlebrown;` : Change la couleur du texte des éléments avec la classe "formateur" lorsqu'ils sont survolés par la souris à la couleur "saddlebrown".

En résumé, ce code CSS apporte des styles visuels à la table HTML et ses éléments associés, en définissant des bordures, des marges, des tailles de police, et en ajoutant des effets visuels au survol pour les éléments avec la classe "formateur". Ces styles contribuent à une présentation claire et attrayante de la liste des cours sur la page web.