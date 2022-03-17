<a href="https://juncture-digital.org" target="_blank"><img src="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/images/btn_juncture.svg" style="height:40px"></a>

<param ve-config 
       title="depart" 
       banner="/images/ViennaDioscoridesFolio483vBirds.jpg" 
       layout="vertical">
       
<param ve-entity eid="Q208220" aliases="démarrage">

# Fichier de démarrage

Ceci est un fichier de démarrage que vous pouvez modifier pour créer votre propre récit numérique.
<param ve-graphic
    url="https://github.com/digitalArtHistory/recits-numeriques/blob/main/27/astafieva2.PNG"
    title="">

Voici quelques actions à réaliser pour commencer :
- modifier le titre de votre essai visuel
- modifier l’image de l’en-tête de votre essai visuel
- enregistrer vos modifications avec une courte description de ce que vous avez fait (cf. « commit » en bas de cette page)
- visualiser votre page en cliquant sur le bouton « mon essai visuel »
<param ve-graphic 
  url="https://upload.wikimedia.org/wikipedia/commons/c/c8/Gargouilles_%28RA_549%29_3.jpg" 
  title="Gargouilles" />

# Explorer Markdown

Markdown est une syntaxe très simple destinée à créer des contenus pour le web en HTML. Voici quelques exemples :
<param ve-tabulator
    url="https://raw.githubusercontent.com/HTR-United/htr-united/master/statistics.csv" />

```
# Titre de niveau 1

## Titre de niveau 2

### Titre de niveau 3
```

Ceci est un paragraphe. Celui-ci contient du texte **en gras** mais aussi du texte *en italique*. Markdown permet également de créer des hyperliens. La cible du lien est indiquée entre crochets `[` et `]` et immédiatement suivi de l’URL entre parenthèses. Par exemple voici un lien vers le site de l’[Université de Montréal](http://www.umontreal.ca).

Ceci est un nouveau paragraphe...  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus dui arcu, venenatis a porta non, malesuada eu eros. Vivamus arcu nisi, imperdiet sit amet fringilla ac, pretium nec ex. Proin vel bibendum massa, vitae lacinia magna. Nunc venenatis augue quis purus imperdiet, nec accumsan lectus elementum. Ut tellus massa, sodales vitae feugiat et, porta ut libero. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Curabitur ornare tempus vulputate. Donec tincidunt est ullamcorper mi interdum aliquam. Nunc id placerat velit. Duis et est nulla. 
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/bpt6k877400g/manifest.json"
       seq="49"/>
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/bpt6k877400g/manifest.json"
       seq="50"/>
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/bpt6k877400g/manifest.json"
       seq="51"/>

Vous pouvez toujours utiliser l’interface graphique de GitHub mais il est souvent plus rapide et plus simple de directement tapper le texte...
<param ve-iframe src="http://www.tadao-ando.com" />

Voici quelques ressources sur Markdown
- [Guide markdown (EN)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Débuter avec markdown (FR)](https://programminghistorian.org/fr/lecons/debuter-avec-markdown)

## Premiers pas avec Juncture (travail dirigé)

Afin de prendre en main la rédaction d’essais visuels avec [Juncture](https://juncture-digital.org/), nous allons introduire quelques fonctionnalités de base du logiciel que vous pourrez ensuite utiliser dans votre propre travail. Pour le moments, contentez-vous de nous suivre pas-à-pas. Au cours de cet exercice, nous allons successivement :
- créer des sections interactives (paragraphes)
- insérer une image
- insérer une image avec IIIF
- insérer un lien Wikidata
- intégrer une vidéo

Tableau de données

I love cheese, especially when the cheese comes out everybody's happy caerphilly. Cheesy grin fromage frais chalk and cheese pecorino dolcelatte lancashire cheesy feet cheesy feet. Queso taleggio croque monsieur goat airedale cheese and wine roquefort roquefort. Bavarian bergkase boursin cream cheese halloumi cottage cheese hard cheese port-salut smelly cheese. Camembert de normandie cream cheese who moved my cheese cream cheese rubber cheese swiss melted cheese when the cheese comes out everybody's happy. Parmesan when the cheese comes out everybody's happy stilton cauliflower cheese airedale cheese triangles jarlsberg cheese slices. Lancashire roquefort everyone loves pepper jack cheese slices everyone loves swiss red leicester. Mascarpone port-salut.
<param ve-tabulator
    url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/27/artpublic.csv">
    
Babybel cheese triangles camembert de normandie. Who moved my cheese manchego mascarpone mascarpone caerphilly cheese and wine cheese triangles monterey jack. Queso ricotta cheeseburger stilton croque monsieur babybel cow the big cheese. Cheese strings blue castello ricotta cheese strings boursin chalk and cheese when the cheese comes out everybody's happy rubber cheese. Hard cheese red leicester cut the cheese cauliflower cheese cauliflower cheese mascarpone cheese and biscuits pecorino. Cream cheese croque monsieur lancashire emmental say cheese smelly cheese squirty cheese monterey jack. Mascarpone emmental roquefort melted cheese parmesan cheese and wine when the cheese comes out everybody's happy cheesy grin. Cauliflower cheese cheddar cheese and biscuits cut the cheese.
<param ve-tabulator
    url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/27/artpublic.csv">


Voici du texte qui va être associé à une carte centrée sur Rimouski. Nous y voyons les œuvres d'art public de la ville de Rimouski, dont la géolocalisation est partagée sur le site de [données ouvertes du Québec](https://www.donneesquebec.ca/recherche/dataset/art-public).
<param ve-map ve-map center="48.4501730, -68.5213712" zoom="13.5"/>
<param ve-map-layer geojson url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/27/artRimouski.geojson" title="Art Public Rimouski" active/> 

Babybel cheese triangles camembert de normandie. Who moved my cheese manchego mascarpone mascarpone caerphilly cheese and wine cheese triangles monterey jack. Queso ricotta cheeseburger stilton croque monsieur babybel cow the big cheese. Cheese strings blue castello ricotta cheese strings boursin chalk and cheese when the cheese comes out everybody's happy rubber cheese. Hard cheese red leicester cut the cheese cauliflower cheese cauliflower cheese mascarpone cheese and biscuits pecorino. Cream cheese croque monsieur lancashire emmental say cheese smelly cheese squirty cheese monterey jack. Mascarpone emmental roquefort melted cheese parmesan cheese and wine when the cheese comes out everybody's happy cheesy grin. Cauliflower cheese cheddar cheese and biscuits cut the cheese.
<param ve-map ve-map center="48.4501730, -68.5213712" zoom="13.5"/>
<param ve-map-layer geojson url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/27/artRimouski.geojson" title="Art Public Rimouski" active/> 

Ici nous pouvons zoomer sur <span data-click-map-flyto="45.5031824, -73.5698065,11">Montréal</span>. I love cheese, especially when the cheese comes out everybody's happy caerphilly. Cheesy grin fromage frais chalk and cheese pecorino dolcelatte lancashire cheesy feet cheesy feet. Queso taleggio croque monsieur goat airedale cheese and wine roquefort roquefort. Bavarian bergkase boursin cream cheese halloumi cottage cheese hard cheese port-salut smelly cheese. Camembert de normandie cream cheese who moved my cheese cream cheese rubber cheese swiss melted cheese when the cheese comes out everybody's happy. Parmesan when the cheese comes out everybody's happy stilton cauliflower cheese airedale cheese triangles jarlsberg cheese slices. Lancashire roquefort everyone loves pepper jack cheese slices everyone loves swiss red leicester. Mascarpone port-salut.
<param ve-map ve-map center="48.4501730, -68.5213712" zoom="13.5"/>
<param ve-map-layer geojson url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/27/artRimouski.geojson" title="Art Public Rimouski" active/> 


<!-- <span data-mouseover-map-flyto="41.893,12.483,11">Rome</span> -->
