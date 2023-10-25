# Les animations avec css

Un super article sur les animations css :
https://la-cascade.io/articles/css-animation-une-introduction

## Deux notions importantes

### Les keyframes

Les keyframes permettent de définir des étapes dans une animation.

```css
@keyframes my-animation {
    0% {
        background-color: red;
    }
    50% {
        background-color: blue;
    }
    100% {
        background-color: green;
    }
}
```

### L'animation

L'animation permet de définir une animation sur un élément.

```css
.my-element {
    animation: my-animation 1s linear infinite;
}
```

### Plein de possibilités

Vous allez pouvoir jouer sur plein de propriétés pour créer des animations.
- toutes les transformations sont possibles : translate, rotate, scale, skew, etc.
- toutes les propriétés css sont animables : background-color, color, border, etc.

Et gérer plein de paramètres comme :
- la durée
- le nombre de répétitions
- le sens de l'animation
- le délai avant le début de l'animation

Les limites viendront de votre imagination.

# Amusons-nous avec les animations

## Le loader

Cela peut sembler très compliqué mais en réalité, c'est une suite de petites instructions très simples :
- Créer une boite carrée de 50px de côté
- Créer une bordure de 5px de large et blanche 
- Créer une bordure à droite de 5px de large et bleue
- Arrondir les angles de la boite à 50%
- Faire tourner la boite sur elle-même de 360° de manière infinie

## Le spinner

- créer une div avec un moyen de la sélectionner en css
- lui donner une image de spinner : "https://www.pngall.com/wp-content/uploads/14/Loading-PNG-Image-File.png
- la faire tourner de la même manière que le loader

## Le texte qui fait boum boum

- Créer une nouvelle page texte-animated.html
- Créer un lien vers cette page
- Créer une div centrer verticalement et horizontalement
- Ajouter en contenu le mot "Love"
- Lui donner une police de caractère qui vous plait grâce à google font
- Lui donner une taille de police conséquente
- Ajouter une animation qui fait grossir le texte de 100% à 200% puis revient à 100% de manière infinie grâce à la transformation scale
- Ajouter une animation qui fait passer le texte de la couleur rouge à la couleur bleu puis revient à la couleur rouge de manière infinie grâce à la transformation color
- Ajouter une animation quand l'utilisateur passe sa souris sur le texte, qui fait tourner le texte de 360° une seule fois

## Le coeur qui écrit un T pour un certain Thomas

- Créer une nouvelle page heart-animated.html
- Créer un lien vers cette page
- Créer un coeur
    - Créer une div avec une classe heart
    - Créer deux enfants à cette div avec une classe heart__left et heart__right
    - la div parent doit avoir comme style un positionnement relatif, une largeur de 100px et une hauteur de 90px
    - les deux enfants doivent avoir comme style un positionnement absolu, une largeur de 50px et une hauteur de 80px, un fond rouge et un bord arrondi de 50% sur les deux premiers coins et de 0% sur les deux derniers coins
    - le premier enfant (left) doit avoir un positionnement top: 0 et left: 42px
    - le deuxième enfant (right) doit avoir un positionnement top: 0 et left: 20px
    - les deux enfants doivent avoir une rotation de 45° un dans un sens et l'autre dans l'autre sens grâce à la transformation rotate
- Ajouter une animation qui fait grossir le coeur de 100% à 200%, ce dirige vers le haut, puis va à gauche puis à droite, puis revient à sa position initiale en reprenant ensuite sa taille initiale. L'animation sera lancée de manière infinie grâce à la transformation scale et translate.

## Et si on se focalisait sur les tableaux responsive ?

- Créer une nouvelle page table-responsive.html
- Créer un lien vers cette page
- Créer un tableau avec 10 colonnes et 3 lignes
- Gérer le responsive de ce tableau de manière à ce qu'il soit lisible sur mobile en le scrollant horizontalement
- Dupliquer le tableau et le rendre responsive en réduisant le nombre de colloque à 3 sur mobile
- Dupliquer le tableau et le rendre responsive en l'affichant sous forme d'une liste d'éléments sur mobile