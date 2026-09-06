# Challenges JavaScript — Recherche Binaire/Linéaire & Tri à Bulles/Sélection

> Progression de difficulté : Facile → Facile-Moyen → Moyen → Avancé → Héro
> 3 groupes de 5 challenges : Entiers, Chaînes de caractères, Objets

---

## Groupe 1 — Tableaux d'entiers

### 1. [Facile] Recherche linéaire simple
Étant donné :
```js
let nombres = [4, 8, 15, 16, 23, 42];
```
Écris une fonction qui recherche un nombre donné dans le tableau et retourne `true`/`false` selon qu'il existe ou non.

### 2. [Facile-Moyen] Tri à bulles croissant
Étant donné :
```js
let notes = [12, 5, 19, 3, 27, 8, 14];
```
Trie le tableau par ordre croissant en utilisant l'algorithme du tri à bulles (sans utiliser `.sort()`).

### 3. [Moyen] Recherche binaire avec index
Étant donné (déjà trié) :
```js
let ids = [2, 7, 11, 15, 23, 34, 45, 58, 61, 70];
```
Écris une fonction de recherche binaire qui retourne l'**index** de la valeur cherchée, ou `-1` si elle n'existe pas.

### 4. [Avancé] Tri par sélection décroissant + compteur d'échanges
Étant donné :
```js
let temperatures = [22, 19, 30, 15, 28, 17, 25];
```
Trie le tableau par ordre **décroissant** avec le tri par sélection, et affiche le **nombre total d'échanges (swaps)** effectués pendant le tri.

### 5. [Héro] Recherche binaire sur tableau presque trié avec doublons
Étant donné :
```js
let scores = [3, 3, 7, 7, 7, 12, 19, 19, 25, 30, 30, 30, 41];
```
Écris une fonction de recherche binaire qui retourne **le premier index** et **le dernier index** où une valeur donnée apparaît (ex : pour `7` → premier index et dernier index de son occurrence).

---

## Groupe 2 — Tableaux de chaînes de caractères

### 6. [Facile] Recherche linéaire d'un mot
Étant donné :
```js
let fruits = ["pomme", "banane", "cerise", "mangue", "kiwi"];
```
Écris une fonction qui recherche un fruit donné et retourne sa position, ou un message indiquant qu'il n'existe pas.

### 7. [Facile-Moyen] Tri à bulles alphabétique
Étant donné :
```js
let prenoms = ["Youssef", "Amina", "Karim", "Salma", "Hicham"];
```
Trie le tableau par ordre alphabétique avec le tri à bulles.

### 8. [Moyen] Recherche binaire insensible à la casse
Étant donné (trié alphabétiquement) :
```js
let mots = ["ananas", "citron", "datte", "figue", "grenade", "kiwi", "mangue"];
```
Écris une fonction de recherche binaire qui trouve un mot **sans tenir compte de la casse** (ex : chercher "FIGUE" doit trouver "figue").

### 9. [Avancé] Tri par sélection selon la longueur
Étant donné :
```js
let villes = ["Rabat", "Casablanca", "Fès", "Youssoufia", "Safi", "Marrakech"];
```
Trie le tableau selon la **longueur des chaînes** (du plus court au plus long) avec le tri par sélection. En cas d'égalité de longueur, garde l'ordre alphabétique.

### 10. [Héro] Recherche binaire par préfixe
Étant donné (trié) :
```js
let dictionnaire = ["abricot", "amande", "ananas", "banane", "cerise", "citron", "datte", "figue"];
```
Écris une fonction de recherche binaire qui retourne **tous les mots** commençant par un préfixe donné (ex : préfixe "a" → `["abricot", "amande", "ananas"]`).

---

##  Groupe 3 — Tableaux d'objets

### 11. [Facile] Recherche linéaire d'un utilisateur par ID
Étant donné :
```js
let utilisateurs = [
  { id: 1, nom: "Sara" },
  { id: 2, nom: "Omar" },
  { id: 3, nom: "Nadia" },
  { id: 4, nom: "Yassine" }
];
```
Écris une fonction qui recherche un utilisateur par son `id` et retourne l'objet correspondant, ou `null` s'il n'existe pas.

### 12. [Facile-Moyen] Tri à bulles par âge
Étant donné :
```js
let etudiants = [
  { nom: "Ali", age: 22 },
  { nom: "Fatima", age: 19 },
  { nom: "Reda", age: 25 },
  { nom: "Imane", age: 21 }
];
```
Trie le tableau par `age` croissant avec le tri à bulles.

### 13. [Moyen] Recherche binaire sur objets triés par clé
Étant donné (déjà trié par `code`) :
```js
let produits = [
  { code: "A012", nom: "Clavier" },
  { code: "B045", nom: "Souris" },
  { code: "C078", nom: "Écran" },
  { code: "D101", nom: "Casque" },
  { code: "E134", nom: "Webcam" }
];
```
Écris une fonction de recherche binaire qui retourne le produit correspondant à un `code` donné.

### 14. [Avancé] Tri par sélection multi-critères
Étant donné :
```js
let commandes = [
  { categorie: "Électronique", prix: 450 },
  { categorie: "Alimentation", prix: 30 },
  { categorie: "Électronique", prix: 120 },
  { categorie: "Vêtement", prix: 80 },
  { categorie: "Alimentation", prix: 15 }
];
```
Trie le tableau d'abord par `categorie` (ordre alphabétique), puis par `prix` croissant à l'intérieur de chaque catégorie, en utilisant le tri par sélection.

### 15. [Héro] Recherche binaire + tri combinés sur clé composée
Étant donné :
```js
let employes = [
  { departement: "RH", matricule: 1023, nom: "Nizar" },
  { departement: "IT", matricule: 2044, nom: "Salma" },
  { departement: "IT", matricule: 2011, nom: "Hamza" },
  { departement: "Finance", matricule: 3007, nom: "Laila" },
  { departement: "RH", matricule: 1002, nom: "Adil" }
];
```
1. Trie d'abord le tableau par `departement` puis par `matricule` (avec le tri par sélection).
2. Écris ensuite une fonction de recherche binaire qui retrouve un employé à partir d'une clé composée `departement + matricule`, en exploitant le tri effectué à l'étape précédente.