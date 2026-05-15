# PARADIGME POUR PRATIQUER MES PROJETS FRONTEND

Pour le Frontend, l'objectif est radicalement différent du Backend : tu ne cherches pas à devenir un artiste du pixel, tu cherches à comprendre comment structurer une interface propre et comment la lier à de la logique.

Voici la **MÉTHODE MAP - VERSION FRONTEND**. Elle est optimisée pour te faire gagner du temps sur l'esthétique tout en te forçant à maîtriser la structure (HTML) et l'accessibilité.

---

# MÉTHODE D’APPRENTISSAGE PILOTÉE (MAP) — SPÉCIAL FRONTEND

*Objectif : Maîtriser la structure sémantique et l'agencement, tout en déléguant le design purement visuel (couleurs, fioritures) à l'IA.*

---

## PHASE 1 : LE CADRAGE STRUCTURAL (Zéro CSS pour l'instant)

*But : Penser en squelette de page avant de penser aux couleurs. Le backend a besoin de structures claires.*

### Étape 1.1 : L'Analyse de la Maquette / Du Projet

- Regarde l'exercice ou l'image du projet proposé par `roadmap.sh`.
- Découpe visuellement la page en grands blocs. Identifie : l'en-tête, la navigation, le contenu principal, les articles, le pied de page.

### Étape 1.2 : Le Prompt de Cartographie Sémantique

Ouvre ton IA et demande-lui de lister les outils structurels avec ce prompt :

> *"Je dois coder le projet Front [Nom du Projet] de roadmap.sh. Consigne stricte : ne me donne aucun code CSS. Donne-moi la liste des **balises HTML sémantiques** obligatoires pour ce projet (ex: `<main>`, `<article>`, `<nav>`, `<form>`, les attributs d'accessibilité `aria`). Donne-moi aussi la liste des concepts d'agencement CSS (ex: Flexbox, Grid) indispensables pour aligner ces éléments."*
> 

### Étape 1.3 : Le Check-point HTML

- Si les balises suggérées te sont inconnues : demande à l'IA pourquoi elles sont préférées à de simples `<div>`. Un bon dev backend sait qu'un HTML sémantique est crucial pour le SEO et l'accessibilité.

---

## PHASE 2 : LA CONSTRUCTION DU SQUELETTE (Le HTML Pur)

*But : Écrire un code HTML parfait sans aucune feuille de style.*

### Étape 2.1 : L'Écriture à la main

- Crée ton fichier `index.html`.
- Code toute la structure de la page **uniquement en HTML**.
- **Ta contrainte :** À la fin de cette étape, ta page doit être moche, noire et blanche, avec les éléments les uns en dessous des autres, mais **parfaitement lisible et structurée**.

---

## PHASE 3 : L'AGENCEMENT GLOBAL (Le CSS Structurel)

*But : Placer les éléments au bon endroit (gauche, droite, grille) par toi-même.*

### Étape 3.1 : Le Code à la main pour le Layout

- Crée ton fichier `style.css`.
- Gère **toi-même** l'alignement des gros blocs en utilisant **Flexbox** ou **CSS Grid**.
- Tu dois être capable de centrer un élément ou de mettre deux colonnes côte à côte sans aide.

### Étape 3.2 : Le S.O.S à l'IA si le Layout casse

Si ta grille explose ou que tes éléments se chevauchent :

- **Prompt :** *"Voici mon HTML [insère le code] et mon CSS d'agencement [insère le code]. Mes colonnes ne s'alignent pas. Ne me donne pas tout le CSS corrigé, explique-moi quelle propriété de Flexbox/Grid j'ai mal configurée."*

---

## PHASE 4 : LA DÉLÉGATION VISUELLE (Le "Design" par l'IA)

*But : C'est ici que tu gagnes du temps. Tu laisses l'IA faire le travail d'esclave visuel.*

### Étape 4.1 : Le Prompt de Peinture

Une fois que tes blocs sont placés au bon endroit, tu peux demander à l'IA de générer le style purement cosmétique (couleurs, arrondis, ombres, polices, dégradés).

- **Prompt :** *"Mon agencement est prêt. Génère-moi uniquement le code CSS cosmétique pour styliser les boutons, ajouter des ombres portées douces, des arrondis de coins (`border-radius`) modernes, et une palette de couleurs [ex: sombre / pastel]. Applique cela via des classes claires."*

### Étape 4.2 : La Règle du "10 pour 1" Visuelle (Allégée)

- Quand l'IA te donne ce CSS cosmétique, ne cherche pas à intellectualiser pendant des heures pourquoi elle a mis `#f3f4f6` plutôt qu'un autre gris.
- **Cependant**, vérifie la propreté : assure-toi qu'elle n'a pas pollué ton code avec des propriétés inutiles ou des `!important` partout. Si tu vois une propriété bizarre (ex: `transform`, `transition`), demande-lui une explication rapide.

---

## LE RITUEL PARALLÈLE : ADAPTATION INTERFACES

- **Ton focus :** Entraîne-toi particulièrement sur les **Formulaires HTML** (`<form>`, `<input>`, `<button>`). Pourquoi ? Parce qu'en tant que futur dev Backend, ta principale interaction avec le Front se fera via des formulaires qui envoient des données à ton serveur. Tu dois savoir comment récupérer ces données proprement.

Cette méthode te permet de boucler un projet Front trois fois plus vite qu'un étudiant classique, car tu ne perds pas ton temps sur le design, tout en développant une rigueur de fer sur la structure.
