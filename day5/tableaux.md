# 20 Challenges JavaScript : Les Tableaux (Arrays)

Deux séries de challenges complémentaires pour vous exercer sur la manipulation des tableaux en JavaScript : 
1. **Sans méthodes prédéfinies** (pour comprendre la logique algorithmique et les boucles).
2. **Avec les méthodes prédéfinies** (pour maîtriser l'écosystème moderne de JavaScript).

---

# PARTIE 1 : 10 Challenges SANS méthodes prédéfinies
*(Interdiction d'utiliser `push`, `pop`, `shift`, `unshift`, `includes`, `indexOf`, `slice`, `splice`, `concat`, `reverse`, `map`, `filter`, `reduce`, `forEach`, etc. Seules la propriété `.length`, l'accès par index `arr[i]` et les boucles `for` / `while` sont autorisées).*

---

### Niveau Débutant

#### Challenge 1 : Parcours et Affichage
* **Consigne :** Écrivez une fonction `afficherElements(tab)` qui parcourt un tableau et affiche chaque élément individuellement dans la console à l'aide d'une boucle.
* **Exemple :** `afficherElements([10, 20, 30])` ➔ Affiche `10`, puis `20`, puis `30`.

#### Challenge 2 : Calculateur de Somme
* **Consigne :** Écrivez une fonction `calculerSomme(tab)` qui prend un tableau de nombres et retourne la somme de tous ses éléments.
* **Exemple :** `calculerSomme([5, 10, 15])` ➔ `30`.

#### Challenge 3 : Recherche du Maximum
* **Consigne :** Écrivez une fonction `trouverMax(tab)` qui retourne le plus grand nombre d'un tableau non vide.
* **Exemple :** `trouverMax([12, 45, 7, 89, 23])` ➔ `89`.

---

### Niveau Intermédiaire

#### Challenge 4 : Ajout à la Fin (Simulation de `push`)
* **Consigne :** Écrivez une fonction `ajouterALaFin(tab, element)` qui ajoute un élément à la fin du tableau passé en paramètre et retourne le tableau modifié (sans utiliser `.push()`).
* **Exemple :** `ajouterALaFin([1, 2, 3], 4)` ➔ `[1, 2, 3, 4]`.

#### Challenge 5 : Recherche d'Élément (Simulation de `includes`)
* **Consigne :** Écrivez une fonction `contientElement(tab, valeur)` qui vérifie si une valeur existe dans le tableau et retourne `true` ou `false`.
* **Exemple :** `contientElement(["pomme", "banane"], "banane")` ➔ `true`.

#### Challenge 6 : Inversion Manuelle (Simulation de `reverse`)
* **Consigne :** Écrivez une fonction `inverserTableau(tab)` qui construit et retourne un nouveau tableau contenant les éléments de `tab` dans l'ordre inverse.
* **Exemple :** `inverserTableau([1, 2, 3, 4])` ➔ `[4, 3, 2, 1]`.

#### Challenge 7 : Filtrage Manuel des Nombres Pairs
* **Consigne :** Écrivez une fonction `filtrerPairs(tab)` qui retourne un nouveau tableau contenant uniquement les nombres pairs présent dans `tab`.
* **Exemple :** `filtrerPairs([1, 2, 3, 4, 5, 6])` ➔ `[2, 4, 6]`.

---

### Niveau Avancé

#### Challenge 8 : Supprimer les Doublons Manuellement
* **Consigne :** Écrivez une fonction `supprimerDoublons(tab)` qui retourne un nouveau tableau contenant les éléments de `tab` sans aucune valeur répétée.
* **Exemple :** `supprimerDoublons([1, 2, 2, 3, 4, 4, 1])` ➔ `[1, 2, 3, 4]`.

#### Challenge 9 : Fusion de Deux Tableaux (Simulation de `concat`)
* **Consigne :** Écrivez une fonction `fusionnerTableaux(tab1, tab2)` qui combine deux tableaux dans un seul nouveau tableau, sans utiliser d'opérateur spread (`...`) ni `.concat()`.
* **Exemple :** `fusionnerTableaux([1, 2], [3, 4])` ➔ `[1, 2, 3, 4]`.

#### Challenge 10 : Tri à Bulles (Bubble Sort)
* **Consigne :** Écrivez une fonction `trierTableau(tab)` qui trie un tableau de nombres par ordre croissant en utilisant l'algorithme du tri à bulles.
* **Exemple :** `trierTableau([5, 3, 8, 1, 2])` ➔ `[1, 2, 3, 5, 8]`.

---
---

# PARTIE 2 : 10 Challenges AVEC méthodes prédéfinies
*(Utilisation recommandée des méthodes courantes : `push`, `pop`, `shift`, `unshift`, `slice`, `splice`, `includes`, `indexOf`, `map`, `filter`, `reduce`, `find`, `some`, `every`, `sort`, `join`, etc.)*

---

### Niveau Débutant

#### Challenge 11 : Formatage de Liste (Chaining & `join`)
* **Consigne :** Écrivez une fonction `formaterChaine(tab)` qui prend un tableau de mots, supprime le premier et le dernier élément, puis joint le reste avec un tiret (`"-"`).
* **Exemple :** `formaterChaine(["Début", "JS", "PHP", "Fin"])` ➔ `"JS-PHP"`.
* **Méthodes suggérées :** `slice()` ou `shift()`/`pop()`, `join()`.

#### Challenge 12 : Élévation au Carré (`map`)
* **Consigne :** Écrivez une fonction `eleverAuCarre(nombres)` qui retourne un nouveau tableau contenant le carré de chaque nombre du tableau d'origine.
* **Exemple :** `eleverAuCarre([2, 4, 6])` ➔ `[4, 16, 36]`.
* **Méthodes suggérées :** `map()`.

#### Challenge 13 : Recherche d'Utilisateur Majeur (`find`)
* **Consigne :** Écrivez une fonction `trouverPremierMajeur(utilisateurs)` qui prend un tableau d'objets `{ nom: string, age: number }` et retourne le premier utilisateur ayant au moins 18 ans.
* **Exemple :** `trouverPremierMajeur([{nom: "Lina", age: 15}, {nom: "Amine", age: 20}])` ➔ `{nom: "Amine", age: 20}`.
* **Méthodes suggérées :** `find()`.

---

### Niveau Intermédiaire

#### Challenge 14 : Filtrage de Produits en Promo (`filter`)
* **Consigne :** Écrivez une fonction `obtenirProduitsEnPromo(produits)` prenant un tableau d'objets `{ nom, prix, enPromo: boolean }` et retournant uniquement un tableau contenant les noms des produits en promotion.
* **Exemple :** `obtenirProduitsEnPromo([{nom: "PC", enPromo: true}, {nom: "Souris", enPromo: false}])` ➔ `["PC"]`.
* **Méthodes suggérées :** `filter()`, `map()`.

#### Challenge 15 : Calcul du Total du Panier (`reduce`)
* **Consigne :** Écrivez une fonction `calculerTotalPanier(panier)` qui calcule le prix total d'un panier d'achats à partir d'un tableau d'objets `{ article: string, prix: number, quantite: number }`.
* **Exemple :** `calculerTotalPanier([{prix: 10, quantite: 2}, {prix: 5, quantite: 1}])` ➔ `25`.
* **Méthodes suggérées :** `reduce()`.

#### Challenge 16 : Validation de Formulaire / Vérification Globale (`every` / `some`)
* **Consigne :** Écrivez une fonction `validerNotes(notes)` qui prend un tableau de notes sur 20 et vérifie :
    1. Si **toutes** les notes sont supérieures ou égales à 10 (`every`).
    2. Si **au moins une** note est égale à 20 (`some`).
    La fonction doit retourner un objet `{ toutesValides: boolean, aUneNoteParfaite: boolean }`.
* **Méthodes suggérées :** `every()`, `some()`.

#### Challenge 17 : Manipulation Ciblée (`splice`)
* **Consigne :** Écrivez une fonction `remplacerElement(tab, ancien, nouveau)` qui cherche un élément dans le tableau et le remplace sur place par la nouvelle valeur en utilisant `.splice()`.
* **Exemple :** `remplacerElement(["A", "B", "C"], "B", "X")` ➔ `["A", "X", "C"]`.
* **Méthodes suggérées :** `indexOf()`, `splice()`.

---

### Niveau Avancé

#### Challenge 18 : Tri Avancé d'Objets (`sort`)
* **Consigne :** Écrivez une fonction `trierParNoteEtNom(etudiants)` qui trie un tableau d'étudiants `{ nom: string, note: number }` par note décroissante. En cas d'égalité de note, trier par ordre alphabétique du nom.
* **Méthodes suggérées :** `sort()`, `localeCompare()`.

#### Challenge 19 : Groupement de Données par Catégorie (`reduce`)
* **Consigne :** Écrivez une fonction `grouperParCategorie(produits)` qui prend un tableau d'objets `{ nom: string, categorie: string }` et retourne un objet où chaque clé est une catégorie contenant le tableau des noms de produits correspondants.
* **Exemple :**
  ```javascript
  grouperParCategorie([
    { nom: "Pomme", categorie: "Fruit" },
    { nom: "Carotte", categorie: "Légume" },
    { nom: "Banane", categorie: "Fruit" }
  ]);
  // Retourne : { Fruit: ["Pomme", "Banane"], Légume: ["Carotte"] }
  ```
* **Méthodes suggérées :** `reduce()`.

#### Challenge 20 : Aplatissement et Nettoyage (`flat`, `flatMap`, `Set`)
* **Consigne :** Écrivez une fonction `nettoyerEtAplatir(tabIndice)` qui prend un tableau à plusieurs niveaux de profondeur contenant des valeurs avec des doublons, l'aplatit complètement et supprime tous les doublons tout en triant le résultat final par ordre croissant.
* **Exemple :** `nettoyerEtAplatir([1, [2, 3, [3, 4]], 2])` ➔ `[1, 2, 3, 4]`.
* **Méthodes suggérées :** `flat(Infinity)`, `Set` / `Array.from()`, `sort()`.