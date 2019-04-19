# Documents type pour Medispring

Des documents types pour le DMI Medispring

Ce répertoire contient des canevas de documents utilisables dans le logiciel médical (DMI) MEDISPRING

## Quels Documents Types

Les documents présents ici sont écrit en HTML tel que le logiciel peut les comprendre et les traiter.
Ce ne sont pas des documents répondant entièrement aux règles de rédaction des documents HTML, dans le sens où, les balises HEAD, BODY, STYLE et SCRIPT ne sont pas présentes, si elles étaient présentes, l'éditeur de texte du logiciel les suprimerait.  L'encodage est à l'image d'un message mail, avec les instructions de formattage insérées dans les blocs du document.

Ces documents types respectent les balises d'insertion des données du logiciel liées à l'utilisateur, au patient ou à la consultation.

Ils sont différents et complètent la collection des documents types de base.

## Comment les utiliser

Pour utiliser l'un de ces documents, il faut l'intégrer dans les documents types du logiciel.
Les documents types sont personnels, ils ne seront disponibles que dans la session appartenant à l'utilisateur qui les aura installés.

- Coisir le rapport et cliquer
- Cliquer RAW
- Copier l'entièreté du contenu (ctrl-c)
- Aller dans le paramétrage du logiciel (engrenage)
- Cliquer 'Documents Types'
- cliquer Créer un nouveau document type
- Le nommer en débutant son nom par une lettre majuscule
- cliquer dans la barre d'outils, le bouton <>
- Mettre le curseur dans la petite fenêtre fraîchement ouverte
- Coller le contenu préalablement copié (ctrl-v)
- Cliquer Ok pour refermer la fenêtre
- A ce stade il serait intéressant de pouvoir imprimer une épreuve, mais il n'y a pas de bouton d'impression
- Cliquer enregistrer pour sauvegarder le nouveau document type

Remarque:
Les documents types sont triés par ordre alphabétiques, mais en séparant les majuscules des minuscules.  Techniquement, il ne s'agit pas d'un tri alphbétique mais d'un tri ASCII.

## tester les documents types

Créer une consultation ou en modifier une récente.
Sous le P de SOAP, ajouter le document fraîchement créé
Imprimer le résultat

remarque:
Pour ne rien polluer dans les données, il est intéressant de se créer un patient de test.

Pour créer facileent un numéro national, copier son propre NIS, ajouter un jour et additionner 1 au nombre formé par les deux derniers chiffres.  Il sera valide et ne devrait pas faire doublon.

## Derniers ajustements

Tous les documents types peuvent être modifiés ou remplacés par la méthode décrite ci-dessus ou modifiés à l'aide de l'éditeur fourni par le logiciel.

## Balises HTML non ou mal supportées par l'editeur WYSIWYG du logiciel

Le DMI lorsqu'il lance l'impression d'un docuent, l'entoure probablement de règles CSS.  Ces règles sont différentes entre l'écran et le papier.  Un simple H1 peut prendre des proportions TRES imposantes.

```html
<script>
<style>
<head>
<body>
<h1>

```
