---
layout: post
title: "Lecture 3"
---

## Completeness and set theory

### Key words

decimal approximation, supremum, infimum, approximation property, additive property of suprema, Archimedean property, set, empty set, subset, union, intersection, relative complement, De Morgan's laws, indexed family, Cartesian product, relation, domain, codomain, function, image

### Reading assignment

Apostol, Chapter 1: review the completeness axiom, properties of suprema, and the Archimedean property. Then read Chapter 2 through the sections on Cartesian products, relations, and functions.

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec03/lec03.pdf)

## Practice problems

You may use results established in lecture, but justify every set equality by reasoning about membership and every claim about a supremum or infimum directly from the appropriate definitions or theorems.

1. **Using the approximation property.** Define

   $$
   S=\left\{\frac{2n-1}{n+1}:n\in\mathbb{N}\right\}.
   $$

   1. Rewrite each element of $$S$$ in the form $$2-\dfrac{c}{n+1}$$ for an appropriate constant $$c$$.
   2. Prove that $$2$$ is an upper bound of $$S$$.
   3. Given $$\varepsilon>0$$, use the Archimedean property to find $$n\in\mathbb{N}$$ such that

      $$
      2-\varepsilon<\frac{2n-1}{n+1}.
      $$

   4. Deduce that $$\sup(S)=2$$.
   5. Determine whether $$S$$ has a maximum, and find $$\inf(S)$$ and $$\min(S)$$.

2. **Another nonunique decimal expansion.** For each $$k\in\mathbb{N}$$, let

   $$
   s_k
   =
   2+\frac{3}{10}
   +\frac{4}{10^2}
   +\frac{9}{10^3}
   +\cdots+
   \frac{9}{10^k},
   $$

   where all digits after the second decimal place are $$9$$. Thus the decimal $$2.34999\ldots$$ is defined to be

   $$
   \sup\{s_k:k\in\mathbb{N},\ k\ge 3\}.
   $$

   1. Prove that

      $$
      s_k=2.35-10^{-k}.
      $$

   2. Prove, using the Archimedean property rather than infinite-series or limit notation, that

      $$
      2.34999\ldots=2.35.
      $$

   3. Generalize the argument: if a finite decimal terminates in a nonzero digit, describe a second decimal expansion representing the same real number.

3. **Integer intervals.** Use the Archimedean property and the well-ordering property of $$\mathbb{N}$$ to prove that for every $$x\in\mathbb{R}$$ there exists an integer $$m$$ such that

   $$
   m\le x<m+1.
   $$

   Then prove that this integer is unique.

   *Hint:* First use the Archimedean property to choose $$N\in\mathbb{N}$$ with $$N>x$$ and $$N>-x$$. Consider the set

   $$
   \{n\in\mathbb{N}:n>x+N\}.
   $$

4. **Set identities by element chasing.** Let $$A,B,C$$ be subsets of a universal set $$X$$. Prove each identity by showing that an arbitrary element belongs to the left-hand side if and only if it belongs to the right-hand side.

   1. Distributivity of intersection over union:

      $$
      A\cap(B\cup C)=(A\cap B)\cup(A\cap C).
      $$

   2. Distributivity of union over intersection:

      $$
      A\cup(B\cap C)=(A\cup B)\cap(A\cup C).
      $$

   3. A relative-complement identity:

      $$
      A-(B\cup C)=(A-B)\cap(A-C).
      $$

   4. Another relative-complement identity:

      $$
      A-(B\cap C)=(A-B)\cup(A-C).
      $$

5. **Indexed unions and intersections.** For each positive real number $$t$$, define

   $$
   A_t=(-t,t),
   \qquad
   B_t=(-\infty,t].
   $$

   Determine each of the following sets and prove your answers:

   $$
   \bigcup_{t>0}A_t,
   \qquad
   \bigcap_{t>0}A_t,
   \qquad
   \bigcup_{t>0}B_t,
   \qquad
   \bigcap_{t>0}B_t.
   $$

   Your argument for the first union and the first intersection should explicitly use the Archimedean property.

6. **A family indexed by the natural numbers.** For each $$n\in\mathbb{N}$$, let

   $$
   C_n=\left[-\frac1n,\,1+\frac1n\right].
   $$

   1. Prove that $$C_{n+1}\subseteq C_n$$ for every $$n\in\mathbb{N}$$.
   2. Determine

      $$
      \bigcup_{n\in\mathbb{N}}C_n
      \qquad\text{and}\qquad
      \bigcap_{n\in\mathbb{N}}C_n.
      $$

   3. To prove your answer for the intersection, explain how the Archimedean property rules out every $$x<0$$ and every $$x>1$$.

7. **Cartesian products and set operations.** Let $$A,B,C$$ be sets.

   1. Prove that

      $$
      A\times(B\cup C)=(A\times B)\cup(A\times C).
      $$

   2. Prove that

      $$
      A\times(B\cap C)=(A\times B)\cap(A\times C).
      $$

   3. Is it always true that

      $$
      (A\cup B)\times(C\cup D)
      =
      (A\times C)\cup(B\times D)?
      $$

      If not, give a counterexample and then write a correct formula for the left-hand side as a union of Cartesian products.

   4. Prove that if $$A\ne\varnothing$$ and $$A\times B=A\times C$$, then $$B=C$$. Explain why the hypothesis $$A\ne\varnothing$$ is necessary.

8. **Relations, domains, and codomains.** Let

   $$
   A=\{-2,-1,0,1,2\},
   \qquad
   B=\{0,1,2,3,4\},
   $$

   and define a relation $$R\subseteq A\times B$$ by

   $$
   aRb
   \quad\Longleftrightarrow\quad
   b=a^2.
   $$

   1. List all ordered pairs in $$R$$.
   2. Find $$\operatorname{dom}(R)$$ and $$\operatorname{codom}(R)$$ using the definitions from lecture.
   3. Is $$R$$ a function from $$A$$ to $$B$$?
   4. Define the inverse relation

      $$
      R^{-1}=\{(b,a)\in B\times A:(a,b)\in R\}.
      $$

      Is $$R^{-1}$$ a function from $$B$$ to $$A$$? Explain precisely which part of the definition succeeds or fails.

9. **When is a relation a function?** For each relation below, determine whether it is a function from $$\mathbb{R}$$ to $$\mathbb{R}$$. If it is not, state exactly why not.

   1. 
      $$
      R_1=\{(x,y)\in\mathbb{R}^2:y^2=x\}.
      $$

   2. 
      $$
      R_2=\{(x,y)\in\mathbb{R}^2:y=x^2\}.
      $$

   3. 
      $$
      R_3=\{(x,y)\in\mathbb{R}^2:xy=1\}.
      $$

   4. 
      $$
      R_4=\{(x,y)\in\mathbb{R}^2:y=\lvert x\rvert\}.
      $$

   For each relation, also determine its domain and codomain as defined in lecture. Notice that the codomain of a relation, in the terminology used in the slides, consists only of values that actually occur.

10. **Images and inverse images.** Let $$f:A\to B$$ be a function. For $$S\subseteq A$$ and $$T\subseteq B$$, define

    $$
    f(S)=\{f(x):x\in S\}
    $$

    and

    $$
    f^{-1}(T)=\{x\in A:f(x)\in T\}.
    $$

    1. Prove that for all $$S_1,S_2\subseteq A$$,

       $$
       f(S_1\cup S_2)=f(S_1)\cup f(S_2).
       $$

    2. Prove that

       $$
       f(S_1\cap S_2)\subseteq f(S_1)\cap f(S_2).
       $$

    3. Give an example in which the inclusion in the previous part is strict.
    4. Prove that for all $$T_1,T_2\subseteq B$$,

       $$
       f^{-1}(T_1\cup T_2)
       =
       f^{-1}(T_1)\cup f^{-1}(T_2)
       $$

       and

       $$
       f^{-1}(T_1\cap T_2)
       =
       f^{-1}(T_1)\cap f^{-1}(T_2).
       $$

    5. What additional property of $$f$$ guarantees that

       $$
       f(S_1\cap S_2)=f(S_1)\cap f(S_2)
       $$

       for every pair of subsets $$S_1,S_2\subseteq A$$?

