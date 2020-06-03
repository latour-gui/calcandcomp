# Definitions

- [Definitions](#definitions)
  - [Modèle de calcul universel](#modèle-de-calcul-universel)
  - [Fonction sémantique d'un langage](#fonction-sémantique-dun-langage)
  - [Syntaxe concrête](#syntaxe-concrête)
  - [Point fixe](#point-fixe)
  - [NP](#np)
  - [NP-hard != NP-complet](#np-hard--np-complet)

## Modèle de calcul universel

Un modèle de calcul est considéré comme universel s'il est possible d'y calculer toutes les ofnctions calculables.

On suppose q'un tel modèle de calcul existe grâce à la thèse de Church-Turing qui suppose que tout modèle de calcul raisonable définit le même ensemble de fonctions calculables.

## Fonction sémantique d'un langage

La fonction sémantique d'un langage L = (P_L, D_L) est une fonction totale [[ . ]] : P_L -> (D_L -> D_L)

On peut donc dire que la fonction sémantique d'un langage L est une fonction qui associe à chaque programme de L une fonction (partielle) définie sur D_L -> D_L

## Syntaxe concrête

On dit qu'un language L = (P_L, D_L) a une syntaxe concrète si P_L est inclu dans D_L

## Point fixe

> les points fixes d'une fonction c'est les éléments pour lesquels
>
> f(x) = x

Directement on voit que, pour des fonctions mathématiques, ce sera tous les points qui se situent sur la droite, `x = y`

Dans le cadre du chap 3, on nous dit que, étant donné une fonction totale `f : P_L -> P_L`

> i.e. une fonction qui prend un programme et qui retourne un programme

il y aura toujours un programme `P \in P_L tq f(P) = P`,
un point fixe.

Dès lors on sait qu'il n'existe aucune fonction `P_L -> P_L` qui transforme tous les programmes qu'on lui donne.

Donc on sait que `pour tout P \in Ps`, 'il existe un programme, mettons `F`, tq:
`[[P]]t = [[F]](P,t)`

Avec `F` qui est donc le programme qui manifeste la fonction de transformation `f` précitée.

En gros, pour tout langage, il existe un programme `F` dont la sémantique `[[F]]` est un point fixe.

i.e.

1. pour toute fonction de transformation de programme il existe un programme pour lequel cette fonction ne fait rien
2. pour tout programme il existe une fonction de transformation telle que cette fonction ne fait rien sur ce programme

## NP

"Non-déterministe polynomial" et pas "non polynomial"

## NP-hard != NP-complet

si je résume intuitivement, j'aurais tendance à dire que

NP-complet est consititué de quelques problèmes de NP tq tous les problèmes de NP peuvent être réduit polynomialement à l'un de ces langage.

NP-hard est tel que chaque problème de NP peut être réduit polynomialement à un problème NP-hard.

NP-hard != NP-complet car NP-complet ⊆ NP et NP ⊆ NP-hard.

On sait que NP != NP-hard car il existe des problèmes
