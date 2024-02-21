[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

## Definition of little $o$ 
$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

## Definition of Big $O$
$f(n)\in O(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) \le c g(n)$

## Proof 
- If we start with $f(n)\in o(g(n))$ by the deffiniton provided we know that for any positive constant $c$ there exists a point called $n_0$
  beyond which is always $\ f(n) < c \cdot g(n)$
- If we were to choose another constant $k$ that is greater then 0 but less then our origninal constant $c$.
- We can then use the new smaller constant for the definition of big $O$ to show that $f(n)\in O(g(n))$
- Since we know that $\ \forall n\ge n_0: f(n) < c g(n)$
- We can see that $\ f(n) \le k g(n)$ using the new smaller constant $k$.
- since we used a constant $k$ that is smaller then $c$ we have shown that the definition of Big $O$ is satisfied.

I got help from the TA during lab hours. 
I looked at a few of the other students repositories to get an idea of how to do this assignment.
- little-o-proof-Assel-Aljazwe
- little-o-proof-ZachRenz
