# CSS Advanced

![CSS](https://img.shields.io/badge/Language-CSS3-1572B6.svg?logo=css3&logoColor=white)
![HTML](https://img.shields.io/badge/Language-HTML5-E34F26.svg?logo=html5&logoColor=white)
![Custom Properties](https://img.shields.io/badge/Concept-CSS%20Variables-blueviolet.svg)
![Holberton](https://img.shields.io/badge/School-Holberton-red.svg)

> Stylisation CSS3 avancee du site "Techium" en partant de zero : variables CSS, typographie, couleurs, fonts, poids, tailles, line-height, decoration de liens et alignement des sections.

---

## Objectifs d'apprentissage

- Utiliser les CSS Custom Properties (variables) pour un design maintenable et coherent
- Definir et appliquer une palette de couleurs via `:root`
- Configurer la typographie (font-family, font-size, font-weight, line-height)
- Integrer des Google Fonts (Open Sans, Raleway)
- Comprendre la technique `font-size: 62.5%` pour faciliter le calcul en `rem`
- Supprimer les decorations par defaut des liens (`text-decoration: none`)
- Gerer les selecteurs de classes CSS (`.visually-hidden`, `.card-category`, `.section-tagline`, `.section-header`)
- Appliquer un alignement centre aux en-tetes de section

---

## Stack technique

| Outil | Version | Role | Installation |
|-------|---------|------|-------------|
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) | 3 | Langage de style | Natif dans tout navigateur |
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) | 5 | Structure de la page | Natif dans tout navigateur |
| ![Google Fonts](https://img.shields.io/badge/Google%20Fonts-4285F4?logo=googlefonts&logoColor=white) | - | Polices web (Open Sans, Raleway) | Via `<link>` CDN |

---

## Taches

### 1. Smooth scrolling
> **Objectif** : Activer le defilement fluide sur toute la page via la propriete `scroll-behavior`

```css
html {
    scroll-behavior: smooth;
}
/* Active le smooth scrolling pour les ancres internes */
```

### 2. Color variables
> **Objectif** : Definir les couleurs du texte et des liens, masquer les elements et styliser les classes d'accent

```css
body {
    color: #161616;
}
a {
    color: #161616;
}
.visually-hidden {
    display: none;
}
.card-category {
    color: #D73953;
}
.section-tagline {
    color: #D73953;
}
/* Couleurs definies en dur, migrees vers des variables a l'etape suivante */
```

### 3. CSS Custom Properties
> **Objectif** : Migrer les couleurs en CSS custom properties dans `:root` pour centraliser la palette

```css
:root {
    --color-primary: #d73953;
    --color-black: #090909;
    --color-white: #ffffff;
    --color-light-grey: #f3f3f3;
    --color-dark-grey: #353535;
    --text-color: var(--color-black);
}
/* Palette centralisee : un seul endroit pour modifier les couleurs */
```

### 4. Font family
> **Objectif** : Definir les familles de polices par defaut pour le body et les headings

```css
:root {
    --font-family-base: "Helvetica Neue", Helvetica, Arial, sans-serif;
    --font-family-title: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
body {
    font-family: var(--font-family-base);
}
h1, h2, h3, h4, h5, h6 {
    font-family: var(--font-family-title);
}
/* Fallback chain pour garantir un rendu coherent sur tous les OS */
```

### 5. Font size
> **Objectif** : Definir une echelle de tailles typographiques en rem avec la technique 62.5%

```css
:root {
    --font-size-small: 1.2rem;
    --font-size-medium: 1.6rem;
    --font-size-large: 1.8rem;
    --font-size-x-large: 2.3rem;
    --font-size-xx-large: 4.8rem;
}
html {
    font-size: 62.5%;
}
body {
    font-size: var(--font-size-medium);
}
/* 62.5% = 10px base, donc 1.6rem = 16px (calcul simplifie) */
```

### 6. Font weight
> **Objectif** : Definir les poids de police pour le texte courant et les titres

```css
:root {
    --font-weight-regular: 400;
    --font-weight-bold: 700;
}
body {
    font-weight: var(--font-weight-regular);
}
h1, h2, h3, h4, h5, h6 {
    font-weight: var(--font-weight-bold);
}
/* Les titres en bold, le texte courant en regular */
```

### 7. Google Fonts
> **Objectif** : Remplacer les polices par defaut par Open Sans (body) et Raleway (titres)

```css
:root {
    --font-family-base: "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
    --font-family-title: "Raleway", "Helvetica Neue", Helvetica, Arial, sans-serif;
}
/* Les Google Fonts sont chargees via un <link> dans le HTML */
```

### 8. Line height
> **Objectif** : Definir les hauteurs de ligne pour ameliorer la lisibilite du texte

```css
:root {
    --line-height-small: 1.2;
    --line-height-base: 1.5;
    --line-height-big: 1.8;
}
body {
    line-height: var(--line-height-base);
}
/* Un line-height de 1.5 est le standard pour le confort de lecture */
```

### 9. Links decoration
> **Objectif** : Supprimer le soulignement par defaut des liens

```css
a {
    color: var(--text-color);
    text-decoration: none;
}
/* Les liens sont stylises sans soulignement pour un design moderne */
```

### 10. Section header alignment
> **Objectif** : Centrer le texte des en-tetes de section via une variable CSS

```css
:root {
    --section-header-align: center;
}
.section-header {
    text-align: var(--section-header-align);
}
/* L'alignement est centralise via une variable pour faciliter les changements */
```

### 11-32. Fichiers CSS supplementaires (vides)
> **Objectif** : Fichiers prepares pour les taches suivantes du projet (padding, margin, layout, grid, responsive, etc.)

```css
/* Fichiers 11-style.css a 32-style.css */
/* Prepares pour accueillir le layout, les cards, le responsive, etc. */
```

---

## Auteur

- **Valentin Planchon**

---

<div align="center">

![Holberton School](https://img.shields.io/badge/HOLBERTON%20SCHOOL-CSS%20Advanced-white?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTE0LjY2NyA4QzE0LjY2NyA0LjY4NiAxMi4zMTQgMi4zMzMzIDkgMi4zMzMzQzUuNjg2NyAyLjMzMzMgMy4zMzMzIDQuNjg2IDMuMzMzIDhDMi4xNDYgOCAyIDguMTQ2IDAgOEMwIDEyLjMxNCAyLjM1NCAxNC42NjcgNi42NjcgMTQuNjY3QzYuNjY3IDE1LjE4NiA2LjkzMyAxNS41MzMgNy4zMzMzIDE1Ljc4N0M3LjczMzMgMTYuMDMzIDguMTMzMyAxNi4xNiA4LjY2NjcgMTYuMTYgOS4yIDkuNTMzMyAxMC4xMzMgMTYuMTYgMTAuNjY3IDE2LjE2QzExLjIgMTYuMTYgMTEuNiAxNi4wMzMgMTIuMDY3IDE1Ljc4N0MxMi41MzMgMTUuNTMzIDEyLjggMTUuMTg2IDEyLjggMTQuNjY3QzE0LjY2NyAxNC42NjcgMTQuNjY3IDguNjY3IDE0LjY2NyA4WiIgZmlsbD0iI0ZGRkZGRiIvPgo8L3N2Zz4K&labelColor=c41e3a&color=36393f) <img src="../images/holberton_logo.png" alt="Holberton Logo" width="34">

[Retour au projet principal](../)

</div>
