Motivation
==========

J'ai essentiellement programmé ce OCaml Pong pour me familiariser avec OCaml et avec certains concepts de la programmation fonctionnelle.

Récursion terminale (*tail recursion*)
-------------------

`main` utilise la récursion terminale pour ne pas faire déborder la pile.


Fermeture (*closures*)
---------------

`balle` est un un enregistrement de type `tballe` qui stocke ses propriétés privées dans une fermeture.

Fonctions comme valeurs de première classe (*first-class functions*)
-------------------------------
`balle` possède une fonction membre `applique_vitesse` qui prend en paramètre une fonction [À COMPLÉTER].

Types et filtres
----------------

L'état du jeu est représenté à l'aide d'un type pouvant être de forme `Splash | EnJeu | Pause | Quitter`. À l'aide de filtres, les fonctions `entree`, `velocite` et `rendu` agissent différemment dépendamment de l'état du jeu.

À faire
==========

1. Encapsuler le tout dans un module.
2. Meilleures abstractions autour des joueurs.