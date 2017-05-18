---
title: Recette
description: Créer une page web au sujet de votre recette préférée, afin que vos amis puissent la suivre !
layout: project
notes: "Recipe - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous allez apprendre à créer une page web pour votre recette préférée.

![capture d'écran](images/recipe-final.png)

# Étape 1: Choisir votre recette { .activity}

Avant de commencer à coder, vous devez choisir votre recette.

## Liste de contrôle d'Activité { .check}

+ Pensez à une recette que vous voulez partager avec vos amis. Ça peut être :
	+ Une recette que vous avez trouvée en ligne;
	+ Votre plat préféré;
	+ Quelque chose que vous avez inventée !

L'exemple que vous retrouvez dans ce projet est pour faire un milk-shake à la banane. Vous pouvez reprendre cette recette si vous ne trouvez pas votre propre recette.

# Étape 2: Ingrédients { .activity}

Créeons une liste des ingrédients nécessaires pour suivre cette recette.

## Liste de contrôle d'Activité { .check}

+ Ouvrir ce modèle trinket : [jumpto.cc/html-template](http://jumpto.cc/html-template).

	Le projet devrait apparaître comme ceci :

	![Capture d'écran](images/recipe-starter.png)

+ Pour votre liste d'ingrédients, vous allez utiliser une __liste non-ordonnée__, en utilisant la balise `<ul>`. Allez à la ligne 8 du modèle et ajouter le HTML, en remplaçant le texte dans le titre `<h1>` avec le nom de votre propre recette :

```
<h1>Milk-shake à la banane</h1>

<h3>Ingrédients:</h3>

<ul>

</ul>
```

+ Visualisez votre page web, et vous devrez voir les deux titres.

![Capture d'écran](images/recipe-headings.png)

Vous ne voyez pas de liste encore, car vous n'avez pas ajouté d'éléments à votre liste !

+ La prochaine étape est d'ajouter des éléments à votre liste, en utilisant la balise `<li>`. Ajoutez le code suivant à l'intérieur de votre balise `<ul>` :

```
<li>1 banane</li>
```
![Capture d'écran](images/recipe-ul.png)

Puisque votre liste est de type "non-ordonnée", il n'y a pas de numéro à coté de chaque élément, plutôt des points.

## Défi : Plus d'ingrédients {.challenge}
Pouvez-vous ajouter tous les ingrédients de __votre__ recette ?

Votre page web devrait ressembler à ceci :

![Capture d'écran](images/recipe-more-ingredients.png)

## Sauvegarder votre projet {.save}

# Étape 3: Mode d'emploi { .activity }

Ensuite, expliquons comment faire votre recette.

## Liste de contrôle d'Activité { .check}

+ Vous allez utiliser une autre liste pour écrire votre méthode, mais cette fois-ci vous allez utiliser une __list ordonnée__, en employant la balise `<ol>`.

Une liste ordonnée est une liste numérotée, que vous devrez utiliser quand l'ordre des étapes est indispensable.

Ajouter le code suivant en-dessous de la liste des ingrédients, en s'assurant que c'est toujours à l'intérieur des balises `<body>` :

```
<h3>Mode d'emploi</h3>

<ol>

</ol>
```

![Capture d'écran](images/recipe-method.png)

+ Maintenant vous avez juste à ajouter des éléments à votre nouvelle liste ordonnée :

```
<li>Ôter la peau et mettre la banane dans le mixer</li>
```

![Capture d'écran](images/recipe-ol.png)

Remarquer comment les éléments de la liste sont numérotés de façon automatique !

## Défi : D'autres étapes {.challenge}
Pouvez-vous ajouter toutes les étapes pour faire __votre__ recette ?

Votre méthode devrait ressembler à ceci :

![Capture d'écran](images/recipe-more-method.png)

## Sauvegarder votre projet {.save}

# Étape 4: Des Couleurs ! { .activity}

Ajoutons des couleurs à notre page de recette.

## Liste de contrôle d'Activité { .check}

+ Vous avez déjà appris comment ajouter du texte de couleur dans une page web. Ajouter le code suivant dans votre fichier `style.css`, afin de transformer en bleu tout le text du corp du site en bleu :

```
body {
    color: blue;
}
```

![Capture d'écran](images/recipe-blue.png)

+ Votre navigateur connait des couleurs comme `blue` (*bleu*), `yellow` (*jaune*) et même `lightgreen` (*vert clair*), mais saviez-vous que votre navigateur connait les __noms__ de plus de 500 couleurs différentes ?

Il y a une liste de tous les noms des couleurs que vous pouvez utiliser : [jumpto.cc/colours](http://jumpto.cc/colours), y compris des noms comme `tomato`, `firebrick` et `peachpuff`.

Changer la couleur du texte de `blue` en `tomato`.

![Capture d'écran](images/recipe-tomato.png)

+ Votre navigateur connait les noms de 140 couleurs, mais en réalité connait les __valeurs de couleur__ de plus de 16 millions de couleurs !


Pour dire au navigateur la couleur à afficher, vous avez besoin simplement de lui indiquer combien de rouge, vert et bleu à utiliser.

Les quantités de rouge, vert et bleu sont écrites comme des chiffres entre `0` et `255`.

![Capture d'écran](images/recipe-rgb-img.png)

Ajouter le code suivant au fichier CSS pour le corp de la page web, pour afficher un fond jaune clair :

```
background: rgb(250,250,210);
```

![Capture d'écran](images/recipe-rgb.png)

+ Si vous préférez, vous pouvez dire au navigateur quelle couleur afficher en utilisant un code hexadécimal (ou __code hex__). Ça fonctionne presque de la même façon que le code `rgb()` ci-dessus, sauf que les codes hex commencent toujours avec un `#`, et utilisent des ‘nombres’ hexadécimaux entre `00` et `ff` pour la quantité de rouge, vert et bleu.

![Capture d'écran](images/recipe-hex-img.png)

Remplacer le code `rgb()` dans votre CSS avec le code hex suivant :

```
background: #fafad2;
```

![Capture d'écran](images/recipe-hex.png)

Vous devriez voir la même couleur jaune clair qu'avant !

## Sauvegarder votre projet {.save}

# Étape 5: Dernières retouches  { .activity}

Ajoutons un peu plus de HTML et CSS afin d'améliorer votre page web.

## Liste de contrôle d'Activité { .check}

+ Vous pouvez ajouter une ligne horizontale à la fin de votre recette, en utilisant la balise <hr>.

![Capture d'écran](images/recipe-hr.png)

À noter que cette balise n'a pas besoin d'une balise de clôture, tout comme la balise `<img>`.

+ La ligne que vous venez d'ajouter n'est pas dans le même style que le reste de votre page web. Nous pouvons régler ça en ajoutant du code CSS :

```
hr {
    height: 2px;
    border: none;
    background-color: tomato;
}
```

![Capture d'écran](images/recipe-hr-css.png)

+ Vous pouvez même changer le style de vos puces avec ce code CSS :

```
ul {
    list-style-type: square;
}
```

![Capture d'écran](images/recipe-ul-css.png)

## Défi : Plus de couleurs ! {.challenge}
Changer les couleurs dans votre code utilisant les noms, valeurs `rgb()` et code hex. Il y a une liste avec beaucoup de couleurs disponible via <a href="http://jumpto.cc/colours" target="_blank">jumpto.cc/colours</a>, ou vous pouvez aller à <a href="http://jumpto.cc/colour-picker" target="_blank">jumpto.cc/colour-picker</a> et créer vos propres couleurs !

Voici quelques exemples de couleurs :

+ Rouge peut être écrit comme : :
	+ `red`
	+ `rgb(255,0,0)` (plein de rouge, pas de vert et pas de bleu)
	+ `#ff0000`

+ Olive peut être écrit comme :
	+ `olive`
	+ `rgb(128, 128, 0)` (un peu de rouge et vert, et pas de bleu)
	+ `#808000`

Essayer de vous assurer que les couleurs que vous utilisez correspondent à votre recette !

## Sauvegarder votre projet {.save}

## Défi : Avis {.challenge}
Demandez à quelques amis de laisser leurs avis sur votre recette. Vous aurez besoin de créer une autre liste pour le faire.

![Capture d'écran](images/recipe-reviews.png)

## Sauvegarder votre projet {.save}

## Défi : Plus de styles {.challenge}
Pouvez-vous insérer une image dans votre page web ? Ou changer la police ? Voilà à quoi votre page pourrait ressembler :

![Capture d'écran](images/recipe-final.png)

Voici un peu de code qui vous aidera :

```
font-family: Arial / Comic Sans MS / Courier / Impact / Tahoma;
font-size: 12pt;
font-weight: bold;

<img src="insérer-lien-vers-image-ici">
```

## Sauvegarder votre projet {.save}
