# Encoder ℕ\* dans ℕ

## Questions

1. Une fonction de ℕ x ℕ → ℕ s'appelle
   1. Une fonction de couplage
   2. Une fonctiond de pairage
   3. Une fonction de projection
   4. N'a pas de nom particulier
2. Si A^k est dénombrable (pour k ∈ ℕ), alors A\* est
   1. Énumérable
   2. Dénombrable
   3. On ne peut rien dire
3. Un langage L défini sur un alphabet Σ (tel que L ⊆ Σ\*) est
   1. Énumérable
   2. Semi-décidable
   3. Récursivement énumérable
   4. Dénombrable
4. Une fonction d'encodage est une fonction
   1. Bijective
   2. De A vers ℕ (A dénombrable)
   3. D'un alphabet vers un autre alphabet
   4. Aucune de ces propositions
5. Si la fonction g réalise la fonction f selon c: A → ℕ, avec d = c^(-1) alors
   1. f(c(a)) = ⊥ ⇒ c(g(a)) = ⊥
   2. f(a) ≠ ⊥ ⇒ d(g(c(a))) = f(a)
   3. g(i) = b ⇒ f(d(i)) = d(b)
6. Un langage L défini sur un alphabet Σ (tel que L ⊆ Σ\*) est semi-décidable si
   1. Σ\* est dénombrable
   2. Σ\* est énumérable
   3. il existe f: L → ℕ avec f injective et calculable
   4. L est dénombrable et décidable

## Réponses

1. 4
2. 2
3. 4
4. 4
5. 2
6. 3

## Notes

### Question 2

> Pourquoi ne peut-on pas dire que A\* est énumérable quand A^k est dénombrable ?

### Question 3

> Pourquoi ne peut-on pas dire que L est énumérable ?
> Le langage L est enumérable ssi il est semi-décidable. Puisqu'on ne précise pas qu'il est semi décidable, on ne peut pas affirmer qu'il est énumérable.

D'ailleurs s'il avait été "énumérable", il aurait été aussi "semi-décidable" et "récursivement énumérable", qui est un synonyme de "semi-décidable".

### Question 4

> Pourquoi une fonction d'encodage n'est pas bijective ?

Un encodage doit être injectif mais pas forcément surjectif.
