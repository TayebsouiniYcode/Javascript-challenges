# Challenges JavaScript — Les Conditions

> **Règle générale :**
>
> * Utiliser uniquement les notions étudiées.
> * Les fonctions prédéfinies sont interdites.
> * Pour les challenges `if / else`, ne pas utiliser `switch`.
> * Pour les challenges `switch / case`, ne pas utiliser `if / else`.
> * Utiliser `console.log()` pour afficher les résultats.

---

# Partie 1 — `if / else`

## Challenge 1 : Vérifier l'âge

Écrivez un programme qui demande l'âge d'une personne et détermine si elle peut accéder à un espace réservé aux adultes.

**Règle :**

* Si l'âge est supérieur ou égal à `18` → afficher `Accès autorisé`
* Sinon → afficher `Accès refusé`

**Exemple :**

```text
Âge : 21

Accès autorisé
```

**Niveau : Facile**

---

## Challenge 2 : Positif, négatif ou zéro

Écrivez un programme qui reçoit un nombre entier et détermine s'il est :

* Positif
* Négatif
* Égal à zéro

**Exemple 1 :**

```text
Nombre : 15

Le nombre est positif.
```

**Exemple 2 :**

```text
Nombre : -8

Le nombre est négatif.
```

**Exemple 3 :**

```text
Nombre : 0

Le nombre est égal à zéro.
```

**Niveau : Facile**

---

## Challenge 3 : Vérification d'une note

Un apprenant obtient une note sur `20`.

Écrivez un programme qui affiche son résultat.

**Règles :**

* Note >= `10` → `Admis`
* Note < `10` → `Non admis`

**Exemple :**

```text
Note : 14

Résultat : Admis
```

**Bonus :**

Ajouter une vérification pour détecter une note invalide :

* Note < `0`
* Note > `20`

**Niveau : Facile**

---

## Challenge 4 : Livraison gratuite

Une boutique en ligne propose la livraison gratuite à partir d'un certain montant.

L'utilisateur saisit le montant de sa commande.

**Règles :**

* Montant >= `500 DH` → Livraison gratuite
* Montant < `500 DH` → Frais de livraison : `40 DH`

Le programme doit afficher le montant final à payer.

**Exemple :**

```text
Montant de la commande : 650 DH

Livraison : Gratuite
Total à payer : 650 DH
```

**Autre exemple :**

```text
Montant de la commande : 300 DH

Livraison : 40 DH
Total à payer : 340 DH
```

**Niveau : Facile → Moyen**

---

## Challenge 5 : Calcul de la mention

Une école souhaite afficher automatiquement la mention obtenue par un apprenant selon sa note.

La note est comprise entre `0` et `20`.

**Règles :**

| Note         | Mention    |
| ------------ | ---------- |
| `< 10`       | Échec      |
| `10 - 11.99` | Passable   |
| `12 - 13.99` | Assez bien |
| `14 - 15.99` | Bien       |
| `16 - 17.99` | Très bien  |
| `18 - 20`    | Excellent  |

Écrivez un programme qui affiche la mention correspondante.

**Exemple :**

```text
Note : 15

Mention : Bien
```

**Bonus :**

Gérer les notes invalides.

**Niveau : Moyen**

---

# Partie 2 — `switch / case`

> Dans cette partie, utilisez **uniquement `switch / case`** pour prendre les décisions.

---

## Challenge 6 : Menu d'une application

Vous développez le menu principal d'une application.

L'utilisateur choisit une option :

```text
1 → Afficher le profil
2 → Afficher les paramètres
3 → Afficher les notifications
4 → Se déconnecter
```

Écrivez un programme qui affiche l'action correspondant au choix.

**Exemple :**

```text
Choix : 2

Ouverture des paramètres...
```

Si l'utilisateur saisit une autre valeur :

```text
Choix invalide.
```

**Niveau : Facile**

---

## Challenge 7 : Jour de la semaine

Un programme reçoit un numéro représentant un jour de la semaine.

```text
1 → Lundi
2 → Mardi
3 → Mercredi
4 → Jeudi
5 → Vendredi
6 → Samedi
7 → Dimanche
```

Utilisez `switch / case` pour afficher le jour correspondant.

**Exemple :**

```text
Numéro : 3

Jour : Mercredi
```

Si le numéro n'est pas compris entre `1` et `7` :

```text
Numéro invalide.
```

**Niveau : Facile**

---

## Challenge 8 : Calculatrice simple

Écrivez une calculatrice simple utilisant `switch / case`.

L'utilisateur fournit :

* Un premier nombre
* Un opérateur
* Un deuxième nombre

Les opérateurs disponibles sont :

```text
+ 
-
*
/
```

Le programme doit effectuer l'opération correspondante.

**Exemple :**

```text
Premier nombre : 20
Opérateur : *
Deuxième nombre : 5

Résultat : 100
```

Si l'utilisateur saisit un opérateur inconnu :

```text
Opérateur invalide.
```

**Bonus :**

Gérer le cas d'une division par zéro.

**Niveau : Moyen**

---

## Challenge 9 : Système de transport

Une application de transport permet à l'utilisateur de choisir son moyen de transport.

```text
1 → Bus
2 → Train
3 → Tramway
4 → Taxi
5 → Vélo
```

Utilisez `switch / case` pour afficher le prix d'un trajet.

**Tarifs :**

```text
Bus     → 5 DH
Train   → 20 DH
Tramway → 6 DH
Taxi    → 15 DH
Vélo    → 10 DH
```

**Exemple :**

```text
Choix : 3

Transport : Tramway
Prix : 6 DH
```

Pour un choix inexistant :

```text
Transport invalide.
```

**Niveau : Moyen**

---

## Challenge 10 : Code d'une catégorie de produit

Une boutique utilise des codes pour identifier les catégories de produits.

```text
A → Électronique
B → Vêtements
C → Alimentation
D → Maison
E → Sport
```

Écrivez un programme utilisant `switch / case` qui reçoit le code d'une catégorie et affiche son nom.

**Exemple :**

```text
Code : C

Catégorie : Alimentation
```

Si le code est inconnu :

```text
Catégorie inconnue.
```

**Bonus :**

Pour chaque catégorie, afficher également un exemple de produit.

```text
A → Électronique → Smartphone
B → Vêtements → T-shirt
C → Alimentation → Pain
D → Maison → Chaise
E → Sport → Ballon
```

**Niveau : Moyen**

---

# Défi bonus — Mix `if / else` + `switch`

## Challenge 11 : Système de commande

Vous développez un système simple de commande pour un restaurant.

L'utilisateur choisit un plat :

```text
1 → Pizza
2 → Burger
3 → Tacos
4 → Salade
```

Chaque plat possède un prix :

```text
Pizza  → 60 DH
Burger → 45 DH
Tacos  → 40 DH
Salade → 30 DH
```

Le programme doit ensuite demander la quantité.

### Étape 1

Utiliser `switch / case` pour déterminer le plat et son prix.

### Étape 2

Utiliser `if / else` pour appliquer une réduction :

* Total >= `200 DH` → réduction de `10%`
* Total < `200 DH` → aucune réduction

### Étape 3

Afficher :

```text
Plat :
Prix unitaire :
Quantité :
Sous-total :
Réduction :
Total à payer :
```

**Exemple :**

```text
Choix : 1
Quantité : 4

Plat : Pizza
Prix unitaire : 60 DH
Sous-total : 240 DH
Réduction : 24 DH
Total à payer : 216 DH
```

## **Niveau : Moyen +**

# Progression pédagogique

| Challenge | Notion                 | Niveau          |
| --------- | ---------------------- | --------------- |
| 1         | `if / else` simple     | 🟢 Facile       |
| 2         | `if / else if / else`  | 🟢 Facile       |
| 3         | Comparaison            | 🟢 Facile       |
| 4         | Condition + calcul     | 🟡 Facile/Moyen |
| 5         | Conditions multiples   | 🟡 Moyen        |
| 6         | `switch / case`        | 🟢 Facile       |
| 7         | `switch / case`        | 🟢 Facile       |
| 8         | `switch` + opérateurs  | 🟡 Moyen        |
| 9         | `switch` + calcul      | 🟡 Moyen        |
| 10        | `switch` + données     | 🟡 Moyen        |
| 11        | `if / else` + `switch` | 🔴 Moyen+       |

# Contraintes

Pour tous les exercices :

* Pas de `Math.*`
* Pas de `parseInt()`
* Pas de `parseFloat()`
* Pas de `Number()`
* Pas de fonctions personnalisées
* Pas de bibliothèques externes
* `let`
* `const`
* Comparaisons
* Opérateurs logiques
* `if / else`
* `switch / case`
* Opérateurs arithmétiques
* `console.log()`

> **Objectif :** être capable de transformer une règle métier simple en conditions JavaScript.
