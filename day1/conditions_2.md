# JavaScript — Challenges Conditions

## Règles générales

Pour tous les challenges :

* Pas de `Math.*`
* Pas de `parseInt()`
* Pas de `parseFloat()`
* Pas de `Number()`
* Pas de `String()`
* Pas de fonctions personnalisées
* Pas de bibliothèques externes
* Variables
* `let` / `const`
* Opérateurs arithmétiques
* Opérateurs de comparaison
* Opérateurs logiques
* `if / else`
* `switch / case`
* `console.log()`

> **Important :** dans les challenges `if / else`, utilisez `if / else` pour les décisions.
> Dans les challenges `switch / case`, utilisez principalement `switch / case`.

---

# Niveau Moyen

# Partie 1 — `if / else`

## Challenge 1 : Tarif de livraison

Une boutique en ligne calcule les frais de livraison selon le montant de la commande.

**Règles :**

* Montant < `100 DH` → livraison `30 DH`
* Montant entre `100 DH` et `299 DH` → livraison `20 DH`
* Montant entre `300 DH` et `499 DH` → livraison `10 DH`
* Montant >= `500 DH` → livraison gratuite

Afficher :

```text
Montant commande :
Frais livraison :
Total à payer :
```

**Exemple :**

```text
Montant commande : 350 DH
Frais livraison : 10 DH
Total à payer : 360 DH
```

---

## Challenge 2 : Feu tricolore

Un système de circulation reçoit une couleur de feu :

* `rouge`
* `orange`
* `vert`

Le programme doit afficher l'action du conducteur.

**Règles :**

```text
rouge  → Arrêtez-vous
orange → Ralentissez
vert   → Vous pouvez passer
```

Si la couleur est inconnue :

```text
Couleur invalide
```

---

## Challenge 3 : Calcul d'une remise

Un magasin applique une réduction selon le montant d'achat.

**Règles :**

* < `500 DH` → aucune réduction
* `500 - 999 DH` → `5%`
* `1000 - 1999 DH` → `10%`
* > = `2000 DH` → `15%`

Calculez :

* Montant initial
* Réduction
* Prix final

**Exemple :**

```text
Montant : 1500 DH
Réduction : 150 DH
Total : 1350 DH
```

---

## Challenge 4 : Validation d'un triangle

L'utilisateur fournit trois longueurs :

```text
a
b
c
```

Déterminez si elles peuvent former un triangle.

**Règle :**

```text
a + b > c
a + c > b
b + c > a
```

Si les trois conditions sont vraies :

```text
Triangle valide
```

Sinon :

```text
Triangle invalide
```

**Bonus :**

Si le triangle est valide, déterminer s'il est :

* Équilatéral
* Isocèle
* Scalène

---

## Challenge 5 : Système de classement

Dans un jeu vidéo, un joueur reçoit un rang selon son score.

**Règles :**

* Score < `1000` → Bronze
* `1000 - 1999` → Argent
* `2000 - 2999` → Or
* `3000 - 4999` → Diamant
* > = `5000` → Légende

Afficher le rang correspondant.

**Bonus :**

Afficher également le nombre de points nécessaires pour atteindre le rang suivant.

---

# Partie 2 — `switch / case`

## Challenge 6 : Mois de l'année

L'utilisateur saisit un numéro de mois.

```text
1  → Janvier
2  → Février
3  → Mars
...
12 → Décembre
```

Utilisez `switch / case` pour afficher le nom du mois.

**Bonus :**

Afficher également le nombre de jours du mois.

---

## Challenge 7 : Type de compte bancaire

Une banque utilise les codes suivants :

```text
1 → Compte courant
2 → Compte épargne
3 → Compte étudiant
4 → Compte professionnel
```

Le programme reçoit le code et affiche le type de compte.

**Bonus :**

Afficher les frais mensuels :

```text
Courant       → 20 DH
Épargne       → 10 DH
Étudiant      → 0 DH
Professionnel → 50 DH
```

---

## Challenge 8 : Niveau de difficulté d'un jeu

Un jeu propose quatre niveaux :

```text
1 → Facile
2 → Normal
3 → Difficile
4 → Extrême
```

Utilisez `switch / case` pour afficher :

* Le niveau
* Le nombre d'ennemis
* Le nombre de points gagnés par ennemi

**Exemple :**

```text
Choix : 3

Niveau : Difficile
Ennemis : 50
Points par ennemi : 30
```

---

## Challenge 9 : Type de billet

Une salle de spectacle propose plusieurs types de billets :

```text
1 → Standard
2 → VIP
3 → Premium
4 → Enfant
```

Utilisez `switch / case` pour déterminer le prix.

```text
Standard → 80 DH
VIP      → 200 DH
Premium  → 350 DH
Enfant   → 40 DH
```

Demandez également la quantité et calculez le total.

---

## Challenge 10 : Convertisseur d'unités

Une application permet de choisir une conversion :

```text
1 → Km vers mètres
2 → Mètres vers cm
3 → Kg vers grammes
4 → Litres vers millilitres
```

Utilisez `switch / case`.

**Exemple :**

```text
Choix : 1
Valeur : 5

Résultat : 5000 mètres
```

---

# Niveau Avancé

# Partie 1 — `if / else`

## Challenge 11 : Analyse d'une date

L'utilisateur fournit :

```text
jour
mois
année
```

Déterminez si la date est valide.

Exemples :

```text
25 / 12 / 2026 → Date valide
31 / 02 / 2026 → Date invalide
```

Gérez également les années bissextiles.

**Règle :**

Une année est bissextile si :

```text
année divisible par 400
OU
année divisible par 4 ET non divisible par 100
```

---

## Challenge 12 : Calcul progressif d'un salaire

Une entreprise calcule une prime selon l'ancienneté et le salaire.

**Règles :**

### Ancienneté

* < 1 an → `0%`
* 1 à 3 ans → `5%`
* 4 à 7 ans → `10%`
* > 7 ans → `15%`

### Bonus supplémentaire

Si le salaire est inférieur à `6000 DH` :

```text
+ 2%
```

Sinon :

```text
+ 0%
```

Calculez la prime et le salaire final.

---

## Challenge 13 : Système de réservation

Un hôtel possède trois types de chambres :

* Standard
* Deluxe
* Suite

Le prix dépend :

* du type de chambre
* du nombre de nuits
* de la saison

**Saison haute :**

```text
+ 30%
```

**Saison normale :**

```text
prix normal
```

**Bonus :**

Si le client réserve plus de `7 nuits` :

```text
- 10%
```

Calculez le prix final.

---

## Challenge 14 : Admission universitaire

Une université accepte un candidat selon plusieurs critères :

* Note générale >= `12`
* Note en mathématiques >= `10`
* Note en informatique >= `12`

Mais certaines formations ont des exigences supplémentaires.

Déterminez si le candidat est :

```text
Admis
Admis sous condition
Refusé
```

Vous devez combiner plusieurs conditions avec :

```text
&&
||
!
```

---

## Challenge 15 : Système de parking

Un parking calcule le prix selon la durée.

**Tarification :**

```text
1ère heure  → 5 DH
2ème heure  → 3 DH
3ème heure  → 3 DH
Chaque heure supplémentaire → 2 DH
```

Le programme reçoit le nombre d'heures.

Calculez le prix total.

**Bonus :**

Ajouter une réduction de `20%` pour les clients possédant une carte membre.

---

# Partie 2 — `switch / case`

## Challenge 16 : Menu de restaurant

Un restaurant propose :

```text
1 → Pizza
2 → Burger
3 → Tacos
4 → Salade
5 → Pasta
```

Utilisez `switch / case` pour déterminer le prix.

Ajoutez ensuite :

* quantité
* total
* réduction éventuelle

**Règle de réduction :**

Si le total dépasse `300 DH`, appliquer `10%`.

---

## Challenge 17 : Opérations mathématiques

Créez une calculatrice avec :

```text
+ 
-
*
/
%
```

L'utilisateur fournit :

```text
nombre1
opérateur
nombre2
```

Utilisez `switch / case`.

**Exemple :**

```text
Nombre 1 : 25
Opérateur : %
Nombre 2 : 7

Résultat : 4
```

Gérer la division par zéro.

---

## Challenge 18 : Code de pays

Une application reçoit un code :

```text
MA → Maroc
FR → France
ES → Espagne
US → États-Unis
CA → Canada
JP → Japon
BR → Brésil
```

Utilisez `switch / case` pour afficher :

* Le pays
* La devise

**Exemple :**

```text
Code : MA

Pays : Maroc
Devise : Dirham marocain
```

---

## Challenge 19 : Système de transport

Une entreprise de transport propose :

```text
1 → Petit trajet
2 → Trajet moyen
3 → Long trajet
4 → Trajet international
```

Utilisez `switch / case` pour déterminer le prix de base.

Ensuite, selon le nombre de passagers, calculez le prix total.

**Tarifs :**

```text
Petit trajet        → 20 DH
Trajet moyen        → 50 DH
Long trajet         → 100 DH
International       → 500 DH
```

**Bonus :**

À partir de `5 passagers`, appliquer `15%` de réduction.

---

## Challenge 20 : Gestion des commandes

Une entreprise utilise des codes de statut :

```text
1 → Commande reçue
2 → En préparation
3 → Expédiée
4 → En livraison
5 → Livrée
6 → Annulée
```

Utilisez `switch / case`.

Pour chaque statut, afficher un message différent.

**Exemple :**

```text
Code : 4

Statut : En livraison
Message : Votre commande est actuellement en route.
```

**Bonus :**

Afficher si l'utilisateur peut encore annuler sa commande.

---

# Niveau HÉRO

> Ces challenges demandent plusieurs étapes de raisonnement et la combinaison de plusieurs conditions.

# Partie 1 — `if / else`

## Challenge 21 : Système bancaire intelligent

Vous développez un système de retrait bancaire.

L'utilisateur fournit :

* Solde disponible
* Montant à retirer
* Carte active ou non
* Code PIN correct ou non

Le retrait est autorisé uniquement si :

```text
Carte active
ET
PIN correct
ET
Montant > 0
ET
Montant <= solde
```

Ajoutez les règles suivantes :

* Retrait maximum : `5000 DH`
* Si le montant est supérieur à `3000 DH`, afficher un avertissement.
* Si le solde après retrait est inférieur à `100 DH`, afficher une alerte.

Le programme doit afficher un message précis pour chaque situation.

---

## Challenge 22 : Système de réservation de vol

Un utilisateur souhaite réserver un vol.

Il fournit :

* Âge
* Classe : économique / business
* Nombre de bagages
* Prix du billet
* Statut membre

### Règles bagages

Économique :

```text
1 bagage gratuit
Chaque bagage supplémentaire → 150 DH
```

Business :

```text
2 bagages gratuits
Chaque bagage supplémentaire → 100 DH
```

### Réduction membre

```text
Membre Gold → 20%
Membre Silver → 10%
Pas membre → 0%
```

Calculez le prix final.

Ajoutez une règle :

```text
Si âge < 12 ans → réduction supplémentaire de 50% sur le billet.
```

---

## Challenge 23 : Évaluation d'un mot de passe

Un utilisateur saisit les caractéristiques d'un mot de passe :

* Nombre de caractères
* Nombre de chiffres
* Nombre de caractères spéciaux
* Présence de lettres majuscules

Déterminez sa sécurité.

**Règles :**

### Faible

```text
moins de 8 caractères
```

### Moyen

```text
au moins 8 caractères
ET
au moins 1 chiffre
```

### Fort

```text
au moins 12 caractères
ET
au moins 2 chiffres
ET
au moins 1 caractère spécial
ET
au moins 1 majuscule
```

Sinon :

```text
Mot de passe moyen
```

---

## Challenge 24 : Système de notation d'un jeu

Un joueur possède :

* Score
* Nombre de victoires
* Nombre de défaites
* Nombre de matchs joués

Calculez son taux de victoire :

```text
Taux = victoires / matchs * 100
```

Déterminez son niveau :

```text
Score >= 5000 ET taux >= 80% → Légende

Score >= 3000 ET taux >= 65% → Diamant

Score >= 1500 ET taux >= 50% → Or

Score >= 500 → Argent

Sinon → Bronze
```

Gérez également le cas où le joueur n'a joué aucun match.

---

## Challenge 25 : Feu intelligent

Vous développez un système de contrôle d'un feu de circulation.

Le programme reçoit :

* Couleur actuelle
* Présence de piétons
* Présence d'une ambulance
* Heure
* Nombre de voitures en attente

Le système doit déterminer l'action.

### Règles prioritaires

**1. Ambulance présente**

```text
→ Donner immédiatement la priorité
```

**2. Piétons présents**

Si le feu est rouge :

```text
→ Autoriser les piétons
```

**3. Beaucoup de voitures**

Si plus de `20` voitures attendent :

```text
→ Prolonger le feu vert
```

**4. Nuit**

Entre `00:00` et `05:00` :

```text
→ Mode nuit
```

Le programme doit déterminer le comportement final du système.

---

# Partie 2 — `switch / case`

## Challenge 26 : Système de paiement

Un site e-commerce propose plusieurs moyens de paiement :

```text
1 → Carte bancaire
2 → PayPal
3 → Virement bancaire
4 → Paiement à la livraison
5 → Carte cadeau
```

Utilisez `switch / case`.

Chaque moyen de paiement possède des règles différentes.

### Carte bancaire

```text
Frais = 2%
```

### PayPal

```text
Frais = 3%
```

### Virement

```text
Frais = 0%
```

### Paiement à la livraison

```text
Frais = 20 DH
```

### Carte cadeau

```text
Aucun frais
```

Calculez le montant final.

---

## Challenge 27 : Système de support technique

Un utilisateur choisit un type de problème :

```text
1 → Connexion
2 → Mot de passe
3 → Paiement
4 → Compte bloqué
5 → Problème technique
6 → Autre
```

Utilisez `switch / case`.

Pour chaque catégorie, afficher :

* Département responsable
* Niveau de priorité
* Délai estimé

**Exemple :**

```text
Choix : 4

Département : Sécurité
Priorité : Haute
Délai estimé : 30 minutes
```

---

## Challenge 28 : Système de réservation de voyage

Une agence propose plusieurs destinations :

```text
1 → Marrakech
2 → Paris
3 → Madrid
4 → Tokyo
5 → New York
```

Utilisez `switch / case`.

Pour chaque destination, définir :

* Prix du billet
* Durée du vol
* Classe disponible

Ensuite, demander :

* Nombre de voyageurs
* Classe choisie
* Nombre de bagages

Calculez le prix final.

---

## Challenge 29 : Gestion d'un abonnement

Une plateforme propose :

```text
1 → Gratuit
2 → Basic
3 → Premium
4 → Business
```

Utilisez `switch / case`.

### Gratuit

```text
Prix : 0 DH
Utilisateurs : 1
Stockage : 1 GB
```

### Basic

```text
Prix : 50 DH
Utilisateurs : 3
Stockage : 10 GB
```

### Premium

```text
Prix : 120 DH
Utilisateurs : 5
Stockage : 50 GB
```

### Business

```text
Prix : 300 DH
Utilisateurs : 20
Stockage : 200 GB
```

Le programme doit afficher les informations de l'abonnement choisi.

**Bonus :**

Ajouter un calcul annuel :

```text
Prix annuel = prix mensuel * 12
```

avec une réduction de `15%` pour le paiement annuel.

---

## Challenge 30 : Terminal de voyage

Vous développez un terminal permettant à un voyageur de choisir une destination.

### Menu principal

```text
1 → Maroc
2 → Europe
3 → Asie
4 → Amérique
```

Utilisez `switch / case`.

Selon le choix, afficher un deuxième menu.

### Maroc

```text
1 → Marrakech
2 → Casablanca
3 → Agadir
```

### Europe

```text
1 → Paris
2 → Madrid
3 → Rome
```

### Asie

```text
1 → Tokyo
2 → Bangkok
3 → Séoul
```

### Amérique

```text
1 → New York
2 → Montréal
3 → São Paulo
```

Le programme doit afficher :

```text
Continent :
Destination :
Prix :
Durée :
```

**Exemple :**

```text
Choix continent : 2

Choix destination : 1

Continent : Europe
Destination : Paris
Prix : 1200 DH
Durée : 3h
```

**Bonus HÉRO :**

Ajouter :

* Classe économique / business
* Nombre de voyageurs
* Nombre de bagages
* Réduction famille
* Réduction membre
* Frais de bagages
* Prix total

---

# Tableau de progression

| #  | Challenge                | Condition   | Niveau    |
| -- | ------------------------ | ----------- | --------- |
| 1  | Tarif de livraison       | `if / else` |  Moyen  |
| 2  | Feu tricolore            | `if / else` |  Moyen  |
| 3  | Calcul d'une remise      | `if / else` |  Moyen  |
| 4  | Validation d'un triangle | `if / else` |  Moyen  |
| 5  | Classement joueur        | `if / else` |  Moyen  |
| 6  | Mois de l'année          | `switch`    |  Moyen  |
| 7  | Compte bancaire          | `switch`    |  Moyen  |
| 8  | Difficulté jeu           | `switch`    |  Moyen  |
| 9  | Billet spectacle         | `switch`    |  Moyen  |
| 10 | Conversion unités        | `switch`    |  Moyen  |
| 11 | Validation date          | `if / else` |  Avancé |
| 12 | Salaire progressif       | `if / else` |  Avancé |
| 13 | Réservation hôtel        | `if / else` |  Avancé |
| 14 | Admission universitaire  | `if / else` |  Avancé |
| 15 | Parking                  | `if / else` |  Avancé |
| 16 | Restaurant               | `switch`    |  Avancé |
| 17 | Calculatrice             | `switch`    |  Avancé |
| 18 | Codes pays               | `switch`    |  Avancé |
| 19 | Transport                | `switch`    |  Avancé |
| 20 | Commandes                | `switch`    |  Avancé |
| 21 | Système bancaire         | `if / else` |  Héro   |
| 22 | Réservation vol          | `if / else` |  Héro   |
| 23 | Mot de passe             | `if / else` |  Héro   |
| 24 | Score jeu                | `if / else` |  Héro   |
| 25 | Feu intelligent          | `if / else` |  Héro   |
| 26 | Paiement                 | `switch`    |  Héro   |
| 27 | Support technique        | `switch`    |  Héro   |
| 28 | Voyage                   | `switch`    |  Héro   |
| 29 | Abonnement               | `switch`    |  Héro   |
| 30 | Terminal voyage          | `switch`    |  Héro   |

---

#  Objectif pédagogique

À travers ces 30 challenges, l'apprenant doit progressivement passer de simples décisions à des **problèmes comportant plusieurs règles métier**.

###  Moyen

L'apprenant doit maîtriser :

```text
if
else if
else
switch
case
default
```

###  Avancé

L'apprenant doit être capable de combiner :

```text
conditions
+
opérateurs logiques
+
calculs
+
plusieurs règles métier
```

###  Héro

L'apprenant doit être capable de :

```text
Analyser le problème
        ↓
Identifier les règles
        ↓
Décomposer le problème
        ↓
Construire les conditions
        ↓
Choisir if/else ou switch
        ↓
Écrire le programme
        ↓
Tester plusieurs scénarios
```

> **Méthode recommandée :** avant d'écrire une seule ligne de JavaScript, l'apprenant doit d'abord écrire les différentes règles du problème sous forme de pseudo-code.
