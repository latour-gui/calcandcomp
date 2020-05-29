# langages de programmation et résultats fondamentaux

## Questions

1. La fonction sémantique d'un langage est une fonction
   1. Totale
   2. Partielle
2. La fonction sémantique d'un langage associe à un programme une fonction
   1. Totale
   2. Partielle
3. Un interpréteur d'un langage M par un langage L est une fonction
   1. Totale
   2. Partielle
   3. Ni l'un ni l'autre
4. Soit M et T deux langages de programmation et f une fonction tq ∥f(P)∥T = ∥P∥M pour tout P ∈ P_M. On appelle f
   1. Une fonction d'interprétation
   2. Un codage
   3. Une transformation de programme
   4. Une fonction de compilation
5. Si un langage admet une syntaxe concrète, ce langage permet l'écriture du programme universel
   1. Vrai
   2. Faux
6. Sous certaines conditions, un langage de programmation permet d'écrire HALT et SINT
   1. Vrai
   2. Faux
7. L'ensemble des programmes While qui ne terminent pas pour une entrée donnée est
   1. Semi-décidable
   2. Décidable
   3. Ni décidable ni semi-décidable
8. Soit l'ensemble des programmes While dont le nombre d'instructions est un produit de facteurs premiers. Cet ensemble est
   1. Décidable
   2. Semi-décidable
   3. Indécidable
   4. Impossible à déterminer
9. Soit l'ensemble des programmes While qui retournent "Hello World!". Cet ensemble est
   1. Décidable
   2. Semi-décidable
   3. Indécidable
   4. Impossible à déterminer
10. Un spécialisateur (en T) appliqué à un interpréteur (de S, écrit en T) pour un programme s (en S) crée
    1. Un interpréteur de S en T
    2. Un compilateur de S en T
    3. Un compilateur de T en S
    4. s compilé en T
11. Un spécialisateur (en T) appliqué à lui-même pour un interpréteur (de S, écrit en T) crée
    1. Un générateur d'interpréteurs
    2. Un générateur de compilateurs
    3. Un compilateur
    4. Un specialisateur

## Réponses

1. 1
2. 2
3. 3
4. 4
5. 2
6. 2
7. 3
8. 1
9. 2
10. 4
11. 3

## Notes

### Questions 1 - 2

> La fonction sémantique d'un langage est une fonction
>
> La fonction sémantique d'un langage associe à un programme une fonction

Attention à ne pas confondre la fonction sémantique **d'un langage** et la fonction sémentique **d'un programme de ce langage**

La fonction sémantique d'un langage est totale alors que celle d'un programme du langage est partielle.

### Question 3

> Un interpréteur d'un langage M par un langage L est une fonction

wtf it is not partielle ??

### Question 4

> Soit M et T deux langages de programmation et f une fonction tq ∥f(P)∥T = ∥P∥M pour tout P ∈ P_M. On appelle f

Pourquoi est-ce que une fonction d'interprétation c'est pas bon ?

### Question 7

> L'ensemble des programmes While qui ne terminent pas pour une entrée donnée

L'ensemble des programmes while qui _se terminent_ pour une entrée donnée est semi-décidable.
Par contre on ne sait rien déduire pour l'ensemble des programmes qui ne se terminent pas.

### Question 8

> Soit l'ensemble des programmes While dont le nombre d'instructions est un produit de facteurs premiers. Cet ensemble

La propriété du nombre d'instruction n'est pas une propriété existentielle (elle ne concerne pas juste les entrées et les sorties du programme) et la décomposition en facteur premiers est calculable.

### Question 9

> Soit l'ensemble des programmes While qui retournent "Hello World!". Cet ensemble est

Pour moi, le fait qu'un programme (while) retourne "Hello World!" est une propriété non-triviale (il y a des programmes qui retournent "Hello World!" et d'autres qui ne retournent pas "Hello World!") et existentielle (elle ne dépend que de la relation établie par le programme entre ses entrées et sorties.).

Dès lors le théorème 3.22 nous dit

> Soit L un langage de programmation et A une propriété non-triviale et existentielle des programmes en L. Alors A est indécidable.
