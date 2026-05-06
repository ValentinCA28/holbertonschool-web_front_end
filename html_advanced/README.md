# HTML Advanced

![HTML](https://img.shields.io/badge/Language-HTML5-E34F26.svg?logo=html5&logoColor=white)
![Semantic](https://img.shields.io/badge/Concept-Semantic%20HTML-orange.svg)
![Holberton](https://img.shields.io/badge/School-Holberton-red.svg)

> Construction progressive d'une page web pour le site "Techium" en HTML5 semantique, de la structure de base jusqu'a une page complete avec navigation, sections, liens, listes, tableaux et styleguide.

---

## Objectifs d'apprentissage

- Comprendre la structure de base d'un document HTML5 (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`)
- Utiliser les balises semantiques HTML5 (`<header>`, `<main>`, `<footer>`, `<section>`, `<article>`, `<nav>`, `<aside>`)
- Structurer une page avec des headings hierarchiques (`<h1>` a `<h6>`)
- Ajouter des meta-donnees (`charset`, `viewport`, `description`, `favicon`)
- Integrer des paragraphes, des liens, des listes et des tableaux
- Utiliser les balises `<div>` et `<span>` pour le regroupement d'elements
- Maitriser les commentaires HTML
- Creer un styleguide HTML complet (headings, paragraphes, listes, blockquotes, tableaux, details)

---

## Stack technique

| Outil | Version | Role | Installation |
|-------|---------|------|-------------|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) | 5 | Langage de balisage | Natif dans tout navigateur |

---

## Taches

### 0. Create your first webpage
> **Objectif** : Creer la structure minimale d'un document HTML5 avec `DOCTYPE` et balise `<html>`

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
</html>
<!-- Structure minimale avec declaration DOCTYPE et attributs lang/dir -->
```

### 1. Structure of your webpage
> **Objectif** : Ajouter les elements `<head>` et `<body>` a la structure HTML

```html
<html lang="en" dir="ltr">
    <head></head>
    <body></body>
</html>
<!-- Separation entre metadonnees (head) et contenu visible (body) -->
```

### 2. The head - meta charset, viewport, title, description, favicons
> **Objectif** : Configurer les meta-donnees essentielles du document (charset, viewport, title, description, favicon)

```html
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <title>Homepage - Techium</title>
    <meta name="description" content="Techium is a digital agency">
    <link rel="icon" type="image/x-icon" href="./favicon.ico">
    <link rel="icon" type="image/png" href="./favicon.png">
</head>
<!-- Metadonnees indispensables pour le SEO et le responsive -->
```

### 3. The body - header, main, footer
> **Objectif** : Structurer le body avec les 3 landmarks semantiques principaux

```html
<body>
    <header>Header</header>
    <main>Main content</main>
    <footer>Footer</footer>
</body>
<!-- Utilisation des balises semantiques pour la structure principale -->
```

### 4. Aside (article.html)
> **Objectif** : Utiliser la balise `<aside>` pour du contenu complementaire dans un article

```html
<main>Main content<aside>Aside</aside></main>
<!-- La balise aside contient du contenu tangentiel au contenu principal -->
```

### 5. Sections
> **Objectif** : Decomposer le contenu principal en sections thematiques

```html
<main>
    <section>Hero section</section>
    <section>Services section</section>
    <section>Works section</section>
    <section>About section</section>
    <section>Latest news section</section>
    <section>Testimonials section</section>
    <section>Contact section</section>
</main>
<!-- 7 sections thematiques pour organiser la page d'accueil -->
```

### 6. Work, News, Testimonial articles
> **Objectif** : Imbriquer des `<article>` dans les sections Works, Latest news et Testimonials

```html
<section>Works section
    <article>Work 1</article>
    <article>Work 2</article>
    <article>Work 3</article>
</section>
<!-- Les articles representent des contenus autonomes et redistribuables -->
```

### 7. Navigation
> **Objectif** : Ajouter une balise `<nav>` dans le header pour la navigation du site

```html
<header>
    <nav></nav>
</header>
<!-- La balise nav delimite les liens de navigation principaux -->
```

### 8. Level 1 heading
> **Objectif** : Ajouter le heading principal `<h1>` de la page

```html
<main>
    <h1>Homepage</h1>
    ...
</main>
<!-- Un seul h1 par page pour la hierarchie semantique et le SEO -->
```

### 9. Level 2 headings
> **Objectif** : Ajouter les headings `<h2>` pour titrer chaque section

```html
<section>
    <h2>We help you build your brand!</h2>
</section>
<section>
    <h2>Services</h2>
</section>
<!-- Chaque section recoit un titre de niveau 2 -->
```

### 10. Level 3 headings
> **Objectif** : Ajouter les headings `<h3>` pour les sous-elements (services, works, articles, about)

```html
<h3>Design & Concept</h3>
<h3>Digital Strategy</h3>
<h3>Content Strategy</h3>
<h3>UX Design</h3>
<h3>Web Development</h3>
<h3>Social Media</h3>
<!-- Hierarchie complete h1 > h2 > h3 pour la structure du document -->
```

### 11. Styleguide - Headings
> **Objectif** : Creer une page styleguide affichant tous les niveaux de headings (h1 a h6)

```html
<section>
    <header><h2>Headings</h2></header>
    <h1>Heading level 1</h1>
    <h2>Heading level 2</h2>
    ...
    <h6>Heading level 6</h6>
</section>
<!-- Reference visuelle de tous les niveaux de titres -->
```

### 12. Paragraphs
> **Objectif** : Ajouter des paragraphes `<p>` de contenu dans chaque section

```html
<section>
    <h2>Services</h2>
    <p>We work with you</p>
    ...
</section>
<!-- Les paragraphes apportent le contenu textuel aux sections -->
```

### 13. Styleguide - Paragraphs
> **Objectif** : Ajouter une section paragraphe au styleguide avec sous-titre et texte

```html
<section>
    <header><h2>Paragraph</h2></header>
    <h2>Heading with a subtitle</h2>
    <p>This is my subtitle</p>
    <p>Nunc lacinia ante nunc ac lobortis...</p>
</section>
<!-- Reference visuelle pour les paragraphes et sous-titres -->
```

### 14. Span
> **Objectif** : Utiliser `<span>` pour le nom de la marque dans le header

```html
<header>
    <span>Techium</span>
    <nav></nav>
</header>
<!-- Le span permet de cibler le texte du logo pour le styliser en CSS -->
```

### 15. Div
> **Objectif** : Envelopper les contenus de chaque section dans des `<div>` conteneurs

```html
<section>
    <div>
        <h2>We help you build your brand!</h2>
    </div>
</section>
<!-- Les div servent de conteneurs generiques pour le layout CSS -->
```

### 16. Structure your sections (header inside sections)
> **Objectif** : Ajouter des `<header>` internes aux sections pour regrouper titre et tagline

```html
<section>
    <div>
        <header>
            <h2>Services</h2>
            <p>We work with you</p>
        </header>
        <div>...</div>
    </div>
</section>
<!-- Le header interne regroupe le titre et le sous-titre de chaque section -->
```

### 17. Comments
> **Objectif** : Ajouter des commentaires HTML pour identifier chaque section du code

```html
<!-- Header -->
<header>...</header>
<!-- Main -->
<main>
    <!-- Hero section -->
    <!-- Services section -->
    ...
</main>
<!-- Footer -->
<!-- Les commentaires ameliorent la lisibilite du code source -->
```

### 18. Link your logo
> **Objectif** : Transformer le logo Techium en lien vers la page d'accueil

```html
<div><a href="/"><span>Techium</span></a></div>
<!-- Le logo est cliquable et redirige vers la racine du site -->
```

### 19. (pas de fichier 19)

### 20. Create new pages (about, latest_news, contact)
> **Objectif** : Creer les pages secondaires About, Latest news et Contact avec la meme structure

```html
<!-- about.html -->
<title>About - Techium</title>
<!-- contact.html -->
<title>Contact - Techium</title>
<!-- latest_news.html -->
<title>Latest news - Techium</title>
<!-- Pages secondaires avec header, nav vide et footer identiques -->
```

### 21. Add links in navigation
> **Objectif** : Remplir la navigation avec des liens ancres vers chaque section

```html
<nav>
    <a href="/">Home</a>
    <a href="#services">Services</a>
    <a href="#works">Works</a>
    <a href="#about">About</a>
    <a href="#latest_news">Latest news</a>
    <a href="#testimonials">Testimonials</a>
    <a href="#contact">Contact</a>
</nav>
<!-- Navigation interne avec liens ancres vers les sections -->
```

### 22. Social links in footer
> **Objectif** : Ajouter les liens vers les reseaux sociaux dans le footer

```html
<footer>
    <div>
        <a href="https://www.facebook.com/HolbertonSchool/">Facebook</a>
        <a href="https://twitter.com/holbertonschool">Twitter</a>
        <a href="https://www.instagram.com/holbertonschool/">Instagram</a>
    </div>
</footer>
<!-- Liens externes vers les profils sociaux de l'entreprise -->
```

### 23. Call to action links
> **Objectif** : Ajouter des liens d'action ("Get started", "Learn more about us", "Get in touch")

```html
<a href="#">Get started</a>
<a href="about.html">Learn more about us</a>
<a href="contact.html">Get in touch</a>
<!-- Les CTA (Call-to-Action) guident l'utilisateur vers les actions cles -->
```

### 24. Links within sections
> **Objectif** : Transformer les titres de services, works et articles en liens cliquables

```html
<h3><a href="#">Design & Concept</a></h3>
<h3><a href="#">Interior Design</a></h3>
<h3><a href="#">Hoc loco tenere se Triarius non potuit.</a></h3>
<!-- Chaque element de carte devient un lien interactif -->
```

### 25. List - Navigation
> **Objectif** : Structurer la navigation et le footer avec des listes `<ul>`/`<li>`

```html
<nav>
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="#services">Services</a></li>
        ...
    </ul>
</nav>
<!-- Les listes apportent une semantique correcte a la navigation -->
```

### 26. Styleguide - Lists
> **Objectif** : Ajouter au styleguide les 3 types de listes (ul, ol, dl)

```html
<h3>Unordered</h3>
<ul><li>Dolor pulvinar etiam magna etiam.</li>...</ul>
<h3>Ordered</h3>
<ol><li>Dolor pulvinar etiam magna etiam.</li>...</ol>
<h3>Definition</h3>
<dl><dt>Startup</dt><dd>A startup company or startup is...</dd></dl>
<!-- Reference des listes non ordonnees, ordonnees et de definition -->
```

### 27. Separate content
> **Objectif** : Ajouter du contenu supplementaire et poursuivre la structuration de la page

```html
<!-- Continuation de la page index avec contenu additionnel -->
<!-- Footer avec liens legaux (Terms of Use, Privacy Policy, Cookie Policy) -->
```

### 28. Styleguide - Horizontal rule
> **Objectif** : Ajouter la balise `<hr>` au styleguide comme separateur visuel

```html
<section>
    <header><h2>Horizontal rule</h2></header>
    <div><hr></div>
</section>
<!-- La balise hr cree une separation thematique entre les sections -->
```

### 29. Clients testimonials with blockquote
> **Objectif** : Enrichir la section testimonials avec de vrais temoignages et citations

```html
<!-- Integration de citations et temoignages dans la page principale -->
```

### 30. Styleguide - Blockquotes
> **Objectif** : Ajouter les citations inline (`<q>`) et en bloc (`<blockquote>`) au styleguide

```html
<h3>Inline quote</h3>
<q>Stay hungry. Stay foolish.</q>
<h3>Blockquote</h3>
<blockquote>
    <p>I will be the leader of a company...</p>
    <cite>Kanye West, Musician</cite>
</blockquote>
<!-- Les balises q et blockquote pour les citations courtes et longues -->
```

### 31. Author quote
> **Objectif** : Ajouter l'attribution d'auteur dans les articles et temoignages

```html
<!-- Ajout des auteurs et citations dans les articles de la page -->
```

### 32. Styleguide - Typography
> **Objectif** : Ajouter au styleguide les elements typographiques (`<address>`, `<pre>`, `<code>`, `<mark>`)

```html
<address>320 Stewart Avenue, Unit 12<br>New York City NY 10001</address>
<pre><code>
    <h2>My title</h2>
    <p>Proin lacus turpis...</p>
</code></pre>
<p>Curabitur sit amet <mark>highlighted</mark> turpis...</p>
<!-- Elements de typographie avancee : adresse, code, surlignage -->
```

### 33. Styleguide - Table
> **Objectif** : Creer un tableau HTML semantique avec `<thead>`, `<tbody>`, `<th>`, `<caption>`

```html
<table>
    <caption>Star Wars Trilogy Data</caption>
    <thead>
        <tr>
            <th scope="col">Title</th>
            <th scope="col">Director</th>
            <th scope="col">Release Date</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">Star Wars: Episode IV - A New Hope</th>
            <td>George Lucas</td>
            <td>May 25th, 1977</td>
        </tr>
        ...
    </tbody>
</table>
<!-- Tableau accessible avec scope pour les lecteurs d'ecran -->
```

### 34. Styleguide - Details
> **Objectif** : Utiliser `<details>` et `<summary>` pour du contenu repliable interactif

```html
<details>
    <summary>Show/Hide me</summary>
    <p>Pellentesque habitant morbi tristique...</p>
</details>
<details open>
    <summary>Always open</summary>
    <p>Pellentesque habitant morbi tristique...</p>
</details>
<!-- L'element details cree un widget interactif sans JavaScript -->
```

---

## Auteur

- **Valentin Planchon**

---

<div align="center">

![Holberton School](https://img.shields.io/badge/HOLBERTON%20SCHOOL-HTML%20Advanced-white?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTE0LjY2NyA4QzE0LjY2NyA0LjY4NiAxMi4zMTQgMi4zMzMzIDkgMi4zMzMzQzUuNjg2NyAyLjMzMzMgMy4zMzMzIDQuNjg2IDMuMzMzIDhDMi4xNDYgOCAyIDguMTQ2IDAgOEMwIDEyLjMxNCAyLjM1NCAxNC42NjcgNi42NjcgMTQuNjY3QzYuNjY3IDE1LjE4NiA2LjkzMyAxNS41MzMgNy4zMzMzIDE1Ljc4N0M3LjczMzMgMTYuMDMzIDguMTMzMyAxNi4xNiA4LjY2NjcgMTYuMTYgOS4yIDkuNTMzMyAxMC4xMzMgMTYuMTYgMTAuNjY3IDE2LjE2QzExLjIgMTYuMTYgMTEuNiAxNi4wMzMgMTIuMDY3IDE1Ljc4N0MxMi41MzMgMTUuNTMzIDEyLjggMTUuMTg2IDEyLjggMTQuNjY3QzE0LjY2NyAxNC42NjcgMTQuNjY3IDguNjY3IDE0LjY2NyA4WiIgZmlsbD0iI0ZGRkZGRiIvPgo8L3N2Zz4K&labelColor=c41e3a&color=36393f) <img src="../images/holberton_logo.png" alt="Holberton Logo" width="34">

[Retour au projet principal](../)

</div>
