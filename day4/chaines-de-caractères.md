# 20 Challenges JavaScript : Les Chaînes de Caractères (Strings)

Voici deux séries de 10 challenges sur la manipulation des chaînes de caractères en JavaScript : 
1. **Sans méthodes prédéfinies** (manipulation algorithmique brute via des boucles et des indices).
2. **Avec les méthodes prédéfinies** (utilisation moderne avec les méthodes de l'objet `String`).

---

# PARTIE 1 : 10 Challenges SANS méthodes prédéfinies
*(Interdiction d'utiliser `split`, `join`, `slice`, `substring`, `includes`, `indexOf`, `toUpperCase`, `toLowerCase`, `replace`, `trim`, etc. Seules la propriété `.length`, l'accès par index `chaine[i]` et les boucles `for` / `while` sont autorisées).*

---

###  Niveau Débutant

#### Challenge 1 : Compteur de Caractères
* **Consigne :** Écrivez une fonction `compterCaracteres(chaine)` qui parcourt une chaîne et retourne le nombre total de caractères qu'elle contient (sans utiliser `.length`).
* **Exemple :** `compterCaracteres("Code")` ➔ `4`.

#### Challenge 2 : Compteur d'Occurrences d'un Caractère
* **Consigne :** Écrivez une fonction `compterLettre(chaine, lettre)` qui compte combien de fois un caractère spécifique apparaît dans une chaîne.
* **Exemple :** `compterLettre("javascript", "a")` ➔ `2`.

#### Challenge 3 : Inverseur de Chaîne
* **Consigne :** Écrivez une fonction `inverserChaine(chaine)` qui construit et retourne une nouvelle chaîne avec les caractères dans l'ordre inverse.
* **Exemple :** `inverserChaine("hello")` ➔ `"olleh"`.

---

###  Niveau Intermédiaire

#### Challenge 4 : Compteur de Voyelles
* **Consigne :** Écrivez une fonction `compterVoyelles(chaine)` qui retourne le nombre de voyelles (a, e, i, o, u, y) présentes dans une chaîne en minuscules.
* **Exemple :** `compterVoyelles("developpeur")` ➔ `5`.

#### Challenge 5 : Test de Palindrome
* **Consigne :** Écrivez une fonction `estPalindrome(chaine)` qui vérifie si un mot se lit de la même façon dans les deux sens (ex: "radar", "kayak"). La fonction doit retourner `true` ou `false`.
* **Exemple :** `estPalindrome("kayak")` ➔ `true`.

#### Challenge 6 : Duplication de Chaîne (Simulation de `repeat`)
* **Consigne :** Écrivez une fonction `repeterChaine(chaine, fois)` qui construit une chaîne en répétant le texte donné le nombre de fois spécifié.
* **Exemple :** `repeterChaine("JS", 3)` ➔ `"JSJSJS"`.

#### Challenge 7 : Remplacement Manuel d'un Caractère
* **Consigne :** Écrivez une fonction `remplacerCaractere(chaine, ancien, nouveau)` qui remplace toutes les apparitions d'un caractère `ancien` par `nouveau`.
* **Exemple :** `remplacerCaractere("banana", "a", "o")` ➔ `"bonono"`.

---

###  Niveau Avancé

#### Challenge 8 : Extraction Manuelle de Sous-chaîne (Simulation de `slice`)
* **Consigne :** Écrivez une fonction `extraireChaine(chaine, debut, fin)` qui extrait les caractères situés entre l'indice `debut` (inclus) et l'indice `fin` (exclus).
* **Exemple :** `extraireChaine("JavaScript", 0, 4)` ➔ `"Java"`.

#### Challenge 9 : Suppression des Espaces Extérieurs (Simulation de `trim`)
* **Consigne :** Écrivez une fonction `nettoyerEspaces(chaine)` qui retire tous les espaces situés au tout début et à la toute fin d'une chaîne, sans toucher aux espaces du milieu.
* **Exemple :** `nettoyerEspaces("   hello world   ")` ➔ `"hello world"`.

#### Challenge 10 : Découpage Manuel en Mots (Simulation de `split(' ')`)
* **Consigne :** Écrivez une fonction `separerMots(chaine)` qui prend une phrase avec des espaces et retourne un tableau contenant chaque mot individuel.
* **Exemple :** `separerMots("Apprendre le JavaScript")` ➔ `["Apprendre", "le", "JavaScript"]`.

---
---

# PARTIE 2 : 10 Challenges AVEC méthodes prédéfinies
*(Utilisation des méthodes natives : `slice`, `substring`, `split`, `includes`, `indexOf`, `startsWith`, `endsWith`, `toUpperCase`, `toLowerCase`, `replace`, `replaceAll`, `trim`, `padStart`, `padEnd`, etc.)*

---

### Niveau Débutant

#### Challenge 11 : Mise en Majuscules et Minuscules
* **Consigne :** Écrivez une fonction `formaterTexte(chaine)` qui prend une chaîne et retourne un objet `{ majuscule: string, minuscule: string }`.
* **Exemple :** `formaterTexte("Code")` ➔ `{ majuscule: "CODE", minuscule: "code" }`.
* **Méthodes suggérées :** `toUpperCase()`, `toLowerCase()`.

#### Challenge 12 : Vérification de Domaine Email
* **Consigne :** Écrivez une fonction `verifierEmail(email)` qui vérifie si une adresse email se termine par `"@gmail.com"`.
* **Exemple :** `verifierEmail("test@gmail.com")` ➔ `true`.
* **Méthodes suggérées :** `endsWith()`, `includes()`.

#### Challenge 13 : Extraction des Initiales
* **Consigne :** Écrivez une fonction `obtenirInitiales(nomComplet)` qui prend un nom complet (ex: `"Tayeb Souini"`) et retourne les initiales en majuscules séparées par un point.
* **Exemple :** `obtenirInitiales("tayeb souini")` ➔ `"T.S"`.
* **Méthodes suggérées :** `split()`, `toUpperCase()`, `map()`, `join()`.

---

### Niveau Intermédiaire

#### Challenge 14 : Masquage de Carte Bancaire
* **Consigne :** Écrivez une fonction `masquerCarte(numeroCarte)` qui prend un numéro de carte à 16 chiffres sous forme de chaîne et remplace tous les chiffres sauf les 4 derniers par des étoiles (`*`).
* **Exemple :** `masquerCarte("1234567812345678")` ➔ `"************5678"`.
* **Méthodes suggérées :** `slice()`, `padStart()`.

#### Challenge 15 : Capitaliser la Première Lettre de Chaque Mot
* **Consigne :** Écrivez une fonction `capitaliserPhrase(phrase)` qui transforme la première lettre de chaque mot d'une phrase en majuscule.
* **Exemple :** `capitaliserPhrase("bienvenue au cours")` ➔ `"Bienvenue Au Cours"`.
* **Méthodes suggérées :** `split()`, `map()`, `slice()`, `toUpperCase()`, `join()`.

#### Challenge 16 : Censure de Mots Interdits
* **Consigne :** Écrivez une fonction `censurerTexte(texte, motsInterdits)` qui prend un texte et un tableau de mots interdits, puis remplace chaque mot interdit trouvé par `"***"`.
* **Exemple :** `censurerTexte("Ce code est mauvais et lent", ["mauvais", "lent"])` ➔ `"Ce code est *** et ***"`.
* **Méthodes suggérées :** `replaceAll()` ou `reduce()`.

#### Challenge 17 : Conversion en Format Slug URL
* **Consigne :** Écrivez une fonction `genererSlug(titre)` qui transforme un titre en slug lisible pour une URL (en minuscules, sans espaces au début/fin, et en remplaçant les espaces par des tirets).
* **Exemple :** `genererSlug("  Mon Premier Article JS  ")` ➔ `"mon-premier-article-js"`.
* **Méthodes suggérées :** `trim()`, `toLowerCase()`, `replaceAll()` ou `split().join()`.

---

### Niveau Avancé

#### Challenge 18 : Analyseur de Fréquence des Mots
* **Consigne :** Écrivez une fonction `analyserMots(phrase)` qui prend un texte, retire la ponctuation de base (points, virgules), convertit en minuscules et retourne un objet contenant la fréquence de chaque mot.
* **Exemple :** `analyserMots("Le chat mange, le chat dort.")` ➔ `{ le: 2, chat: 2, mange: 1, dort: 1 }`.
* **Méthodes suggérées :** `toLowerCase()`, `replaceAll()`, `split()`, `reduce()`.

#### Challenge 19 : Validation de Format de Téléphone
* **Consigne :** Écrivez une fonction `validerTelephone(numero)` qui vérifie si un numéro respecte le format `"06-XX-XX-XX-XX"` ou `"07-XX-XX-XX-XX"` (longueur exacte, tirets aux bons endroits, commence par 06 ou 07).
* **Méthodes suggérées :** `startsWith()`, `split()`, `length`, `every()`.

#### Challenge 20 : Compteur de Chiffres et Lettres
* **Consigne :** Écrivez une fonction `analyserComposition(chaine)` qui prend une chaîne alphanumérique et retourne un objet indiquant le nombre exact de lettres, le nombre de chiffres et le nombre de symboles/espaces.
* **Exemple :** `analyserComposition("Code123!")` ➔ `{ lettres: 4, chiffres: 3, symboles: 1 }`.
* **Méthodes suggérées :** `split()`, `filter()`, conversion ou expressions régulières simples.