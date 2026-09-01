# JavaScript — Challenges sur les Boucles

## Boucles `for` et `while`

> **Règle générale :**
>
> Ces challenges doivent être réalisés **sans utiliser de tableaux**.
>
> L'objectif est de maîtriser les boucles, les compteurs, les accumulateurs et les conditions.

### Interdit

* Tableaux `[]`
* Objets
* `forEach()`
* `map()`
* `filter()`
* `reduce()`
* Fonctions personnalisées
* Bibliothèques externes
* Fonctions `Math.*`
* Utiliser une chaîne de caractères comme tableau
* Copier manuellement plusieurs valeurs dans des variables

### Autorisé

*  `let`
*  `const`
*  `for`
*  `while`
*  `if / else`
*  `break`
*  `continue`
*  Opérateurs arithmétiques
*  Opérateurs de comparaison
*  Opérateurs logiques
*  `console.log()`

---

#  A

# Partie 1 — Boucle `for`

## Challenge 1 : Compter les participants

Une formation commence avec un certain nombre de participants.

Écrivez un programme qui affiche les numéros des participants de `1` jusqu'au nombre fourni par l'utilisateur.

**Exemple :**

```text
Nombre de participants : 8

Participant 1
Participant 2
Participant 3
Participant 4
Participant 5
Participant 6
Participant 7
Participant 8
```

**Niveau : 🟡 Moyen**

---

## Challenge 2 : Afficher les nombres pairs

Écrivez un programme qui affiche tous les nombres pairs compris entre `1` et `N`.

**Exemple :**

```text
N = 20

2
4
6
8
10
12
14
16
18
20
```

**Contrainte :**

Utiliser une boucle `for`.

---

## Challenge 3 : Somme des nombres

Écrivez un programme qui calcule la somme de tous les nombres de `1` à `N`.

**Exemple :**

```text
N = 5

Somme = 15
```

Car :

```text
1 + 2 + 3 + 4 + 5 = 15
```

---

## Challenge 4 : Table de multiplication

Écrivez un programme qui demande un nombre et affiche sa table de multiplication de `1` à `10`.

**Exemple :**

```text
Nombre : 7

7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
...
7 x 10 = 70
```

---

## Challenge 5 : Compter les multiples

Écrivez un programme qui demande deux nombres :

* `N`
* `X`

Le programme doit afficher tous les multiples de `X` compris entre `1` et `N`.

**Exemple :**

```text
N = 30
X = 5

5
10
15
20
25
30
```

**Bonus :**

Afficher également le nombre total de multiples trouvés.

---

# Partie 2 — Boucle `while`

## Challenge 6 : Compte à rebours

Écrivez un programme qui effectue un compte à rebours à partir d'un nombre donné jusqu'à `0`.

**Exemple :**

```text
Départ : 5

5
4
3
2
1
0

Décollage !
```

Utilisez `while`.

---

## Challenge 7 : Trouver le premier nombre supérieur

Écrivez un programme qui part de `1` et cherche le premier nombre dont le carré est supérieur à `100`.

**Exemple :**

```text
Résultat : 11

11 × 11 = 121
```

Utilisez `while`.

---

## Challenge 8 : Accumulation de points

Dans un jeu vidéo, un joueur gagne `100` points par mission terminée.

Demandez au joueur combien de missions il souhaite réaliser.

Affichez le score après chaque mission.

**Exemple :**

```text
Nombre de missions : 5

Mission 1 → Score : 100
Mission 2 → Score : 200
Mission 3 → Score : 300
Mission 4 → Score : 400
Mission 5 → Score : 500
```

---

## Challenge 9 : Trouver une puissance

Écrivez un programme qui calcule une puissance sans utiliser `Math.pow()`.

L'utilisateur fournit :

```text
base
exposant
```

Le programme doit effectuer la multiplication plusieurs fois avec une boucle `while`.

**Exemple :**

```text
Base : 2
Exposant : 5

Résultat : 32
```

Car :

```text
2 × 2 × 2 × 2 × 2 = 32
```

---

## Challenge 10 : Saisie jusqu'à une valeur spéciale

Un programme demande à l'utilisateur de saisir des nombres.

La saisie continue jusqu'à ce que l'utilisateur saisisse `0`.

Le programme doit afficher :

* Le nombre de valeurs saisies
* La somme des valeurs

**Exemple :**

```text
Saisie : 10
Saisie : 5
Saisie : 8
Saisie : 0

Nombre de valeurs : 3
Somme : 23
```

---

# B

# Partie 3 — Boucle `for`

## Challenge 11 : Factorielle

Écrivez un programme qui calcule la factorielle d'un nombre.

**Formule :**

```text
N! = N × (N-1) × (N-2) × ... × 1
```

**Exemple :**

```text
N = 5

5! = 120
```

Car :

```text
5 × 4 × 3 × 2 × 1 = 120
```

**Contrainte :**

Ne pas utiliser de fonction prédéfinie.

---

## Challenge 12 : Compter les diviseurs

Écrivez un programme qui reçoit un nombre entier et compte combien de diviseurs il possède.

**Exemple :**

```text
Nombre : 12

Diviseurs :
1
2
3
4
6
12

Nombre de diviseurs : 6
```

**Bonus :**

Afficher également les diviseurs.

---

## Challenge 13 : Vérifier si un nombre est premier

Écrivez un programme qui détermine si un nombre est premier.

Un nombre premier possède exactement deux diviseurs :

```text
1
lui-même
```

**Exemple :**

```text
Nombre : 17

17 est un nombre premier.
```

**Autre exemple :**

```text
Nombre : 15

15 n'est pas un nombre premier.
```

---

## Challenge 14 : Somme des nombres pairs et impairs

Écrivez un programme qui parcourt les nombres de `1` à `N`.

Calculez séparément :

* La somme des nombres pairs
* La somme des nombres impairs

**Exemple :**

```text
N = 10

Somme des pairs : 30
Somme des impairs : 25
```

---

## Challenge 15 : Nombre parfait

Un nombre est considéré comme **parfait** si la somme de ses diviseurs propres est égale au nombre lui-même.

**Exemple :**

```text
6
```

Ses diviseurs propres sont :

```text
1 + 2 + 3 = 6
```

Donc :

```text
6 est un nombre parfait.
```

Écrivez un programme qui vérifie si un nombre donné est parfait.

---

# Partie 4 — Boucle `while`

## Challenge 16 : Deviner un nombre

Le programme possède un nombre secret.

L'utilisateur doit essayer de le trouver.

Après chaque tentative, afficher :

* `Trop petit`
* `Trop grand`
* `Bravo !`

Le programme continue jusqu'à ce que le nombre soit trouvé.

**Exemple :**

```text
Nombre secret : 37

Tentative : 20
Trop petit

Tentative : 50
Trop grand

Tentative : 37
Bravo !
```

---

## Challenge 17 : Compter les chiffres

L'utilisateur fournit un nombre entier positif.

Comptez combien de chiffres contient ce nombre.

**Exemple :**

```text
Nombre : 58392

Nombre de chiffres : 5
```

**Indice :**

Utilisez la division et la boucle `while`.

---

## Challenge 18 : Inverser un nombre

Écrivez un programme qui inverse un nombre entier sans utiliser de chaîne de caractères.

**Exemple :**

```text
Nombre : 12345

Inverse : 54321
```

**Indice :**

Utilisez :

```text
%
/
```

avec une boucle `while`.

---

## Challenge 19 : Somme des chiffres

Écrivez un programme qui calcule la somme des chiffres d'un nombre.

**Exemple :**

```text
Nombre : 583

Somme :
5 + 8 + 3 = 16
```

Résultat :

```text
Somme = 16
```

---

## Challenge 20 : Palindrome numérique

Un nombre est un palindrome lorsqu'il peut être lu dans les deux sens.

**Exemples :**

```text
121 → palindrome
1331 → palindrome
4554 → palindrome
```

Mais :

```text
123 → pas palindrome
1234 → pas palindrome
```

Écrivez un programme qui vérifie si un nombre est un palindrome.

**Contrainte :**

*  Pas de chaîne de caractères
*  Pas de tableau
*  `while`
*  `%`
*  `/`

---

# 🦸 Niveau HÉRO

> Les challenges HÉRO demandent plusieurs étapes de raisonnement et combinent boucles + conditions + calculs.

# Partie 5 — Boucle `for`

## Challenge 21 : Nombres premiers dans un intervalle

L'utilisateur fournit :

```text
début
fin
```

Affichez tous les nombres premiers compris dans cet intervalle.

**Exemple :**

```text
Début : 10
Fin : 30

Nombres premiers :

11
13
17
19
23
29
```

**Contrainte :**

Utiliser des boucles `for`.

**Bonus :**

Afficher également le nombre total de nombres premiers trouvés.

---

## Challenge 22 : Tous les nombres parfaits

L'utilisateur fournit une limite `N`.

Trouvez tous les nombres parfaits compris entre `1` et `N`.

**Exemple :**

```text
N = 10000

Nombres parfaits :

6
28
496
8128
```

Le programme doit utiliser des boucles pour rechercher les nombres parfaits.

---

## Challenge 23 : Suite de Fibonacci

Écrivez un programme qui affiche les `N` premiers termes de la suite de Fibonacci.

La suite commence par :

```text
0
1
```

Chaque nouveau nombre est obtenu en additionnant les deux précédents.

**Exemple :**

```text
N = 10

0
1
1
2
3
5
8
13
21
34
```

**Contrainte :**

Ne pas utiliser de tableau.

---

## Challenge 24 : Triangle numérique

L'utilisateur fournit un nombre `N`.

Affichez un triangle composé de nombres.

**Exemple :**

```text
N = 5

1
12
123
1234
12345
```

**Bonus :**

Créer le triangle suivant :

```text
1
22
333
4444
55555
```

**Contrainte :**

Utiliser des boucles imbriquées.

---

## Challenge 25 : Table de multiplication complète

Affichez toutes les tables de multiplication de `1` à `10`.

**Exemple :**

```text
1 x 1 = 1
1 x 2 = 2
...
1 x 10 = 10

2 x 1 = 2
2 x 2 = 4
...
10 x 10 = 100
```

**Contrainte :**

Utiliser deux boucles imbriquées.

---

# Partie 6 — Boucle `while`

## Challenge 26 : Caisse automatique

Vous développez une caisse automatique.

Le programme demande le prix des produits un par un.

La saisie s'arrête lorsque l'utilisateur entre :

```text
0
```

Le programme doit calculer :

* Nombre de produits
* Total
* Prix moyen
* Produit le plus cher
* Produit le moins cher

**Exemple :**

```text
Prix : 50
Prix : 120
Prix : 35
Prix : 80
Prix : 0

Nombre de produits : 4
Total : 285 DH
Prix moyen : 71.25 DH
Plus cher : 120 DH
Moins cher : 35 DH
```

> ⚠️ Ne pas utiliser de tableau.

---

## Challenge 27 : Système de connexion

Créez un système de connexion simple.

Le programme possède :

```text
Utilisateur : admin
Mot de passe : 1234
```

L'utilisateur dispose de **3 tentatives maximum**.

Après chaque tentative incorrecte :

```text
Identifiants incorrects.
Tentatives restantes : X
```

Si les identifiants sont corrects :

```text
Connexion réussie.
Bienvenue !
```

Après trois échecs :

```text
Compte temporairement bloqué.
```

**Contrainte :**

Utiliser `while`.

---

## Challenge 28 : Analyse de plusieurs nombres

L'utilisateur saisit plusieurs nombres.

La saisie s'arrête lorsqu'il entre `0`.

Le programme doit calculer :

* Nombre total de valeurs
* Somme
* Moyenne
* Plus grand nombre
* Plus petit nombre
* Nombre de valeurs positives
* Nombre de valeurs négatives

**Exemple :**

```text
Saisie : 10
Saisie : -5
Saisie : 20
Saisie : -3
Saisie : 8
Saisie : 0

Nombre de valeurs : 5
Somme : 30
Moyenne : 6
Plus grand : 20
Plus petit : -5
Positifs : 3
Négatifs : 2
```

---

## Challenge 29 : Distributeur automatique

Vous développez un distributeur automatique.

Le menu est :

```text
1 → Retirer de l'argent
2 → Consulter le solde
3 → Déposer de l'argent
4 → Quitter
```

Le solde initial est :

```text
1000 DH
```

Le programme doit continuer à afficher le menu jusqu'à ce que l'utilisateur choisisse `4`.

### Retrait

Vérifier :

* Montant positif
* Montant inférieur ou égal au solde

### Dépôt

Vérifier :

* Montant positif

### Consultation

Afficher le solde actuel.

**Exemple :**

```text
=== MENU ===

1. Retirer
2. Consulter
3. Déposer
4. Quitter

Choix : 1
Montant : 300

Retrait effectué.
Nouveau solde : 700 DH
```

---

## Challenge 30 : Jeu de combat

🦸 **Challenge HÉRO**

Vous développez un mini-jeu de combat entre un joueur et un monstre.

Le joueur possède :

```text
PV = 100
```

Le monstre possède :

```text
PV = 100
```

À chaque tour, le joueur choisit :

```text
1 → Attaque faible
2 → Attaque forte
3 → Soin
```

### Attaque faible

Inflige :

```text
15 dégâts
```

### Attaque forte

Inflige :

```text
30 dégâts
```

### Soin

Récupère :

```text
20 PV
```

Le monstre attaque ensuite automatiquement le joueur et inflige :

```text
10 dégâts
```

Le combat continue tant que :

```text
PV joueur > 0
ET
PV monstre > 0
```

### Fin du combat

Si le joueur atteint `0 PV` :

```text
Game Over !
Le monstre a gagné.
```

Si le monstre atteint `0 PV` :

```text
Victoire !
Vous avez vaincu le monstre.
```

### Bonus HÉRO +

Ajouter :

* Un nombre maximum de potions
* Des coups critiques
* Une attaque spéciale utilisable une seule fois
* Une défense permettant de réduire les dégâts
* Un compteur de tours

**Contrainte :**

*  Aucun tableau
*  Aucune fonction personnalisée
*  Aucune bibliothèque
*  `while`
*  `switch`
*  `if / else`
*  Variables
*  Opérateurs
*  Conditions

---

# 🏆 Tableau de progression

| #  | Challenge               | Boucle  | Niveau    |
| -- | ----------------------- | ------- | --------- |
| 1  | Participants            | `for`   |  Moyen  |
| 2  | Nombres pairs           | `for`   |  Moyen  |
| 3  | Somme                   | `for`   |  Moyen  |
| 4  | Table multiplication    | `for`   |  Moyen  |
| 5  | Multiples               | `for`   |  Moyen  |
| 6  | Compte à rebours        | `while` |  Moyen  |
| 7  | Premier carré supérieur | `while` |  Moyen  |
| 8  | Accumulation de points  | `while` |  Moyen  |
| 9  | Puissance               | `while` |  Moyen  |
| 10 | Saisie jusqu'à 0        | `while` |  Moyen  |
| 11 | Factorielle             | `for`   |  Avancé |
| 12 | Diviseurs               | `for`   |  Avancé |
| 13 | Nombre premier          | `for`   |  Avancé |
| 14 | Somme pairs/impairs     | `for`   |  Avancé |
| 15 | Nombre parfait          | `for`   |  Avancé |
| 16 | Deviner un nombre       | `while` |  Avancé |
| 17 | Compter les chiffres    | `while` |  Avancé |
| 18 | Inverser un nombre      | `while` |  Avancé |
| 19 | Somme des chiffres      | `while` |  Avancé |
| 20 | Palindrome              | `while` |  Avancé |
| 21 | Premiers intervalle     | `for`   |  Héro   |
| 22 | Nombres parfaits        | `for`   |  Héro   |
| 23 | Fibonacci               | `for`   |  Héro   |
| 24 | Triangle numérique      | `for`   |  Héro   |
| 25 | Tables complètes        | `for`   |  Héro   |
| 26 | Caisse automatique      | `while` |  Héro   |
| 27 | Système connexion       | `while` |  Héro   |
| 28 | Analyse nombres         | `while` |  Héro   |
| 29 | Distributeur            | `while` |  Héro   |
| 30 | Jeu de combat           | `while` |  Héro   |

---

# Objectif pédagogique

## Niveau Moyen

L'apprenant doit comprendre :

```text
Initialisation
     ↓
Condition
     ↓
Exécution
     ↓
Mise à jour
     ↓
Nouvelle itération
```

Et savoir utiliser :

```javascript
for
while
```

pour répéter une action.

---

## Niveau Avancé

L'apprenant doit être capable de combiner :

```text
Boucle
   +
Condition
   +
Compteur
   +
Accumulateur
```

Exemple :

```text
compteur → compter
somme → accumuler
maximum → comparer
minimum → comparer
```

---

## Niveau HÉRO

L'apprenant doit être capable de résoudre des problèmes comportant :

```text
Boucles imbriquées
        +
Conditions multiples
        +
Calculs
        +
Compteurs
        +
Accumulateurs
        +
Gestion de scénarios
```

> **Méthode recommandée :**
>
> 1. Comprendre le problème
> 2. Identifier les données d'entrée
> 3. Identifier les données à calculer
> 4. Déterminer la condition d'arrêt
> 5. Choisir `for` ou `while`
> 6. Écrire le pseudo-code
> 7. Traduire en JavaScript
> 8. Tester plusieurs cas
