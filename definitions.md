# Definitions

- [Definitions](#definitions)
  - [Modèle de calcul universel](#modèle-de-calcul-universel)
  - [Fonction sémantique d'un langage](#fonction-sémantique-dun-langage)
  - [Syntaxe concrête](#syntaxe-concrête)
  - [Point fixe](#point-fixe)

## Modèle de calcul universel

vtff

## Fonction sémantique d'un langage

waitwat

## Syntaxe concrête

ntm

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
