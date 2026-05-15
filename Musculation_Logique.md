# GUIDE DE MUSCULATION LOGIQUE (GML)

*Objectif : Développer une rigueur algorithmique en JavaScript Vanilla et réussir les tests techniques d'embauche.*

---

## 1. LE CADRE D'ENTRAÎNEMENT (La Routine)

- **Fréquence :** 5 jours par semaine (du lundi au vendredi, idéalement le matin au réveil pour avoir le cerveau frais).
- **Durée :** 30 à 45 minutes maximum. Si tu ne trouves pas la solution dans ce laps de temps, tu t'arrêtes (voir Phase 3).
- **Plateformes :** Crée un compte sur **Codewars** (vise le niveau *8kyu* puis *7kyu* pour commencer) ou **LeetCode** (niveau *Easy* uniquement).

---

## 2. LES 4 PHASES DE LA RÉSOLUTION (Face au problème)

### Phase 2.1 : L'Analyse à blanc (10 minutes — IA interdite)

Lis l'énoncé du problème d'algo. Prends une feuille et un stylo (ou un fichier texte sur ton Zorin OS).

1. **Isole les types de données :** Qu'est-ce qu'on te donne ? (Un tableau de chaînes ? Un objet ? Un entier ?). Qu'est-ce que tu dois renvoyer ? (Un booléen ? Un tableau trié ?).
2. **Fais le test manuellement :** Prends l'exemple fourni par le site et résous-le "à la main" sur ton papier. Écris le cheminement que ton cerveau a pris.
3. **Traque les cas tordus (*Edge Cases*) :** Que doit faire ton code si l'entrée est un tableau vide `[]` ? Si on te donne un nombre négatif ? Si la chaîne est vide `""` ?

### Phase 2.2 : Le Pseudo-code (5 minutes — IA interdite)

Traduis ton raisonnement papier en étapes logiques en français directement dans l'éditeur du site (sous forme de commentaires).

- *Exemple :*JavaScript
    
    # 
    
    `// 1. Boucler sur le tableau du début à la fin
    // 2. Si l'élément actuel est égal à l'élément recherché, stocker son index
    // 3. Si la boucle se termine sans rien trouver, renvoyer -1`
    

### Phase 2.3 : Le Codage "Brut" (15 minutes — IA interdite)

- Traduis ton pseudo-code en JavaScript Vanilla.
- **Interdiction d'utiliser des fonctions magiques de JS** que tu ne comprends pas à 100%. Reste sur des structures de base (`for`, `while`, `if/else`, manipulation d'index).
- Lance les tests de la plateforme.

---

## 3. COMMENT UTILISER L'IA QUAND ÇA COINCE ?

### Cas A : Tu es bloqué pendant le codage (Après 20 minutes de recherche)

**NE DEMANDE PAS :** *"Donne-moi la solution à ce problème"*.

**PROMPTE l'IA ainsi :**

> *"Je résous le problème d'algo suivant : [Colle l'énoncé]. J'ai écrit ce pseudo-code : [Colle ton pseudo-code] mais je bloque sur sa traduction en JavaScript / sur un bug de logique. Ne me donne aucun code. Donne-moi uniquement **un indice** ou une piste sur la structure de données ou la méthode que je devrais utiliser."*
> 

### Cas B : Tu as réussi à faire passer les tests (Le code fonctionne)

C'est ici que la règle du **10 pour 1** prend tout son sens en algo. Tu donnes ton code réussi à l'IA.

**PROMPTE l'IA ainsi :**

> *"Mon code JavaScript fonctionne pour ce problème : [Colle ton code]. Analyse sa complexité temporelle et spatiale en utilisant la **Notation Big O** (ex: $O(n)$, $O(n^2)$, $O(1)$). Propose-moi ensuite une version plus optimisée et explique-moi ligne par ligne pourquoi elle est plus efficace en termes de performance ou de mémoire."*
> 

---

## 4. LA CHECK-LIST DES FONDAMENTAUX À MAÎTRISER (Dans l'ordre)

Tu dois être capable d'implémenter ces concepts en JavaScript sans transpirer avant d'aller en entretien :

| **Concept / Structure** | **Ce que tu dois savoir faire à la main** | **Pourquoi c'est vital en Backend** |
| --- | --- | --- |
| **Les Tableaux (Arrays)** | Parcourir, inverser, filtrer, et découper un tableau sans utiliser les fonctions natives (juste avec des boucles `for`). | Manipulation brute des listes de données. |
| **Les Hash Maps (Objects/Maps)** | Utiliser un objet JS comme un dictionnaire pour stocker des paires Clé/Valeur et y accéder en temps constant ($O(1)$). | Éviter les boucles imbriquées qui font ramer les serveurs. |
| **Les Chaînes (Strings)** | Inverser une chaîne, compter les occurrences d'une lettre, vérifier les palindromes. | Nettoyage et validation des données d'un formulaire. |
| **La Récursivité** | Écrire une fonction qui s'appelle elle-même (ex: calculer une factorielle ou parcourir un arbre). | Parcourir des dossiers ou des structures de données imbriquées. |

---

## 5. LA POSTURE DU COMMANDO EN ENTRETIEN (Live Coding)

Le jour J, face au recruteur, applique ces trois règles tirées de ce guide :

1. **Parle tout le temps :** Le recruteur se fiche de la solution parfaite. Il veut entendre ta pensée. Dis tout haut : *"Je commence par vérifier si le tableau est vide pour éliminer le cas limite..."*.
2. **N'écris pas de code tout de suite :** Écris d'abord ton pseudo-code sous ses yeux. Cela prouve que tu es structuré.
3. **Assume tes erreurs :** Si le recruteur te dit *"Qu'est-ce qui se passe à la ligne 5 si je passe un 0 ?"*, ne te défends pas. Regarde ton code, fais le calcul mentalement et dis : *"Ah oui, bien vu, ça va créer une division par zéro, je dois ajouter une condition de sécurité"*.

---

Tu as désormais tes trois cartes de route : **MAP Backend**, **MAP Frontend**, et **Guide Algo**. L'arsenal est complet. Tu es armé pour affronter n'importe quel projet de roadmap.sh.
