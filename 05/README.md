<a href="https://juncture-digital.org"><img src="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/images/btn_juncture.svg" style="height:40px"></a>

<param ve-config 
       title="depart" 
       banner="/images/ViennaDioscoridesFolio483vBirds.jpg" 
       layout="vertical">

# Fichier de démarrage

Ceci est un fichier de démarrage que vous pouvez modifier pour créer votre propre récit numérique.

Voici quelques actions à réaliser pour commencer :
- modifier le titre de votre essai visuel
- modifier l’image de l’en-tête de votre essai visuel
- enregistrer vos modifications avec une courte description de ce que vous avez fait (cf. « commit » en bas de cette page)
- visualiser votre page en cliquant sur le bouton « mon essai visuel »



## Premiers pas avec Juncture (travail dirigé)

Afin de prendre en main la rédaction d’essais visuels avec [Juncture](https://juncture-digital.org/), nous allons introduire quelques fonctionnalités de base du logiciel que vous pourrez ensuite utiliser dans votre propre travail. Pour le moments, contentez-vous de nous suivre pas-à-pas. Au cours de cet exercice, nous allons successivement :
- créer des sections interactives (paragraphes)
- insérer une image
- insérer une image avec IIIF
- insérer un lien Wikidata
- intégrer une vidéo

voici une image de gargouille
<param ve-graphic 
  url="https://upload.wikimedia.org/wikipedia/commons/c/c8/Gargouilles_%28RA_549%29_3.jpg" 
  title="Gargouilles" />
  
voici une image de dragon qui provient d'un ouvrage de bestiaire. Cet ouvrage se base comme un encyclopédie pour expliquer le monde qui entoure la communauté humaine au Moyen Âge. Il suffit d'une peur des reptiles pour y voir une légende de dragon pour les artistes de l'époque et ainsi faire fructifier l'imaginaire bla blaa vla bla vla bvld aldmsf
<param ve-graphic 
  url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/05/dragon.jpeg" 
  title="dragon" />
  
  
  Présentation

Le griffon est un animal légendaire représenté le plus souvent avec le corps arrière d'un lion (corps, pattes arrières et queue) et un avant d'aigle (pattes avant, poitrail et tête). Le plus souvent, les griffons sont affublés d’oreilles longues et pointues comme celles des chevaux, de chats ou de certains chiens, en fonction des époques et des ethnies. De même, parfois on peut le voir représenté avec quatre pattes de lion. Dans ce dernier cas, on l'appelle un opinicus.

Dans énormément de cultures, le lion est le roi des animaux terrestres et l'aigle celui des animaux célestes. Né de cette union entre ces deux rois, le griffon est donc souvent considéré comme le roi de tous les animaux.

Au travers des cultures différentes qu'il a traversées, le griffon a reçu les rôles de gardien de trésors, de tombes ou de temples, mais également de monture divine.
Son rôle de gardien est, probablement le plus courant puisque, au Moyen-Âge, il était souvent utilisé comme gargouilles pour protéger les cathédrales des esprits malins.

On pourra également souligner que dans l'iconographie chrétienne, le griffon est, au départ, une créature maléfique. Cependant, sa valeur a évolué au fil du temps : cet animal légendaire a fini par représenter la double nature du Christ. Ainsi, le lion, animal terrestre rappelait la condition humaine de Jésus, tandis que l'aigle, animal du ciel représentait sa dimension divine.
<param ve-image 
    manifest=:"//baobab.biblissima.fr/sites/interne.biblissima-condorcet.fr.boiteaoutils/files/green2.jpg" />
    Il a également eu, à certaines périodes de l'histoire le rôle de gardien (encore) et de guide des morts. Il était chargé de l'importante mission de mener les âmes des morts dans l'Autre Monde.

Le griffon est également un meuble important en héraldique. Il représente la force et le courage du lion mêlés à la vigilance et à la ruse de l'aigle, mais également la justice et la protection, valeurs dont il est considéré comme le gardien... toujours !

Les textes anciens lui accordaient un habitat bien particulier : une montagne ou un désert où l'on trouve de l'or dont les griffons se serviraient pour faire leurs nids.
On leur prête également la force de cent aigles ou de huit lions et leurs griffes noirciraient au contact du poison.

Origines
<param ve-image 
    manifest="://gallica.bnf.fr/blog/sites/default/files/a_la_une_fieres_de_lettres.jpg" />
Les plus anciennes représentations de griffons connues à l'heure actuelle datent du IVè siècle avant notre ère en Élam (un ancien pays occupant la partie sud-ouest du plateau Iranien, voisin de la Mésopotamie) ainsi qu'en Égypte datant de -3000.
Par la suite, les légendes grecques et romaines reprirent cet animal mythique au travers de légendes diverses telles que les griffons gardiens des trésors d’Apollon dans l'Altaï. Dans cette légendes, il est question d'un peuple, les Arimaspes, qui guerroyaient sans cesse contre les griffons afin de leur voler l'or d'Apollon.
Adrienne Mayor, spécialiste des folklores classiques, pense que ces légendes sont dues à la présence de fossiles de protocératops trouvés près des mines d'or de l'Altaï, chaîne montagneuse qui s'étend du Kazakhstan jusqu'en Mongolie.  
  « […] l'Indois Griffon aux yeus estincelans,
A la bouche aquiline, aux ailes blanchissantes,
Au sein rouge, au dos noir, aux griffes ravissantes,
Dont il va guerroyant et par monts et par vaux
Les lyons, les sangliers, les ours, et les chevaux :
Dont il fouille pillard le feconde poictrine
De nostre bisayeule, et là dedans butine
Maint riche lingot d'or, pour apres en plancher,
Son nid haut eslevé sur un aspre rocher :
Dont il deffend, hardi, contre plusieurs armees
Les mines par sa griffe une fois entamees ».  
<param ve-graphic 
  url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/05/griffon.jpeg" />
  
  
# Explorer Markdown

Markdown est une syntaxe très simple destinée à créer des contenus pour le web en HTML. Voici quelques exemples :

```
# Titre de niveau 1

## Titre de niveau 2

### Titre de niveau 3
```

Ceci est un paragraphe. Celui-ci contient du texte **en gras** mais aussi du texte *en italique*. Markdown permet également de créer des hyperliens. La cible du lien est indiquée entre crochets `[` et `]` et immédiatement suivi de l’URL entre parenthèses. Par exemple voici un lien vers le site de l’[Université de Montréal](http://www.umontreal.ca).

Ceci est un nouveau paragraphe...  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus dui arcu, venenatis a porta non, malesuada eu eros. Vivamus arcu nisi, imperdiet sit amet fringilla ac, pretium nec ex. Proin vel bibendum massa, vitae lacinia magna. Nunc venenatis augue quis purus imperdiet, nec accumsan lectus elementum. Ut tellus massa, sodales vitae feugiat et, porta ut libero. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Curabitur ornare tempus vulputate. Donec tincidunt est ullamcorper mi interdum aliquam. Nunc id placerat velit. Duis et est nulla. 

> Ceci est du texte cité.

Vous pouvez toujours utiliser l’interface graphique de GitHub mais il est souvent plus rapide et plus simple de directement tapper le texte...

Voici quelques ressources sur Markdown
- [Guide markdown (EN)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Débuter avec markdown (FR)](https://programminghistorian.org/fr/lecons/debuter-avec-markdown)
