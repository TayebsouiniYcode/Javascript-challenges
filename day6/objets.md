# JavaScript — Challenges Objets & Tableaux d'Objets

## Objectifs

- Créer et manipuler des objets
- Accéder et modifier des propriétés
- Parcourir un tableau d'objets
- Rechercher dans un tableau d'objets
- Utiliser conditions, boucles et fonctions avec les objets
- Découvrir `filter()`, `find()`, `map()` et `reduce()` en bonus

---

# Partie 1 — Les Objets

## Challenge 01 — Profil étudiant

**Niveau : 1 **

Créez un objet `student` avec les propriétés :

- `firstName`
- `lastName`
- `age`
- `city`
- `school`

### Travail demandé

1. Créer l'objet.
2. Afficher le prénom.
3. Afficher le nom.
4. Afficher l'âge.
5. Afficher la ville.
6. Afficher une phrase contenant plusieurs propriétés.

### Exemple de résultat

```text
Prénom : Yassine
Nom : Amrani
Age : 21
Ville : Youssoufia

Yassine Amrani a 21 ans et habite à Youssoufia.
```

---

## Challenge 02 — Modifier un profil

**Niveau : 1 **

```javascript
let user = {
    username: "Ahmed",
    age: 22,
    city: "Marrakech",
    status: "student"
};
```

### Travail demandé

1. Afficher le `username`.
2. Afficher l'âge.
3. Modifier l'âge.
4. Modifier la ville.
5. Modifier le `status`.
6. Ajouter une propriété `email`.
7. Afficher toutes les informations.

---

## Challenge 03 — Produit

**Niveau : 1 **

Créez un objet `product` avec :

- `name`
- `price`
- `category`
- `quantity`
- `available`

### Travail demandé

1. Afficher le nom.
2. Afficher le prix.
3. Afficher la catégorie.
4. Vérifier si le produit est disponible.
5. Calculer le prix total du stock.

---

## Challenge 04 — Calculateur de salaire

**Niveau : 2 **

```javascript
let employee = {
    firstName: "Sara",
    lastName: "Amrani",
    salary: 7000,
    bonus: 1000,
    absenceDays: 2
};
```

Une pénalité de `200 DH` est appliquée par jour d'absence.

### Travail demandé

Calculer :

1. Le salaire de base.
2. Le bonus.
3. Les pénalités.
4. Le salaire final.

```text
Salaire final = salaire + bonus - pénalités
```

---

## Challenge 05 — Gestion d'un compte bancaire

**Niveau : 2 **

```javascript
let account = {
    owner: "Tayeb",
    balance: 5000,
    type: "saving"
};
```

### Travail demandé

Créer des fonctions permettant de :

1. Afficher le solde.
2. Déposer de l'argent.
3. Retirer de l'argent.
4. Vérifier si le solde est suffisant.
5. Afficher les informations du compte.

### Contraintes

- Un retrait supérieur au solde doit être refusé.
- Un montant négatif doit être refusé.
- Utiliser `return` lorsque cela est pertinent.

---

# Partie 2 — Tableaux d'Objets

## Challenge 06 — Liste des étudiants

**Niveau : 1 **

```javascript
let students = [
    {
        firstName: "Ali",
        age: 20,
        city: "Youssoufia"
    },
    {
        firstName: "Sara",
        age: 22,
        city: "Marrakech"
    },
    {
        firstName: "Omar",
        age: 19,
        city: "Safi"
    }
];
```

### Travail demandé

1. Afficher tous les étudiants.
2. Afficher uniquement leurs prénoms.
3. Afficher leur âge.
4. Afficher une phrase pour chaque étudiant.

---

## Challenge 07 — Notes des étudiants 

**Niveau : 2 **

```javascript
let students = [
    { name: "Ali", note: 15 },
    { name: "Sara", note: 8 },
    { name: "Omar", note: 17 },
    { name: "Imane", note: 11 },
    { name: "Yassine", note: 6 }
];
```

### Travail demandé

Parcourir le tableau et :

1. Afficher chaque étudiant.
2. Afficher sa note.
3. Afficher `Admis` si la note est >= 10.
4. Afficher `Non admis` sinon.
5. Compter les étudiants admis.
6. Compter les étudiants non admis.

---

## Challenge 08 — Recherche d'un étudiant

**Niveau : 2 **

```javascript
let students = [
    { id: 1, name: "Ali", age: 20 },
    { id: 2, name: "Sara", age: 22 },
    { id: 3, name: "Omar", age: 19 },
    { id: 4, name: "Imane", age: 21 }
];
```

### Travail demandé

Demander à l'utilisateur un `id` puis rechercher l'étudiant correspondant.

### Si l'étudiant existe

```text
Étudiant trouvé !

ID : 3
Nom : Omar
Age : 19
```

### Sinon

```text
Aucun étudiant trouvé avec cet ID.
```

### Bonus

Créer :

```javascript
rechercherEtudiant(id)
```

La fonction doit retourner l'étudiant trouvé ou une valeur indiquant qu'il n'existe pas.

---

## Challenge 09 — Recherche avancée

**Niveau : 3 **

```javascript
let products = [
    {
        id: 1,
        name: "Laptop",
        category: "Informatique",
        price: 7500
    },
    {
        id: 2,
        name: "Phone",
        category: "Smartphone",
        price: 3500
    },
    {
        id: 3,
        name: "Keyboard",
        category: "Informatique",
        price: 500
    },
    {
        id: 4,
        name: "Monitor",
        category: "Informatique",
        price: 2200
    }
];
```

### Travail demandé

Créer un programme permettant de rechercher un produit selon :

1. Son `id`.
2. Son `name`.
3. Sa `category`.
4. Son prix maximum.

Créer les fonctions :

```javascript
rechercherParId()
rechercherParNom()
rechercherParCategorie()
rechercherParPrix()
```

---

# Challenge 10 — Student Manager

**Niveau : 4 **

Créez un petit système de gestion d'une classe.

```javascript
let students = [
    {
        id: 1,
        name: "Ali",
        age: 21,
        city: "Youssoufia",
        note: 15
    },
    {
        id: 2,
        name: "Sara",
        age: 22,
        city: "Marrakech",
        note: 17
    },
    {
        id: 3,
        name: "Omar",
        age: 20,
        city: "Safi",
        note: 8
    },
    {
        id: 4,
        name: "Imane",
        age: 23,
        city: "Youssoufia",
        note: 12
    },
    {
        id: 5,
        name: "Yassine",
        age: 19,
        city: "Safi",
        note: 9
    }
];
```

## Menu

```text
=============================
     STUDENT MANAGER
=============================

1. Afficher tous les étudiants
2. Rechercher un étudiant
3. Rechercher par ville
4. Afficher les étudiants admis
5. Afficher les étudiants non admis
6. Afficher le meilleur étudiant
7. Afficher la moyenne de la classe
8. Quitter

Votre choix :
```

## Travail demandé

### Option 1
Afficher tous les étudiants.

### Option 2
Rechercher un étudiant par son `id`.

### Option 3
Rechercher tous les étudiants d'une ville.

### Option 4
Afficher les étudiants ayant une note >= 10.

### Option 5
Afficher les étudiants ayant une note < 10.

### Option 6
Trouver l'étudiant ayant la meilleure note.

### Option 7
Calculer la moyenne générale de la classe.

### Option 8
Quitter le programme.

## Contraintes

Votre programme doit utiliser :

- Objets
- Tableaux d'objets
- Variables
- Conditions
- `switch`
- `for` ou `while`
- `do...while`
- Fonctions
- Paramètres
- `return`
- `break`

---

#  Bonus

## Bonus 1

Créer :

```javascript
afficherEtudiant(student)
```

## Bonus 2

Créer :

```javascript
rechercherEtudiant(id)
```

qui retourne l'étudiant.

## Bonus 3

Créer :

```javascript
calculerMoyenne()
```

qui retourne la moyenne de la classe.

## Bonus 4 — Apprenants excellents

Résoudre certaines recherches avec :

```javascript
filter()
```

```javascript
find()
```

```javascript
map()
```

```javascript
reduce()
```

Comparer ensuite avec une solution utilisant une boucle `for`.

---


#  Méthode de résolution

Pour chaque challenge :

1. Comprendre le problème.
2. Identifier les données.
3. Identifier les traitements nécessaires.
4. Écrire un pseudo-code.
5. Écrire le code JavaScript.
6. Tester avec plusieurs valeurs.
7. Améliorer la solution.

> Ne cherchez pas immédiatement la solution sur Internet.
> Essayez d'abord de résoudre le problème avec les concepts que vous connaissez.
