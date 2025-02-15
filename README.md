# Devoir Maison - Programmation Orientée Objet

## Cahier des Charges

### Classe `Carte`

- [ ] **Attributs et méthodes de classe** :
  - [ ] Définir les attributs privés de classe `VALEURS` et `COULEURS`.
  - [ ] Implémenter les méthodes de classe `VALEURS()` et `COULEURS()` pour accéder aux valeurs des attributs.

- [ ] **Attributs d'instance et propriétés** :
  - [ ] Définir les attributs privés `valeur` et `couleur`.
  - [ ] Créer des propriétés pour accéder à `valeur` et `couleur` sans permettre leur modification.

- [ ] **Méthode `__init__()`** :
  - [ ] Implémenter le constructeur pour vérifier les valeurs des arguments et lever des erreurs si elles ne sont pas valides.

- [ ] **Méthode `__str__()`** :
  - [ ] Implémenter la méthode pour renvoyer la représentation informelle de la carte (ex: "As de cœur").

- [ ] **Méthode `__repr__()`** :
  - [ ] Implémenter la méthode pour renvoyer la représentation officielle de la carte (ex: `Carte('As', 'Coeur')`).

- [ ] **Méthode `__eq__()`** :
  - [ ] Implémenter la méthode pour vérifier l'égalité entre deux cartes.

- [ ] **Méthode `__hash__()`** :
  - [ ] Implémenter la méthode pour rendre les cartes hachables.

### Classe `Combinaison`

- [ ] **Attribut d'instance et propriété** :
  - [ ] Définir l'attribut privé `cartes`.
  - [ ] Créer une propriété pour accéder à une copie profonde de `cartes`.

- [ ] **Méthode `__init__()`** :
  - [ ] Implémenter le constructeur pour vérifier l'intégrité de l'argument et lever une erreur si nécessaire.

- [ ] **Méthode `__eq__()`** :
  - [ ] Implémenter la méthode pour vérifier l'égalité entre deux combinaisons.

- [ ] **Méthode `__str__()`** :
  - [ ] Implémenter la méthode pour renvoyer la représentation informelle de la combinaison.

- [ ] **Méthode `est_brelan()`** :
  - [ ] Implémenter la méthode pour déterminer si la combinaison est un brelan.

- [ ] **Méthode `est_carre()`** :
  - [ ] Implémenter la méthode pour déterminer si la combinaison est un carré.

- [ ] **Méthode `est_sequence()`** :
  - [ ] Implémenter la méthode pour déterminer si la combinaison est une séquence.

- [ ] **Méthode `est_valide()`** :
  - [ ] Implémenter la méthode pour déterminer si la combinaison est valide.

- [ ] **Méthode `calcule_nombre_points()`** :
  - [ ] Implémenter la méthode pour calculer le nombre de points d'une combinaison valide.

### Classe `_ListeCartes`

- [ ] **Attribut d'instance et propriété** :
  - [ ] Définir l'attribut privé `cartes`.
  - [ ] Créer une propriété pour accéder à une copie profonde de `cartes`.

- [ ] **Méthode `__init__()`** :
  - [ ] Implémenter le constructeur pour vérifier l'intégrité de l'argument et lever une erreur si nécessaire.

- [ ] **Méthode `__eq__()`** :
  - [ ] Implémenter la méthode pour vérifier l'égalité entre deux listes de cartes.

- [ ] **Méthode `__str__()`** :
  - [ ] Implémenter la méthode pour renvoyer la représentation informelle de la liste de cartes.

- [ ] **Méthode `__len__()`** :
  - [ ] Implémenter la méthode pour renvoyer le nombre de cartes dans la liste.

- [ ] **Méthode `melanger()`** :
  - [ ] Implémenter la méthode pour mélanger les cartes.

- [ ] **Méthode `ajouter_carte()`** :
  - [ ] Implémenter la méthode pour ajouter une carte à la fin de la liste.

- [ ] **Méthode `retirer_carte()`** :
  - [ ] Implémenter la méthode pour retirer une carte de la liste et la renvoyer.

### Classe `Reserve`

- [ ] **Méthode `__init__()`** :
  - [ ] Implémenter le constructeur en appelant le constructeur de la classe mère `_ListeCartes`.

- [ ] **Méthode `distribuer()`** :
  - [ ] Implémenter la méthode pour distribuer les cartes aux joueurs en début de partie.

### Classe `Defausse`

- [ ] **Méthode `__init__()`** :
  - [ ] Implémenter le constructeur en appelant le constructeur de la classe mère `_ListeCartes`.

- [ ] **Méthode `vider()`** :
  - [ ] Implémenter la méthode pour vider la défausse et l'ajouter à la fin de la réserve après mélange.

### Classe `Main`

- [ ] **Méthode `__init__()`** :
  - [ ] Implémenter le constructeur en appelant le constructeur de la classe mère `_ListeCartes`.

- [ ] **Méthode `__eq__()`** :
  - [ ] Implémenter la méthode pour vérifier l'égalité entre deux mains.

- [ ] **Méthode `piocher()`** :
  - [ ] Implémenter la méthode pour piocher la première carte de la réserve.

- [ ] **Méthode `jeter()`** :
  - [ ] Implémenter la méthode pour jeter une carte de la main dans la défausse.

- [ ] **Méthode `poser()`** :
  - [ ] Implémenter la méthode pour poser des combinaisons de cartes.

## Tests

- [ ] **Tests pour `Carte`** :
  - [ ] Implémenter les tests pour la classe `Carte`.

- [ ] **Tests pour `Combinaison`** :
  - [ ] Implémenter les tests pour la classe `Combinaison`.

- [ ] **Tests pour `_ListeCartes`** :
  - [ ] Implémenter les tests pour la classe `_ListeCartes`.

- [ ] **Tests pour `Reserve`** :
  - [ ] Implémenter les tests pour la classe `Reserve`.

- [ ] **Tests pour `Defausse`** :
  - [ ] Implémenter les tests pour la classe `Defausse`.

- [ ] **Tests pour `Main`** :
  - [ ] Implémenter les tests pour la classe `Main`.

## Documentation

- [ ] **Documentation des classes et méthodes** :
  - [ ] Documenter chaque classe et méthode avec une description courte, les paramètres et les retours.

## Style de code

- [ ] **Vérification avec Flake8** :
  - [ ] Exécuter Flake8 pour vérifier le style de code et corriger les erreurs.

- [ ] **Formatage avec Black** :
  - [ ] Utiliser Black pour formater le code.

## Tests de couverture

- [ ] **Vérification de la couverture des tests** :
  - [ ] Utiliser `pytest-cov` pour vérifier que tout le code est couvert par les tests.

## Rendu

- [ ] **Archivage du dossier `src`** :
  - [ ] Compresser le dossier `src` en `.zip` ou `.7z` et le déposer sur Moodle.
