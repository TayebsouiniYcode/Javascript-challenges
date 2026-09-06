# 20 Mises en Situation — Préparation Soutenance SAS

> Niveaux : Moyen et Avancé
> Chaque challenge combine plusieurs concepts : variables/types, conditions (if/else, switch), boucles (for, while, do while, for...in, forEach), fonctions, algorithmes de recherche/tri, et bonus concepts avancés JS.

---

## 1. [Moyen] Gestion des inscriptions à un examen
Une école reçoit une liste de candidats avec leur note d'admission. Écris un programme qui :
- Stocke les candidats dans un tableau d'objets `{ nom, note }`.
- Utilise une **boucle for** pour parcourir la liste et une **condition if/else** pour classer chaque candidat en `"Admis"` (note ≥ 10) ou `"Recalé"`.
- Trie ensuite la liste des admis par note décroissante avec un **tri à bulles**.
- Écris une **fonction** `afficherResultats(liste)` qui affiche le classement final.

## 2. [Moyen] Distributeur automatique de boissons
Simule un distributeur avec un tableau d'objets `{ nom, prix, stock }`. Le programme doit :
- Demander (variable) le nom de la boisson choisie et le montant inséré.
- Utiliser un **switch case** pour déterminer le type de boisson (chaude/froide/soda).
- Vérifier avec une **condition if** si le stock est suffisant et si le montant est suffisant.
- Utiliser une **boucle while** pour rendre la monnaie pièce par pièce (ex : rendre en 5, 2, 1 dh).
- Implémenter une **fonction** `rechercherBoisson(nom)` utilisant une **recherche linéaire**.

## 3. [Moyen] Gestion d'une bibliothèque
Une bibliothèque possède un tableau de livres `{ titre, auteur, disponible }`. Le programme doit :
- Parcourir le tableau avec **forEach** pour afficher les livres disponibles.
- Écrire une **fonction** `emprunterLivre(titre)` qui recherche le livre (**recherche linéaire**) et change son statut si disponible, sinon affiche un message avec **if/else**.
- Trier les livres par ordre alphabétique du titre avec un **tri par sélection**.
- Bonus : utiliser la **déstructuration** pour extraire `titre` et `auteur` lors de l'affichage.

## 4. [Moyen] Calcul de moyennes de classe
Un tableau contient les notes de plusieurs élèves `{ nom, notes: [n1, n2, n3] }`. Le programme doit :
- Utiliser une **boucle for** imbriquée pour calculer la moyenne de chaque élève.
- Utiliser un **switch case** sur la moyenne pour attribuer une mention (`"Excellent"`, `"Bien"`, `"Passable"`, `"Insuffisant"`).
- Trier les élèves par moyenne décroissante (**tri à bulles**).
- Écrire une **fonction** `trouverMeilleurEleve(liste)` sans paramètre supplémentaire qui retourne le premier du classement.

## 5. [Moyen] Vérification de mot de passe
Écris un programme qui vérifie la robustesse d'un mot de passe (variable `string`) :
- Utilise une **boucle for** pour parcourir chaque caractère et détecter la présence de majuscules, minuscules, chiffres.
- Utilise des **conditions if/else** imbriquées pour classer le mot de passe (`"Faible"`, `"Moyen"`, `"Fort"`).
- Écris une **fonction** `verifierMotDePasse(mdp)` avec paramètre qui retourne le résultat.
- Bonus : utilise une **expression régulière simple** ou les méthodes `.includes()`/`.charCodeAt()`.

## 6. [Moyen] Gestion de stock d'un magasin
Un tableau d'objets `{ produit, quantite, prix }` représente le stock. Le programme doit :
- Utiliser une **boucle do while** pour simuler un menu (ajouter, rechercher, afficher, quitter) tant que l'utilisateur ne choisit pas "quitter".
- Implémenter une **recherche linéaire** pour trouver un produit par nom.
- Implémenter un **tri par sélection** pour trier les produits par prix croissant.
- Écrire une **fonction** `calculerValeurStock(stock)` qui retourne la valeur totale (quantité × prix).

## 7. [Moyen] File d'attente d'un guichet
Simule une file d'attente de clients `{ nom, priorite }` (priorite : "normal" ou "urgent"). Le programme doit :
- Utiliser une **boucle for...in** ou **for** pour parcourir la file.
- Utiliser un **switch case** sur la priorité pour déterminer l'ordre de passage.
- Trier la file par priorité puis par ordre d'arrivée (**tri à bulles multi-critères**).
- Écrire une **fonction** `prochainClient(file)` qui retourne le prochain à être servi.

## 8. [Avancé] Système de réservation de places de cinéma
Un tableau de sièges `{ numero, occupe }` (100 sièges) doit être géré :
- Utilise une **boucle for** pour initialiser les sièges (tous libres au départ).
- Écris une **fonction** `reserverSiege(numero)` utilisant une **recherche binaire** (le tableau étant trié par numéro) pour localiser rapidement le siège.
- Utilise **if/else** pour vérifier la disponibilité avant de réserver.
- Bonus : utilise le **spread operator** pour créer une copie du tableau des sièges avant modification (immutabilité).

## 9. [Avancé] Gestion des employés et calcul de salaires
Un tableau d'objets `{ nom, poste, heuresTravaillees, tauxHoraire }` représente les employés. Le programme doit :
- Utiliser une **boucle forEach** pour calculer le salaire de chaque employé (fonction avec paramètres).
- Utiliser un **switch case** sur le poste pour appliquer une prime différente (`"Manager"`, `"Développeur"`, `"Stagiaire"`).
- Trier les employés par salaire décroissant avec un **tri par sélection**.
- Écrire une **fonction récursive ou une fonction fléchée (arrow function)** pour calculer le salaire total de l'entreprise.

## 10. [Avancé] Analyseur de température sur une semaine
Un tableau contient les températures journalières `[t1, t2, ..., t7]`. Le programme doit :
- Utiliser une **boucle for** pour calculer min, max et moyenne.
- Utiliser des **conditions if/else if/else** pour classer chaque journée (`"Froid"`, `"Doux"`, `"Chaud"`, `"Canicule"`).
- Trier les températures avec un **tri à bulles** pour identifier la médiane.
- Écrire une **fonction** `rechercherJourLePlusChaud(temperatures)` utilisant une **recherche linéaire**.
- Bonus : utilise `.map()` et `.filter()` pour extraire les jours chauds directement.

## 11. [Avancé] Système d'authentification simplifié
Un tableau d'objets `{ email, motDePasse, tentatives }` représente les comptes utilisateurs. Le programme doit :
- Implémenter une **recherche binaire** (tableau trié par email) pour retrouver un compte.
- Utiliser une **boucle while** pour gérer les tentatives de connexion (max 3 essais).
- Utiliser **if/else** pour verrouiller le compte après 3 échecs.
- Écrire une **fonction** `authentifier(email, motDePasse)` avec plusieurs paramètres et une valeur de retour booléenne.
- Bonus : utiliser une **closure** pour garder le compteur de tentatives privé.

## 12. [Avancé] Gestionnaire de tâches (To-Do List) avec priorités
Un tableau d'objets `{ tache, priorite, terminee }` doit être géré :
- Utiliser un **switch case** pour attribuer un score numérique à chaque priorité (`"haute"`, `"moyenne"`, `"basse"`).
- Trier les tâches par score de priorité avec un **tri par sélection**.
- Utiliser une **boucle for...in** pour afficher les propriétés de chaque tâche.
- Écrire une **fonction** `filtrerTachesNonTerminees(taches)` bonus avec `.filter()`.
- Écrire une **fonction** `rechercherTache(nomTache)` avec **recherche linéaire**.

## 13. [Avancé] Simulateur de panier d'achat en ligne
Un tableau d'objets `{ produit, prix, quantite, categorie }` représente un panier. Le programme doit :
- Utiliser une **boucle forEach** pour calculer le sous-total de chaque produit (prix × quantité).
- Utiliser un **switch case** sur la catégorie pour appliquer une réduction différente.
- Trier les produits par catégorie puis par prix (**tri à bulles multi-critères**).
- Écrire une **fonction** `calculerTotalPanier(panier)` qui retourne le total après réductions.
- Bonus : utiliser `.reduce()` pour calculer le total en une seule ligne.

## 14. [Avancé] Système de notation d'un tournoi sportif
Un tableau d'objets `{ equipe, victoires, defaites, nuls }` représente le classement. Le programme doit :
- Utiliser une **boucle for** pour calculer les points de chaque équipe (3 pts victoire, 1 pt nul, 0 pt défaite).
- Utiliser **if/else** pour déterminer si une équipe est qualifiée (points ≥ seuil).
- Trier le classement par points décroissants avec un **tri par sélection**.
- Écrire une **fonction** `rechercherEquipe(nom, classement)` avec **recherche linéaire**.
- Bonus : gérer les égalités de points avec un second critère de tri (différence de buts).

## 15. [Avancé] Gestion d'un parking intelligent
Un tableau d'objets `{ place, occupee, typeVehicule }` (places numérotées et triées). Le programme doit :
- Utiliser une **boucle do while** pour simuler l'arrivée de véhicules tant qu'il reste de la place.
- Utiliser un **switch case** sur le type de véhicule (`"voiture"`, `"moto"`, `"camion"`) pour déterminer la zone assignée.
- Implémenter une **recherche binaire** pour trouver rapidement une place libre par numéro.
- Écrire une **fonction** `libererPlace(numero)` avec paramètre.
- Bonus : utiliser une fonction fléchée pour compter le nombre de places libres avec `.filter()`.

## 16. [Avancé] Correcteur automatique de quiz
Un tableau d'objets `{ question, reponseCorrecte, reponseEtudiant }` représente les réponses d'un étudiant à un quiz. Le programme doit :
- Utiliser une **boucle for** pour comparer chaque réponse et calculer le score.
- Utiliser des **conditions if/else if/else** pour attribuer une appréciation selon le score (`"Excellent"`, `"Bon"`, `"À revoir"`).
- Écrire une **fonction** `corrigerQuiz(reponses)` qui retourne le score final.
- Trier les questions par difficulté (si un champ `difficulte` est ajouté) avec un **tri à bulles**.
- Bonus : utiliser `.every()` pour vérifier si toutes les réponses sont correctes.

## 17. [Avancé] Système de recommandation de films
Un tableau d'objets `{ titre, genre, note, annee }` représente un catalogue de films. Le programme doit :
- Utiliser une **boucle forEach** pour filtrer les films selon un genre donné (variable).
- Utiliser un **switch case** sur le genre pour afficher un message personnalisé.
- Trier les films filtrés par note décroissante avec un **tri par sélection**.
- Écrire une **fonction** `rechercherFilmParTitre(titre, catalogue)` utilisant une **recherche binaire** (catalogue trié par titre).
- Bonus : utiliser le **spread operator** pour fusionner deux catalogues de films sans doublons.

## 18. [Avancé] Simulateur de facturation d'un hôtel
Un tableau d'objets `{ client, typeChambre, nombreNuits }` représente les réservations. Le programme doit :
- Utiliser un **switch case** sur le type de chambre (`"simple"`, `"double"`, `"suite"`) pour déterminer le prix par nuit.
- Utiliser une **boucle for** pour calculer la facture totale de chaque client.
- Utiliser **if/else** pour appliquer une remise si `nombreNuits > 7`.
- Trier les factures par montant décroissant (**tri à bulles**).
- Écrire une **fonction** `rechercherClient(nom, reservations)` avec **recherche linéaire**.

## 19. [Avancé] Gestion des votes d'une élection
Un tableau d'objets `{ candidat, votes }` représente les résultats d'un scrutin. Le programme doit :
- Utiliser une **boucle for...in** ou **forEach** pour calculer le total des votes exprimés.
- Utiliser des **conditions if/else** pour déterminer le vainqueur (majorité simple).
- Trier les candidats par nombre de votes décroissant avec un **tri par sélection**.
- Écrire une **fonction** `calculerPourcentage(votes, totalVotes)` avec paramètres qui retourne un pourcentage.
- Bonus : utiliser `.reduce()` pour calculer le total des votes en une ligne, et gérer une égalité (ex tie-break) avec une condition supplémentaire.

## 20. [Avancé] Assistant de planification d'emploi du temps
Un tableau d'objets `{ cours, jour, heureDebut, heureFin }` représente un emploi du temps. Le programme doit :
- Utiliser une **boucle while** pour vérifier s'il existe un chevauchement d'horaires entre deux cours.
- Utiliser un **switch case** sur le jour de la semaine pour organiser l'affichage.
- Trier les cours par jour puis par heure de début (**tri à bulles multi-critères**).
- Écrire une **fonction** `rechercherCoursParNom(nom, emploiDuTemps)` avec **recherche linéaire**.
- Bonus : utiliser une **fonction récursive** ou une **closure** pour générer un identifiant unique auto-incrémenté pour chaque cours ajouté.

---

### 💡 Concepts avancés bonus à explorer (transversaux)
- Déstructuration (objets et tableaux)
- Spread/Rest operator
- Fonctions fléchées (arrow functions)
- Closures
- Méthodes de tableaux : `.map()`, `.filter()`, `.reduce()`, `.every()`, `.some()`, `.find()`
- Fonctions récursives
- Template literals