# Challenges JavaScript — Problem Solving

> **Règle générale :** Les fonctions prédéfinies de JavaScript sont interdites.
>
> L'objectif est de résoudre les problèmes avec les variables, les types, les opérateurs et les conditions.

## Fonctions interdites

```javascript
Math.sqrt()
Math.pow()
Math.PI
parseInt()
parseFloat()
Number()
String()
.toString()
```

---

## Exercices sur les Variables et les Opérateurs

### Challenge 1 : Profil d'un joueur

Vous développez un petit système pour un jeu vidéo.

Créez un programme qui stocke dans des variables les informations d'un joueur :

* Pseudo
* Niveau
* Âge
* Score
* Pays

Puis affichez toutes les informations dans la console.

**Exemple :**

```text
Pseudo : ShadowX
Niveau : 12
Âge : 21
Score : 4580
Pays : Maroc
```

---

### Challenge 2 : Conversion de monnaie

Vous développez une application permettant à un voyageur de convertir son budget.

L'utilisateur possède un montant en **dirhams marocains (MAD)**.

Convertissez ce montant en **euros (EUR)**.

Pour cet exercice, utilisez le taux fictif :

```text
1 EUR = 11 MAD
```

**Formule :**

```text
EUR = MAD / 11
```

**Exemple :**

```text
Budget en MAD : 2200

Budget en EUR : 200
```

---

### Challenge 3 : Conversion de stockage

Un utilisateur souhaite connaître l'espace disponible sur son ordinateur.

Il possède une capacité exprimée en **Gigaoctets (GB)**.

Convertissez cette capacité en **Mégaoctets (MB)**.

Utilisez :

```text
1 GB = 1024 MB
```

**Formule :**

```text
MB = GB * 1024
```

**Exemple :**

```text
Stockage : 10 GB

Résultat : 10240 MB
```

---

### Challenge 4 : Calcul de consommation d'une voiture

Vous développez une application pour calculer la consommation d'une voiture.

L'utilisateur fournit :

* La distance parcourue en kilomètres
* La quantité de carburant consommée en litres

Calculez la consommation moyenne en **litres / 100 km**.

**Formule :**

```text
Consommation = (litres / kilomètres) * 100
```

**Exemple :**

```text
Distance : 500 km
Carburant : 35 litres

Consommation : 7 L/100 km
```

---

### Challenge 5 : Catégorie d'un film

Une plateforme de streaming souhaite classer automatiquement les films selon leur durée.

L'utilisateur fournit la durée du film en minutes.

Déterminez la catégorie :

* Moins de 60 minutes → `Court métrage`
* De 60 à 120 minutes → `Film standard`
* Plus de 120 minutes → `Film long`

**Exemple :**

```text
Durée : 95 minutes

Catégorie : Film standard
```

---

### Challenge 6 : Calcul du score d'un examen

Un apprenant passe un examen composé de quatre parties.

Chaque partie donne un score différent.

L'utilisateur fournit :

```text
Score partie 1
Score partie 2
Score partie 3
Score partie 4
```

Calculez :

* Le score total
* Le score moyen

**Exemple :**

```text
Partie 1 : 15
Partie 2 : 12
Partie 3 : 18
Partie 4 : 15

Score total : 60
Moyenne : 15
```

---

### Challenge 7 : Calcul de la note finale

Un apprenant est évalué selon trois éléments :

* Contrôle continu : coefficient `2`
* Projet : coefficient `3`
* Examen final : coefficient `5`

Écrivez un programme qui calcule la note finale pondérée.

**Formule :**

```text
Note finale =
(noteCC * 2 + noteProjet * 3 + noteExamen * 5) / 10
```

**Exemple :**

```text
Contrôle continu : 14
Projet : 16
Examen : 12

Note finale : 13.8
```

---

### Challenge 8 : Calcul de la puissance d'une batterie

Une application mobile doit calculer l'énergie théorique d'une batterie.

L'utilisateur fournit :

* La tension `U` en volts
* L'intensité `I` en ampères
* Le temps `t` en heures

Calculez l'énergie consommée.

**Formule :**

```text
Énergie = U * I * t
```

**Exemple :**

```text
Tension : 12 V
Intensité : 2 A
Temps : 3 heures

Énergie : 72 Wh
```

---

### Challenge 9 : Distance parcourue par un drone

Un drone se déplace entre deux positions dans un espace 3D.

La première position est :

```text
A(x1, y1, z1)
```

La deuxième position est :

```text
B(x2, y2, z2)
```

Calculez la distance parcourue par le drone.

**Formule :**

```text
Distance = √((x2-x1)² + (y2-y1)² + (z2-z1)²)
```

**Exemple :**

```text
Position A : (1, 2, 3)
Position B : (4, 6, 3)

Distance : 5
```

> `Math.sqrt()` et `Math.pow()` sont interdits.

---

### Challenge 10 : Calcul de la capacité d'un réservoir cylindrique

Un système industriel possède un réservoir cylindrique.

L'utilisateur fournit :

* Le rayon du réservoir
* La hauteur du réservoir

Calculez son volume.

**Formule :**

```text
Volume = π * r² * h
```

Utilisez :

```text
π = 3.14159
```

**Exemple :**

```text
Rayon : 2 m
Hauteur : 5 m

Volume : 62.8318 m³
```

> `Math.PI` et `Math.pow()` sont interdits.

---

### Challenge 11 : Calcul de la surface d'une pièce

Vous développez une application destinée aux architectes.

Une pièce possède une forme rectangulaire.

L'utilisateur fournit :

* Longueur
* Largeur

Calculez :

* La surface
* Le périmètre

**Formules :**

```text
Surface = longueur * largeur
```

```text
Périmètre = 2 * (longueur + largeur)
```

**Exemple :**

```text
Longueur : 6 m
Largeur : 4 m

Surface : 24 m²
Périmètre : 20 m
```

---

### Challenge 12 : Lire les chiffres d'un code PIN

Un système de sécurité utilise un code composé de quatre chiffres.

L'utilisateur saisit un nombre à quatre chiffres.

Votre programme doit afficher chaque chiffre séparément.

**Exemple :**

```text
Code : 5832

Premier chiffre : 5
Deuxième chiffre : 8
Troisième chiffre : 3
Quatrième chiffre : 2
```

**Contrainte :**

* Pas de boucle
* Pas de conversion en chaîne de caractères
* Utiliser les opérateurs `/` et `%`

---

### Challenge 13 : Calculer le montant en binaire

Un système informatique stocke certaines valeurs sous forme binaire.

L'utilisateur fournit un nombre entier compris entre `0` et `255`.

Écrivez un programme qui affiche sa représentation binaire.

**Exemple :**

```text
Nombre : 13

Binaire : 1101
```

**Autres exemples :**

```text
Nombre : 7

Binaire : 111
```

```text
Nombre : 16

Binaire : 10000
```

**Contrainte :**

La méthode suivante est interdite :

```javascript
nombre.toString(2)
```

La conversion doit être réalisée manuellement.

---

## Challenges supplémentaires

### Challenge 14 : Échange de deux scores

Deux joueurs possèdent chacun un score.

```text
Joueur A : 1500
Joueur B : 2300
```

Écrivez un programme permettant d'échanger leurs scores.

Après l'échange :

```text
Joueur A : 2300
Joueur B : 1500
```

**Contrainte :**

Utiliser une troisième variable.

**Bonus :**

Réaliser l'échange sans troisième variable.

---

### Challenge 15 : Ticket de cinéma

Un cinéma souhaite automatiser le calcul du prix d'une réservation.

L'utilisateur fournit :

* Prix d'un billet
* Nombre de billets
* Prix d'une boisson
* Nombre de boissons

Calculez le montant total.

**Formule :**

```text
Total billets = prix billet * nombre billets
```

```text
Total boissons = prix boisson * nombre boissons
```

```text
Total = total billets + total boissons
```

**Exemple :**

```text
Prix billet : 50 DH
Nombre de billets : 3

Prix boisson : 15 DH
Nombre de boissons : 3

Total : 195 DH
```

---

### Challenge 16 : Convertisseur de durée

Une application de streaming reçoit une durée exprimée en secondes.

Transformez cette durée en :

* Heures
* Minutes
* Secondes

**Exemple :**

```text
Durée : 7384 secondes

Heures : 2
Minutes : 3
Secondes : 4
```

**Indice :**

Utilisez :

```text
/
%
```

---

### Challenge 17 : Calcul des points d'un joueur

Dans un jeu, un joueur gagne :

* `100` points par ennemi éliminé
* `50` points par mission terminée
* `200` points pour chaque boss vaincu

L'utilisateur fournit :

* Nombre d'ennemis éliminés
* Nombre de missions terminées
* Nombre de boss vaincus

Calculez le score total.

**Formule :**

```text
Score =
ennemis * 100
+ missions * 50
+ boss * 200
```

**Exemple :**

```text
Ennemis : 10
Missions : 5
Boss : 2

Score total : 2500
```

---

### Challenge 18 : Informations sur un produit

Un magasin possède un produit avec :

```javascript
let nom = "Clavier";
let prix = 350;
let disponible = true;
let stock = 12;
```

Affichez le type de chaque variable avec `typeof`.

**Exemple :**

```text
nom → string
prix → number
disponible → boolean
stock → number
```

Ajoutez également une variable contenant `null` et observez son type.

---

### Challenge 19 : Réduction sur un produit

Un magasin propose une réduction sur ses produits.

L'utilisateur fournit :

* Le prix initial
* Le pourcentage de réduction

Calculez :

* Le montant de la réduction
* Le prix final

**Formules :**

```text
Réduction = prix * pourcentage / 100
```

```text
Prix final = prix - réduction
```

**Exemple :**

```text
Prix : 800 DH
Réduction : 25%

Montant de la réduction : 200 DH
Prix final : 600 DH
```

---

### Challenge 20 : Vérification d'un numéro de casier

Dans une salle de sport, chaque casier possède un numéro.

Écrivez un programme qui reçoit le numéro d'un casier et détermine s'il est :

* `Pair` → Casier côté A
* `Impair` → Casier côté B

**Exemple :**

```text
Numéro du casier : 24

Casier côté A
```

```text
Numéro du casier : 17

Casier côté B
```

**Contrainte :**

Utiliser l'opérateur `%`.

---

# Règles générales

Pour tous les challenges :

## Interdit

* `Math.sqrt()`
* `Math.pow()`
* `Math.PI`
* `parseInt()`
* `parseFloat()`
* `Number()`
* `String()`
* `.toString()`
* Fonctions personnalisées
* Bibliothèques externes

## Autorisé

* `let`
* `const`
* Variables
* Types primitifs
* `typeof`
* `console.log()`
* Opérateurs arithmétiques
* Opérateurs d'affectation
* Opérateurs de comparaison
* Opérateurs logiques
* `if / else`
* `/`
* `%`

# Objectif pédagogique

Ces challenges ont pour objectif de développer :

* Le raisonnement logique
* La décomposition d'un problème
* La manipulation des variables
* La compréhension des types
* La maîtrise des opérateurs
* La capacité à traduire une formule en code
* La résolution de problèmes sans dépendre des fonctions prédéfinies

> **Principe :** comprendre le problème → identifier les données → trouver la formule ou la logique → écrire l'algorithme → traduire en JavaScript.
