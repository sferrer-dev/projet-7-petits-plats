# Projet Les petits plats

## Présentation

Réaliser le site de recettes de cuisine les petits plats pour la formation Openclassrooms de développeur d'application JS React. Les petits plats est le projet numéro 7 de la formation.

- Cliquer sur une HTML Card de recette imprime cette recette sur la console avec son id, ses ingrédients, ustentiles, électroménager et description complète.
- Une classe singleton RecipesAPI crée un tableau d'objets de recettes **Recipe** en découvrant tous les ingrédients, les ustensiles et l'électroménager présents dans les données.
- La classe recette Recipe a trois propriétés statiques allIngredients, allUstensils, allAppliances pour contenir tous les ingrédients, les ustensiles et l'électroménager découverts dans les 50 recettes du tableau JavaScript de données. Ces propriétés sont des stuctures Set.
- La classe recette **Recipe** stocke ses ingrédients de recette dans une structure Map dont la clé est le nom de l'ingrédient et la valeur est un objet de la classe **Ingredient**
- Deux fonctions étendent la classe **String** pour travailler avec les chaines de caractères:
  - capitalizeFirstLetter()
  - removeDiacritics() : Remplacer tous les signes qui s'ajoute aux lettres avant de faire des recherches.
- Deux expressions régulières sont utilisées par les deux types de recherche :
  - Début de mot pour la recherche globale ("écha" trouve "échalotte" mais pas "préchauffer" ni "béchamel" par exemple)
  - Mot complet pour la recherche d'étiquettes.
- L'algorithme choisi utilise [la méthode filter()](https://github.com/SFERRER-DEV/projet-7-petits-plats/blob/dev/scripts/util/search.js) sur des ensembles d'objets Recettes (branch: champ_de_rercherche_principal_1 -> dev -> main)
- Le fichier Dom.js contient des fonctions utilitaires nécessaires communes aux fabriques pour manipuler et créer les éléments du DOM.
- Une méthode de factory fabrique des HTML Cards pour les cartes des recettes.
- Les list-items des listes déroulantes ingredients, ustensiles et l'électroménager sont dynamiques.
- La librairie Bootstrap 4.6.2 est utilisée pour présenter l'affichage. Elle est fournie par BootstrapCDN.
- Le dossier **docs/** contient la fiche d'investigation, les algorigrammes, le détail des benchmarks.

## Liens

- Voir le site sur github pages : [Openclassrooms projet 7: Les petits plats](https://sferrer-dev.github.io/projet-7-petits-plats/)
- Code Climate: [Codebase summary projet 7 petits plats](https://codeclimate.com/github/SFERRER-DEV/projet-7-petits-plats)
- La recherche globale altenative se trouve sur la branche "algo_option_2": [Algorithme While & For](https://github.com/SFERRER-DEV/projet-7-petits-plats/blob/algo_option_2/scripts/util/search.js)
- La fiche d'investigation de la fonctionnalité de recherche générale de recettes :
  [**Fiche d'investigation.pdf**](https://github.com/SFERRER-DEV/projet-7-petits-plats/blob/main/docs/Fiche%20d'investigation.pdf)
- Les deux algorigrammes de la fiche d'investigation:
  [**Algorigrammes**](https://github.com/SFERRER-DEV/projet-7-petits-plats/blob/main/docs/algorigrammes.png)

- Exemples de benchmarks **Algo Filter** versus **Algo While & For**
  - [Benchmark en recherchant "coco"](https://jsben.ch/76g2e)
  - [Benchmark en recherchant "échalotte"](https://jsben.ch/wGcV5)
  - [Benchmark en recherchant "pim"](https://jsben.ch/dG0mj)
  - [Benchmark en recherchant "Faire cuire les pates"](https://jsben.ch/zQHha)
