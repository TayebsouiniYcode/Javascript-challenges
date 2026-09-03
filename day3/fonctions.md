# 10 Challenges JavaScript : Les Fonctions (avec et sans paramètres)

Cette liste de défis est conçue pour consolider vos compétences sur la création et la manipulation des **fonctions en JavaScript**, allant du niveau débutant au niveau avancé.

---

## Niveau Débutant (1 à 3)

### Challenge 1 : Le Salueur Automatique
* **Objectif :** Créer une fonction sans paramètre.
* **Consigne :** Écrivez une fonction nommée `afficherBienvenue` qui ne prend aucun paramètre. Lorsqu'elle est appelée, elle doit afficher dans la console le message : `"Bienvenue dans le cours de JavaScript ! Bonne chance."`.
* **Notions :** Déclaration de fonction, `console.log`.

---

### Challenge 2 : Calculateur d'Âge Canin
* **Objectif :** Créer une fonction avec un paramètre simple.
* **Consigne :** Écrivez une fonction `calculerAgeChien` qui prend un paramètre `ageHumain` (un nombre). La fonction doit calculer et retourner l'âge équivalent du chien (sachant qu'1 an humain ≈ 7 ans de chien).
* **Exemple :** `calculerAgeChien(4)` doit retourner `28`.
* **Notions :** Paramètre, opérations arithmétiques, instruction `return`.

---

### Challenge 3 : Générateur d'Email Professionnel
* **Objectif :** Utiliser une fonction avec plusieurs paramètres.
* **Consigne :** Écrivez une fonction `genererEmail` qui prend deux paramètres : `prenom` et `nom`. La fonction doit retourner une adresse email sous la forme : `prenom.nom@entreprise.com` (tout en minuscules).
* **Exemple :** `genererEmail("Tayeb", "Souini")` ➔ `"tayeb.souini@entreprise.com"`.
* **Notions :** Multiples paramètres, concaténation ou Template Literals (`` ` ``), méthode `.toLowerCase()`.

---

## Niveau Intermédiaire (4 à 7)

### Challenge 4 : Salutation Personnalisée avec Valeur par Défaut
* **Objectif :** Manipuler les valeurs par défaut des paramètres.
* **Consigne :** Écrivez une fonction `saluerClient` qui accepte deux paramètres : `nom` (chaîne de caractères) et `titre` (chaîne de caractères, valeur par défaut : `"Client"`).
    * Si seul le nom est fourni, afficher : `"Bonjour Client [nom]"`.
    * Si les deux sont fournis, afficher : `"Bonjour [titre] [nom]"`.
* **Exemple :** `saluerClient("Dupont")` ➔ `"Bonjour Client Dupont"`.
* **Notions :** Default parameters (paramètres par défaut).

---

### Challenge 5 : Le Somateur Universel (Rest Parameter)
* **Objectif :** Traiter un nombre variable d'arguments.
* **Consigne :** Créez une fonction `additionnerTout` qui accepte n'importe quel nombre d'arguments numériques (sans savoir à l'avance combien) et retourne la somme totale de tous ces nombres.
* **Exemple :** `additionnerTout(10, 20, 30, 40)` ➔ `100`.
* **Notions :** Rest parameters (`...args`), boucles ou méthode `reduce()`.

---

### Challenge 6 : Validateur de Mot de Passe
* **Objectif :** Fonction effectuant des vérifications conditionnelles et retournant un booléen.
* **Consigne :** Écrivez une fonction `verifierMotDePasse` prenant un paramètre `motDePasse`. La fonction doit retourner `true` si le mot de passe contient au moins 8 caractères ET contient le caractère `@`, sinon elle retourne `false`.
* **Exemple :** `verifierMotDePasse("code1234")` ➔ `false`, `verifierMotDePasse("code@1234")` ➔ `true`.
* **Notions :** Conditions, méthodes de String (`.length`, `.includes()`).

---

### Challenge 7 : Horloge / Horodatage Système
* **Objectif :** Créer une fonction sans paramètre retournant des données dynamiques.
* **Consigne :** Écrivez une fonction `obtenirHeureActuelle` sans paramètre qui génère et retourne l'heure courante au format HH:MM:SS.
* **Exemple de sortie :** `"14:30:15"`.
* **Notions :** Objet `Date`, manipulation des méthodes d'heure.

---

## Niveau Avancé / Expert (8 à 10)

### Challenge 8 : Convertisseur Universel de Devises avec Callback
* **Objectif :** Passer une fonction en paramètre d'une autre fonction (Callback).
* **Consigne :** Écrivez une fonction `convertirMontant` qui prend trois paramètres : `montant`, `taux` et une fonction callback `formatter`.
    * La fonction doit multiplier le `montant` par le `taux`, puis passer le résultat à la fonction `formatter` avant de retourner le résultat final.
* **Exemple :** 
  ```javascript
  const formatMAD = (val) => val + " DH";
  convertirMontant(100, 10.5, formatMAD); // Retourne "1050 DH"
  ```
* **Notions :** Callback functions, fonctions de ordre supérieur (Higher-Order Functions).

---

### Challenge 9 : Générateur de Compteur Indépendant (Closure)
* **Objectif :** Retourner une fonction sans paramètre à partir d'une fonction avec paramètre.
* **Consigne :** Écrivez une fonction `creerCompteur` qui prend un paramètre `valeurInitiale` (par défaut `0`). Elle doit retourner une nouvelle fonction (sans paramètre) qui, à chaque appel, incrémente la valeur de 1 et la retourne.
* **Exemple :**
  ```javascript
  const MonCompteur = creerCompteur(10);
  MonCompteur(); // Retourne 11
  MonCompteur(); // Retourne 12
  ```
* **Notions :** Closures, portabilité des variables (lexical scope).

---

### Challenge 10 : Le Pipeline de Transformation de Texte
* **Objectif :** Combiner plusieurs fonctions modulaires avec et sans paramètres.
* **Consigne :** Écrivez :
    1. Une fonction sans paramètre `nettoyerEspaces(texte)` qui retire les espaces au début et à la fin.
    2. Une fonction `mettreEnMajuscule(texte)`.
    3. Une fonction `ajouterPrefixe(texte, prefixe = "LOG:")`.
    4. Une fonction principale `traiterMessage(texte, ...transformations)` qui applique successivement chaque fonction de transformation transmise sur le texte original.
* **Notions :** Composition de fonctions, Rest parameters, modularité avancée.
