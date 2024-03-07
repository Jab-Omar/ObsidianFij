---
date: 07-03-2024
Time: 11:18
---
Consigne : Faire en HTML et CSS un horaire similaire que celui de la classe. 

## HTML
```html
<!DOCTYPE html>

<html lang="fr">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>horaire</title>

    <link rel="stylesheet" href="style.css">

    <link rel="preconnect" href="https://fonts.googleapis.com">

<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">

</head>

<body>

    <table>

        <tr>

            <th colspan="6">Technicien.ne Informatique cert.tui<br><em>Du 4 mars au 8 mars 2024 Semaine 9</em></th>

        </tr>

        <tr>

            <td class="horaire">Heures</td>

            <td class="jour">Lundi</td>

            <td class="jour">Mardi</td>

            <td class="jour">Mercredi</td>

            <td class="jour">Jeudi</td>

            <td class="jour">Vendredi</td>

        </tr>

        <tr>

            <td class="horaire">8h55 à 10h40</td>

            <td><strong>Html</strong><br>Géraldine<br><mark>Shiva</mark></td>

            <td><strong>Windows Réseau</strong><br>Wassim<br><mark>Shiva</mark></td>

            <td class="vide"></td>

            <td><strong>Html</strong><br>Géraldine<br><mark>Shiva</mark></td>

            <td rowspan="2"><strong>BDD</strong><br>Simon<br><mark>Shiva</mark></td>

        </tr>

        <tr>

            <td class="horaire">10h50 à 12h35</td>

            <td><strong>Anglais</strong><br>Gilbert<br><mark>Shiva</mark></td>

            <td><strong>Méthodo</strong><br>Alain<br><mark>Shiva</mark></td>

            <td><strong>Helpdesk</strong><br>Véronique & Wassim<br><mark>Shiva</mark></td>

            <td><strong>Français</strong><br>Géraldine<br><mark>Shiva</mark></td>

        </tr>

        <tr>

            <td class="horaire">12h35 à 13h25</td>

            <td colspan="5">Pause de Midi</td>

        </tr>

        <tr>

            <td class="horaire">13h25 à 15h10</td>

            <td rowspan="2"><strong>Linux Réseau</strong><br>Alain<br><mark>Shiva</mark></td>

            <td rowspan="2"><strong>Linux Réseau</strong><br>Alain<br><mark>Shiva</mark></td>

            <td rowspan="2"><strong>Math Appliquées</strong><br>Simon<br><mark>Shiva</mark></td>

            <td><strong>Anglais</strong><br>Gilbert<br><mark>Shiva</mark></td>

            <td rowspan="2"><strong>Windows Réseau</strong><br>Wassim<br><mark>Shiva</mark></td>

        </tr>

        <tr>

            <td class="horaire">15h20 à 17h00</td>

            <td><strong>Emploi</strong><br>Marie<br><mark>Shiva</mark></td>

        </tr>

  

    </table>

</body>

</html>
```
Ce code HTML représente une page web affichant un emploi du temps pour un(e) Technicien(ne) Informatique certifié(e) pour la semaine du 4 mars au 8 mars 2024 (Semaine 9). Voici une explication détaillée du code :

1. **Doctype et Balise HTML :**
   - `<!DOCTYPE html>` déclare le type de document comme étant un document HTML5.
   - `<html lang="fr">` indique que la page est écrite en français.

2. **Balise Head :**
   - Les balises `<head>` contiennent des métadonnées et des liens vers des feuilles de style et des polices.
   - `charset="UTF-8"` définit l'encodage des caractères comme UTF-8.
   - La balise `<meta name="viewport" content="width=device-width, initial-scale=1.0">` est utilisée pour rendre la page responsive sur les appareils mobiles.
   - Le titre de la page est défini avec `<title>horaire</title>`.
   - Des liens vers une feuille de style externe (`style.css`) et une police Google Fonts (`Montserrat`) sont inclus.

3. **Balise Body :**
   - Le corps de la page (`<body>`) contient un tableau (`<table>`) qui représente l'emploi du temps.
   - Les différentes parties de l'emploi du temps sont organisées en lignes (`<tr>`) et colonnes (`<td>`).
   - Les horaires, les jours de la semaine, et les matières avec les noms des enseignants sont affichés dans les cellules du tableau.
   - Certains cours ont des cellules fusionnées à l'aide de l'attribut `rowspan` pour indiquer qu'ils s'étendent sur plusieurs plages horaires.

4. **Classes CSS :**
   - Le code utilise des classes CSS telles que `horaire`, `jour`, `vide` pour styliser différentes parties du tableau.
   - Les balises `<strong>` sont utilisées pour mettre en évidence le nom des matières.
   - La balise `<mark>` est utilisée pour mettre en surbrillance le nom de l'enseignant.

5. **Commentaires HTML :**
   - Certains commentaires (`<!-- ... -->`) sont inclus pour donner des informations supplémentaires sur le contenu de certaines cellules.

L'ensemble du code vise à présenter de manière structurée et lisible un emploi du temps hebdomadaire pour un(e) Technicien(ne) Informatique certifié(e).
## CSS
```css
table, th, td {

    border: 1px solid black;

    border-collapse: collapse;

    padding: 10px;

    text-align: center;

}

table{

    margin-right: 5%;

    margin-left: 5%;

    margin-top: 5%;

}

td{

    width: 10%;

    background-color: rgba(189, 89, 7, 0.432);

    font-size:18px;

    font-family: "Montserrat", sans-serif;

}

.vide{

    background-color: black;

}

th{

    font-size: 40px;

    background-color: lemonchiffon;

}

em{

    font-size: 16px;

    display: block;

    width: 100%;

    font-style: normal;

    background-color: rgba(12, 11, 11, 0.623);

    color: rgba(255, 255, 255, 0.863);

    border-radius: 10px;

}

.horaire{

    background-color: whitesmoke;

}

.jour{

    background-color: whitesmoke;

}

mark{

    background-color: rgb(255, 174, 0);

    font-size: 14px;

}
```
Ce code CSS est destiné à styliser la présentation d'un tableau HTML qui semble représenter un emploi du temps. Voici une explication des différentes règles de style :

1. **Styling de la table, des en-têtes (th) et des cellules (td) :**
   ```css
   table, th, td {
       border: 1px solid black;
       border-collapse: collapse;
       padding: 10px;
       text-align: center;
   }
   ```
   - `border: 1px solid black;` : Ajoute une bordure noire de 1 pixel autour de la table, des en-têtes et des cellules.
   - `border-collapse: collapse;` : Fusionne les bordures adjacentes pour donner un aspect plus propre.
   - `padding: 10px;` : Ajoute un espace de remplissage de 10 pixels à l'intérieur des cellules.
   - `text-align: center;` : Centre le texte à l'intérieur des cellules.

2. **Styling spécifique à la table :**
   ```css
   table {
       margin-right: 5%;
       margin-left: 5%;
       margin-top: 5%;
   }
   ```
   - Ajoute des marges à la table pour la positionner à 5% du bord droit, 5% du bord gauche et 5% du bord supérieur.

3. **Styling spécifique aux cellules (td) :**
   ```css
   td {
       width: 10%;
       background-color: rgba(189, 89, 7, 0.432);
       font-size: 18px;
       font-family: "Montserrat", sans-serif;
   }
   ```
   - Définit la largeur des cellules à 10% de la largeur totale de la table.
   - Fixe la couleur de fond à une teinte orangée semi-transparente.
   - Définit la taille de la police à 18 pixels et la famille de police à "Montserrat" ou sans-serif.

4. **Styling pour les cellules avec la classe "vide" :**
   ```css
   .vide {
       background-color: black;
   }
   ```
   - Donne aux cellules ayant la classe "vide" une couleur de fond noire.

5. **Styling pour les en-têtes (th) :**
   ```css
   th {
       font-size: 40px;
       background-color: lemonchiffon;
   }
   ```
   - Définit la taille de la police des en-têtes à 40 pixels.
   - Fixe la couleur de fond à une teinte jaune pâle.

6. **Styling pour la balise `<em>` :**
   ```css
   em {
       font-size: 16px;
       display: block;
       width: 100%;
       font-style: normal;
       background-color: rgba(12, 11, 11, 0.623);
       color: rgba(255, 255, 255, 0.863);
       border-radius: 10px;
   }
   ```
   - Définit la taille de la police de la balise `<em>` à 16 pixels.
   - Définit la largeur à 100%, la rendant une balise de bloc.
   - Modifie le style de la police à normal.
   - Ajoute une couleur de fond semi-transparente, une couleur de texte blanche et des coins arrondis à la balise `<em>`.

7. **Styling pour les cellules avec la classe "horaire" et "jour" :**
   ```css
   .horaire, .jour {
       background-color: whitesmoke;
   }
   ```
   - Donne aux cellules ayant les classes "horaire" et "jour" une couleur de fond blanc fumé.

8. **Styling pour la balise `<mark>` :**
   ```css
   mark {
       background-color: rgb(255, 174, 0);
       font-size: 14px;
   }
   ```
   - Donne à la balise `<mark>` une couleur de fond jaune orangé et une taille de police de 14 pixels.