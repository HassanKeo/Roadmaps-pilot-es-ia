# MÉTHODE D’APPRENTISSAGE PILOTÉE (MAP)

*Objectif : Utiliser l'IA comme levier de productivité et tuteur socratique, sans jamais lui déléguer sa propre réflexion logique.*

---

## PHASE 1 : LE CADRAGE INTELLECTUEL & CARTOGRAPHIE (Clavier interdit)

*But : Savoir où l'on va et de quels outils on a besoin avant de poser la première ligne de code.*

### Étape 1.1 : L'Analyse du Brief

- Prends l'énoncé du projet sur `roadmap.sh`.
- Identifie manuellement (sur papier ou bloc-notes) :
    - **Les entrées (Inputs) :** Qu'est-ce que le système reçoit ? (Une commande CLI, une requête HTTP, un fichier JSON ?)
    - **Les sorties (Outputs) :** Qu'est-ce que le système doit produire ? (Un message de succès, une modification de fichier, un statut HTTP ?)

### Étape 1.2 : Le Prompt de Cartographie Technique

Ouvre ton IA et envoie **strictement** ce prompt (à adapter avec le nom du projet) :

> *"Je vais coder le projet [Nom du Projet] de roadmap.sh en JavaScript Vanilla pour le backend. Avant de me donner l'architecture, je veux que tu dresses la **liste des compétences techniques et des concepts clés** nécessaires pour réaliser ce projet.*
> 
> 
> *Divise cette liste en :*
> 
> *1. **Concepts JavaScript fondamentaux** (ex: l'asynchronisme, la manipulation des tableaux, les modules ES...).*
> 
> *2. **Concepts Réseau / Backend** (ex: les codes de statut HTTP, la gestion des fichiers FS, les en-têtes...).*
> 
> *3. **Concepts optionnels (Front/Outils)** si pertinents.*
> 
> *Consigne : Ne me donne aucun code, juste la liste des concepts sous forme de feuille de route pour que je puisse les réviser avant d'attaquer."*
> 

### Étape 1.3 : Le Check-point des Connaissances

Face à la liste générée par l'IA, applique le tri des trois filtres :

- **Filtre Vert (Je maîtrise) :** Tu connais le concept et sa syntaxe. Tu passes.
- **Filtre Orange (Flou) :** Tu as déjà vu, mais tu as un doute. Demande à l'IA : *"Fais-moi un mini-cours théorique de 3 paragraphes sur [Concept] avec un exemple minimaliste qui n'a rien à voir avec le projet."*
- **Filtre Rouge (Inconnu complet) :** Tu ne démarres pas le projet. Tu passes 30 à 60 minutes à te documenter (MDN Web Docs ou cours IA) pour comprendre la théorie de ce concept.

### Étape 1.4 : L'Architecture (Le Squelette)

Demande enfin le plan de construction à l'IA avec ce prompt :

> *"Maintenant que j'ai validé les concepts, propose-moi uniquement une architecture de fichiers propre (le squelette des dossiers/fichiers) et la liste des étapes logiques à implémenter dans l'ordre pour ce projet. Consigne stricte : ZÉRO ligne de code."*
> 
- Sur ton PC, crée l'arborescence des dossiers et des fichiers vides. **Ton squelette est prêt.**

---

## PHASE 2 : LA CONCEPTION LOGIQUE (Mentalité Backend)

*But : Valider la logique humaine avant de la traduire en syntaxe informatique.*

### Étape 2.1 : L'Isolation

- Prends la **première étape logique** de la liste fournie par l'IA (Ex : *Étape 1 : Lire le fichier JSON s'il existe*).

### Étape 2.2 : Le Pseudo-code

- Dans ton fichier de code, ouvre un bloc de commentaires.
- Écris en **français** les étapes logiques exactes que ton programme doit suivre.
- *Exemple :*JavaScript
    
    # 
    
    `// 1. Importer le module de gestion de fichiers (fs).
    // 2. Vérifier si le fichier 'data.json' existe.
    // 3. Si non, afficher un message et créer un fichier vide.
    // 4. Si oui, lire le contenu et le transformer en objet JS.`
    

### Étape 2.3 : La Traque des Cas Limites (*Edge Cases*)

Force ton cerveau à penser comme un attaquant ou un système qui plante. Ajoute à ton pseudo-code :

- *Et si le fichier JSON est vide ou corrompu ?*
- *Et si l'utilisateur envoie une chaîne de caractères au lieu d'un nombre ?*

---

## PHASE 3 : L'IMPLÉMENTATION & LE JUGEMENT (Le combat)

*But : Écrire le code soi-même et utiliser l'IA uniquement comme un débloqueur conceptuel.*

### Étape 3.1 : Le Code "À la main"

- Traduis ton pseudo-code en JavaScript Vanilla. Aide-toi de la documentation pour la syntaxe exacte si besoin.

### Étape 3.2 : La Posture face à l'Erreur (Interdiction de copier-coller)

Si ton code plante ou que tu es bloqué depuis plus de 15 minutes :

- **NE DEMANDE JAMAIS :** *"Corrige mon code"* ou *"Donne-moi la solution"*.
- **TU DOIS PROMPTER :**
    
    > *"Voici mon code pour l'étape X : [insère ton code]. J'obtiens l'erreur suivante : [insère l'erreur]. Ne me donne pas le code corrigé. Explique-moi la faille logique ou le concept que je maîtrise mal ici pour que je puisse corriger moi-même."*
    > 

### Étape 3.3 : L'Assimilation Active

- Une fois que l'IA t'a expliqué ton erreur, **tape le code de correction toi-même**. N'utilise pas le clic droit "Copier". Forcer tes doigts à taper la syntaxe fixe la mémoire kinésthésique.

---

## PHASE 4 : LA REVUE DE CODE & REFACTORING (La règle du 10 pour 1)

*But : Passer du code "qui marche" au code de "niveau professionnel".*

### Étape 4.1 : La Soumission

Une fois que ton étape (ou ton projet) fonctionne parfaitement, donne le code à l'IA et dis-lui :

> *"Voici mon code fonctionnel pour cette étape : [insère le code]. Analyse-le comme un Lead Developer Senior et trouve-moi :*
> 
> 
> *1. Les failles de sécurité ou de robustesse.*
> 
> *2. Les problèmes de performance ou de complexité algorithmique (Big O Notation).*
> 
> *3. Comment rendre ce code plus propre (Clean Code/Lisibilité)."*
> 

### Étape 4.2 : L'Application de la Règle du "10 pour 1"

- Si l'IA te propose une version optimisée (qui fait par exemple 5 lignes au lieu de tes 15 lignes de code) :
    - **Tu passes 10 fois plus de temps à analyser sa proposition** que le temps qu'il lui a fallu pour la générer.
    - Décortique chaque méthode inconnue. Demande-lui : *"Pourquoi cette méthode est plus performante en mémoire ici ?"*.
    - Si tu es capable d'expliquer la proposition de l'IA à voix haute à un enfant de 10 ans, **alors et seulement alors**, tu as le droit de réécrire ton code en t'en inspirant.

---

## LE RITUEL PARALLÈLE : LA MUSCULATION LOGIQUE (30 min / jour)

*En dehors des projets, pour briller en entretien de Live Coding.*

- **Quand :** Chaque matin ou avant de démarrer ta session projet.
- **Où :** LeetCode ou Codewars (Focus niveau *Easy / Débutant* pour commencer).
- **Règle d'or :** Pas d'IA du tout pendant les 20 premières minutes de recherche sur le problème d'algo. L'IA n'intervient que pour donner un indice (*"Donne-moi une piste sur la structure de données idéale pour résoudre ça"*), jamais le code de la solution.

---

Cette méthode est lente au début, elle demande de la discipline, mais c'est la seule qui fera de toi un développeur backend recherché, capable de piloter n'importe quelle IA du marché plutôt que de te faire remplacer par elle.
