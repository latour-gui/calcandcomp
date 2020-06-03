# Lamda Calcul

## Questions

1. (xy).λy.x est une expression Lambda correcte
   1. Vrai
   2. Faux
2. λx.xyy est une application
   1. Vrai
   2. Faux
3. λx.xyλt.tx
   1. est une application
   2. est une abstraction
   3. n'est pas une expression lambda correcte
4. λxyzt.z(xt)ab(zsy) contient
   1. 1 variable libre
   2. 2 variables libres
   3. 3 variables libres
   4. 4 variables libres
5. Il est possible d'écrire un compilateur de Lambda Calcul vers While
   1. Vrai
   2. Faux
6. Il faut d'abord appliquer la β-réduction du redex
   1. Le plus à gauche
   2. Le plus intérieur (innermost)
   3. Le plus extérieur (outermost)
   4. Peu importe
7. La définition correcte du Successeur d'un entier de Church est
   1. λxy.y(yx)
   2. λw.λyx.y(wyx)
   3. λw.λx.xwx
   4. λwxy.y(wyx)
8. λsz.s(λwab.a(wab))z
   1. Multiplie s par z
   2. Calcule x exposant z
   3. Renvoie True si z vaut zéro
   4. Additionne s à z
9. Si Z est "is_zero", S "successeur" et P "prédecesseur" alors Toto ≡ λn.Zn 0 (n S (Toto(P n))) calcule
   1. La factorielle
   2. La somme des n premiers entiers
   3. Rien du tout

## Réponses

1. 2
2. 2
3. 2
4. 3
5. 1
6. 4
7. 2
8. 4
9. 3

## Notes

### Question 5

> Comment est-ce possible de produire à l'aide du lamda calcul, un compilateur While alors que le lambda calcul ne possède pas dans son langage les éléments du langage du While ?

Il faut partir du principe que, bien que le lambda calcul ne va pas "output" un programme while, il sera possible d'en simuler le comportement.

Il est par exemple possible de définir, en lambda calcul, chacun des caractères du langage while d'une manière similaire à la définition des naturels.

Dès lors on pourra considérer que ces nouvelles définitions nous permettent de produire un compilateur while en lambda calcul.

### Question 9

Nous sommes en présence de ce qu'on appelle dans le domaine un "coup de pute".

En effet en lambda calcul il n'est pas possilbe de donner un nom à une fonction, donc cette expression n'est pas valide en lambda calcul donc elle ne calcule rien du tout.

Pour effectuer la récursion, il faut utiliser l'opérateur point fixe : `Y ≡ λy. (λx. y (x x)) (λx. y (x x))`, définir Toto comme ceci : `Toto ≡ λrn.Zn 0 (n S (r(P n)))`.

À partir de là il est possible de calculer la somme des n premiers entiers : `Y Toto`.
