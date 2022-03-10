[Juncture](https://juncture-digital.org/) est un projet expérimental de l’organisme à but non lucratif JStor destiné à publier des essais visuels interactifs. L’utilisation de Juncture ne nécessite aucune connaissance informatique mais permet de présenter des essais enrichis avec des ressources visuelles, avec des cartes ou des données.

## Documentation de Juncture

- [Quick Start](https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Quick-Start)
- [Tags Visual Essay](https://github.com/jstor-labs/juncture/wiki/visual-essay-tags)
- [Récapitulatif de la syntaxe Markdown](https://github.com/jstor-labs/juncture/wiki/Markdown-Primer)

## Récapitulatif des Tags pour créer des composants interactifs

Les différents composants interactifs de Juncture sont insérés avec des éléments `param` identifiés par attribut préfixé par `ve-`. Chaque composant dispose de plusieurs attributs qui servent à personnaliser leur comportement.

**Exemple**

```html
<param ve-identifiant attribut="valeur" />
```

Un élément débute par une séquence de caractères `<`, le nom de l’élément et se termine par `/>`. Les attributs son placés à l’intérieur de la balise et séparé du nom de l’élément par un espace. Ils prennent la forme `nom="valeur"`. Attention à bien placer la valeur à l’intérieur des guillemets et à ne pas ajouter d’espace superflus.

### Visualiseur d’image (`ve-graphic`)

Pour ajouter des images fixes, on utilise l’élément `<param ve-graphic />` avec les attributs `url` et `title`.  

- `url` lien ou chemin vers l’image,  
- `title` titre de l’image.  

**Exemple**

```html
<param ve-graphic 
  url="https://upload.wikimedia.org/wikipedia/commons/c/c8/Gargouilles_%28RA_549%29_3.jpg" 
  title="Gargouilles" />
```

**Copiez ce bloc-ci :**

```html
<param ve-graphic url="" title="" />
```

➡️ Voir [Documentation sur les composants Graphic](https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Graphic-Tag)

---

### Affichage de vidéo YouTube (`ve-video`)

Pour ajouter des vidéos YouTube, on utilise l’élément `<param ve-video />` avec les attributs `id`, `title` et `start`. L’attribut `id` permet d'indiquer l'identifiant de la vidéo YouTube : par exemple pour la vidéo "https://youtu.be/a3ta5Q3ITUc", l’identifiant est "a3ta5Q3ITUc". L’attribut `title` permet d’indiquer le titre de la vidéo, et enfin `start` permet de préciser à quelle seconde déclencher la vidéo.  

- `id` identifiant de la vidéo YouTube
- `title` titre de la vidéo
- `start` point de départ de la vidéo

**Exemple**

```hmtl
<param ve-video id="a3ta5Q3ITUc" title="Walter, the cat" start="26" />
```

**Copiez ce bloc-ci :**

```hmtl
<param ve-video id="" title="" start="" />
```

➡️ Voir [Documentation sur les composants Video](https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Video-Tag)


---

### Visualiseur interactif de données tabulaires (`ve-tabulator`)

Pour afficher un tableau de données, on utilise l'élément `ve-tabulator`. Cet élément ne possède qu'un seul attribut : `url`.

- `url` lien ou chemin vers un fichier tabulaire brut (CSV, TSV...)[^1]

**Exemple**

```html
<param ve-tabulator
    url="https://raw.githubusercontent.com/HTR-United/htr-united/master/statistics.csv" />
```

**Copiez ce bloc-ci**

```html
<param ve-tabulator src="" />
```

---

### Élément HTML embarqué (`ve-iframe`)

Les iframes permettent d’intégrer très simplement du contenu web à l’intérieur d’une page web. Il peut s’agir d’une page web, d’une vidéo YouTube ou encore d’un fichier brut (`json` ou `txt` par exemple) hébergé en ligne.

Un seul attribut pour ce composant : `src` qui sert à indiquer la source de l’élément à afficher.

**Exemple**

```html
<param ve-iframe 
    src="https://www.youtube.com/embed/5fJDslITV34" />
```

**Copiez ce bloc-ci**
```html
<param ve-iframe src="" />
```

---

### Frise chronologique avec TimelineJS (`ve-knightlab-timeline`)

La publication de chronologies sur Juncture utilise l’outil TimelineJS de Knightlab.

Ici le plus gros consiste à construire la frise avec Knightlab en suivant les instructions données ici : https://timeline.knightlab.com/#make

Knightlab fournit une URL au format suivant (la liste des paramètres peut varier) :  

``` 
https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?
    source={id de la source}&
    lang={langue, 'en' par défaut}&
    font={font, 'Default' par défaut}&
    timenav_position={bottom|top}&
    hash_bookmark={true|false}&
    initial_zoom={niveau de zoom}&
    start_at_slide={# de la slide de départ, 0 par défaut}&
    height={hauteur de la frise, 650 par défaut}
```

Chacun de ces éléments peut être redistribué dans les attribues de l’éléments `ve-knightlab-timeline`. On a donc les attributs `source`, `timenav-position`, `initial-zoom` et `height` correspondant à une partie des options listées ci-dessus. L’attribut `hash-bookmark` permet de créer des liens URL pour chaque étape de la frise. 

```html
<param ve-knightlab-timeline
    source="" # id de la frise
    timenav-position="" # position de la frise (top ou bottom)
    hash-bookmark="" # création de liens unique pour chaque slide de la frise (true ou false)
    initial-zoom="" # échelle de zoom 
    height="" # hauteur de la frise en pixel />
```

Notons qu’on obtient le même résultat avec `ve-iframe` et l’URL fournie par Knightlab (avec même plus d’options de personnalisation).

---

### Visualiseur IIIF (`ve-image`)

➡️ voir [Options pour le visualiseur IIIF](https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Image-Tag#options)
➡️ voir [Options avancées](https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Image-Tag#interactions)

Avec un manifest IIIF :
```html
<param ve-image
    manifest="" # lien vers manifest.json
/>
```
Les métadonnées associées au manifest sont en partie importées. Attention, si le manifest renvoit à plusieurs images, une seule image est affichée (par défaut, la première voir les option `seq` et `ref` pour modifier cela).

En pointant vers une image spécifiquement :
```html
<param ve-image
    url="" # lien vers image (JPG ou PNG seulement) servi par IIIF
/>
```

Ajouter texte alternatif et description (inutile avec manifest):
```html
<param ve-image
    ...
    label=""
    description=""
/>
```

Ajouter la licence : 

```html
<param ve-image
    ...
    license="CC BY-SA"
/>
```

Autres options: 
| attribut | effet |
| :------- | :---- |
| `fit` | This attribute defines how an image will be scaled or cropped in the image viewer window. Possible values: `contain`, `cover` (default)
| `rotate` | The rotate attribute will rotate the image by the degree number specified. For example` | "90", "180". | 
| `region` | The region attribute is used to show a cropped region of the image in the image viewer. The entire image is loaded and can be seen by zooming and panning but the initial display will only include the specified region. The value for a region is a comma separated sequence of 4 integers representing the origin, width and height. The origin includes both the x and y coordinates relative to the top left of the image. The region may be expressed as absolute pixel values or as percentages of the relative values. More information on IIIF regions can be found at https | //iiif.io/api/image/2.0/#region | 
| `layers` | A multi-image viewer mode that superimposes one image over another with an opacity slider. This mode is activated by including layers or layers="true" on the first ve-image tag when multiple images are associated with an element. | 
| `curtain` | A multi-image viewer mode that overlays one image over another with a curtain slider. This mode is activated by including curtain or curtain="true" on the first ve-image tag when multiple images are associated with an element. | 
| `compare` | A multi-image viewer mode that simultaneously displays multiple images in the viewer pane. This mode is activated by including compare or compare="true" on the first ve-image tag when multiple images are associated with an element. | 
| `ref` | A reference ID (numerical integers) that is used to identify images when multiple are present in one viewer. This is used when a specific image or specific image and region needs to be shown when specified text is clicked. | 
| `seq` | The seq attribute can be used to select a specific image in a manifest if there is more than one image, such as in a book manifest. This attribute accepts the sequence or page number of the desired image. |

Exemples :  

``` html
# manifest de la BnF avec une seule image
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/btv1b53125897q/manifest.json" 
    license="CC BY-SA"/>

# manifest de la BnF avec plusieurs images, où l'on cible la 11e
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/btv1b10539087h/manifest.json" 
    license="CC BY-SA"
    seq="10"/>

# URL vers une image servie par IIIF, les métadonnées doivent être ajoutées manuellement
<param ve-image url="https://gallica.bnf.fr/iiif/ark:/12148/btv1b10539087h/f18/full/1500/0/native.jpg" 
    license="CC BY-SA"
    description="Le Nouvel Opéra de Paris"
    fit="contain"/>
```

Pour créer un carrousel on peut mettre les composants à la suite les uns des autres :  

``` html
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/btv1b53125897q/manifest.json" license="CC BY-SA">
<param ve-image manifest="https://gallica.bnf.fr/iiif/ark:/12148/btv1b10539087h/manifest.json" license="CC BY-SA" seq="10">
<param ve-image url="https://gallica.bnf.fr/iiif/ark:/12148/btv1b10539087h/f18/full/1500/0/native.jpg" license="CC BY-SA" description="Le Nouvel Opéra de Paris" fit="contain"/>
```

---

## Pas encore testés :  

- Map (`ve-map`) et Map Layer (`ve-map-layer`) : https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Map-Tag et https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Map-Layer-Tag
- Network (`ve-vis-network`, `ve-d3plus-network`, & `ve-d3plus-ring-network`) : https://github.com/jstor-labs/juncture/wiki/Visual-Essay-Network-Tags

Pour naviguer dans la carte

```html
Voici du texte qui va être associé à une carte centrée sur Rimouski
Ici nous pouvons zoomer sur <span data-click-map-flyto="41.893,12.483,11">Rome</span>
Ensuite on continue

<param ve-map ve-map center="48.4501730, -68.5213712" zoom="13.5"/>
<param ve-map-layer geojson url="https://raw.githubusercontent.com/digitalArtHistory/recits-numeriques/main/27/artRimouski.geojson" title="Art Public Rimouski" active/> 
```

---

## Notes

[^1] Pour savoir comment exporter un CSV ou un TSV depuis Microsoft Excel : https://support.microsoft.com/fr-fr/office/importer-ou-exporter-des-fichiers-texte-txt-ou-csv-5250ac4c-663c-47ce-937b-339e391393ba