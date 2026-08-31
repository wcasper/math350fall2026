---
layout: post
title: "Lecture 4"
---

## Functions and cardinality

### Key words

function, domain, codomain, image, injection, surjection, bijection, converse relation, inverse function, composition, cardinality, Cantor-Schröder-Bernstein theorem, finite set, countably infinite set, countable set, uncountable set, diagonalization, power set, countable union

### Reading assignment

Apostol, Chapter 2: the sections on functions, one-to-one functions and inverses, composite functions, finite and infinite sets, countability, uncountability, and cardinal numbers.

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec04/lec04.pdf)

## Practice problems

You may use the results established in lecture, including the Cantor-Schröder-Bernstein theorem, Cantor's theorem, and the theorem that a countable union of countable sets is countable. When proving that two sets have the same cardinality, clearly identify the functions you use and verify the required properties.

1. **Changing the domain and codomain.** Consider the rule

   $$
   f(x)=x^2.
   $$

   Determine whether $$f$$ is injective, surjective, or bijective in each of the following cases:

   1. $$f:\mathbb{R}\to\mathbb{R}$$;
   2. $$f:\mathbb{R}\to[0,\infty)$$;
   3. $$f:[0,\infty)\to\mathbb{R}$$;
   4. $$f:[0,\infty)\to[0,\infty)$$;
   5. $$f:(-\infty,0]\to[0,\infty)$$.

   For every case in which $$f$$ is bijective, find its inverse. Explain why injectivity and surjectivity depend on the specified domain and codomain, not merely on the formula.

2. **Composition and injectivity.** Let

   $$
   f:A\to B
   \qquad\text{and}\qquad
   g:B\to C.
   $$

   1. Prove that if $$f$$ and $$g$$ are injective, then $$g\circ f$$ is injective.
   2. Prove that if $$g\circ f$$ is injective, then $$f$$ must be injective.
   3. Must $$g$$ be injective if $$g\circ f$$ is injective? Give a counterexample.
   4. Prove that if $$g\circ f$$ is injective and $$f$$ is surjective, then $$g$$ is injective.

3. **Composition and surjectivity.** Again let

   $$
   f:A\to B
   \qquad\text{and}\qquad
   g:B\to C.
   $$

   1. Prove that if $$f$$ and $$g$$ are surjective, then $$g\circ f$$ is surjective.
   2. Prove that if $$g\circ f$$ is surjective, then $$g$$ must be surjective.
   3. Must $$f$$ be surjective if $$g\circ f$$ is surjective? Give a counterexample.
   4. Prove that if $$g\circ f$$ is surjective and $$g$$ is injective, then $$f$$ is surjective.

4. **When does an inverse exist?** Let $$f:A\to B$$ be a function, and let its converse relation be

   $$
   \check f=\{(b,a)\in B\times A:f(a)=b\}.
   $$

   Prove that $$\check f$$ is a function from $$B$$ to $$A$$ if and only if $$f$$ is bijective.

   When these conditions hold, write $$f^{-1}=\check f$$ and prove that

   $$
   f^{-1}\circ f=\operatorname{id}_A
   \qquad\text{and}\qquad
   f\circ f^{-1}=\operatorname{id}_B.
   $$

5. **The rational numbers are countable.** Let

   $$
   \mathbb{Z}\times\mathbb{N}
   $$

   represent the possible numerators and positive denominators of rational numbers.

   1. Prove that $$\mathbb{Z}\times\mathbb{N}$$ is countable.
   2. Define

      $$
      F:\mathbb{Z}\times\mathbb{N}\to\mathbb{Q},
      \qquad
      F(p,q)=\frac pq.
      $$

      Prove that $$F$$ is surjective.
   3. Deduce that $$\mathbb{Q}$$ is countable.
   4. Explain why the fact that different pairs can represent the same rational number causes no problem.
   5. Prove that the set of irrational real numbers is uncountable.

6. **Finite strings form a countable set.** Let $$\Sigma=\{0,1,\ldots,9\}$$, and let $$W_n$$ be the set of all strings of exactly $$n$$ symbols from $$\Sigma$$.

   1. Prove that $$W_n$$ is finite for every $$n\in\mathbb{N}$$.
   2. Let

      $$
      W=\bigcup_{n\in\mathbb{N}}W_n.
      $$

      Prove that $$W$$ is countable.
   3. Is $$W$$ finite or countably infinite? Justify your answer.
   4. Deduce that the set of all finite English texts is countable, assuming that only finitely many symbols may be used.

7. **Finite subsets of the natural numbers.** Let

   $$
   \mathcal{F}
   =
   \{S\subseteq\mathbb{N}:S\text{ is finite}\}.
   $$

   For each $$k\in\mathbb{N}$$, define

   $$
   \mathcal{F}_k
   =
   \{S\subseteq\mathbb{N}:\lvert S\rvert=k\}.
   $$

   1. Construct a surjection from $$\mathbb{N}^k$$ onto $$\mathcal{F}_k$$, or otherwise prove that $$\mathcal{F}_k$$ is countable.
   2. Prove that $$\mathcal{F}$$ is countable.
   3. Prove that the full power set $$\mathcal{P}(\mathbb{N})$$ is uncountable.
   4. Conclude that most subsets of $$\mathbb{N}$$ are infinite, in the precise sense that the family of finite subsets is countable while the family of all subsets is uncountable.

8. **Infinite binary sequences.** Let

   $$
   X=\{(a_1,a_2,a_3,\ldots):a_n\in\{0,1\}\text{ for every }n\in\mathbb{N}\}.
   $$

   1. Suppose that

      $$
      x^{(1)},x^{(2)},x^{(3)},\ldots
      $$

      were an enumeration of $$X$$, where

      $$
      x^{(j)}=(a_{j1},a_{j2},a_{j3},\ldots).
      $$

      Define a sequence $$b=(b_1,b_2,\ldots)$$ by

      $$
      b_j=1-a_{jj}.
      $$

      Prove that $$b$$ is not equal to any sequence in the enumeration.
   2. Deduce that $$X$$ is uncountable.
   3. Construct a bijection between $$X$$ and $$\mathcal{P}(\mathbb{N})$$.
   4. Explain why this version of diagonalization avoids the ambiguity of decimal expansions ending in repeating nines.

9. **Understanding Cantor's power-set argument.** Let $$A$$ be any set, and suppose that

   $$
   f:A\to\mathcal{P}(A).
   $$

   Define

   $$
   D=\{a\in A:a\notin f(a)\}.
   $$

   1. Prove that $$D\subseteq A$$, so $$D\in\mathcal{P}(A)$$.
   2. Suppose that $$D=f(x)$$ for some $$x\in A$$. Analyze separately the possibilities $$x\in D$$ and $$x\notin D$$ and derive a contradiction in each case.
   3. Deduce that no function from $$A$$ to $$\mathcal{P}(A)$$ can be surjective.
   4. Construct an injective function from $$A$$ to $$\mathcal{P}(A)$$.
   5. Conclude that

      $$
      \lvert A\rvert<\lvert\mathcal{P}(A)\rvert.
      $$

10. **Comparing familiar uncountable sets.** Use explicit injections and the Cantor-Schröder-Bernstein theorem to prove the following statements.

    1. $$[0,1]$$ and $$(0,1)$$ have the same cardinality.

       *Hint:* One injection is immediate. For the other, send $$0,1,\frac12,\frac13,\ldots$$ to distinct points of $$(0,1)$$ and leave all other points fixed.

    2. $$(0,1)$$ and $$\mathbb{R}$$ have the same cardinality.

       *Hint:* For an injection from $$\mathbb{R}$$ into $$(0,1)$$, consider a function involving

       $$
       \frac{x}{1+\lvert x\rvert}.
       $$

    3. Every nonempty open interval $$(a,b)$$ has the same cardinality as $$\mathbb{R}$$.
    4. The set of irrational numbers in $$(0,1)$$ has the same cardinality as $$(0,1)$$.

       *Hint:* Use the countability of $$\mathbb{Q}\cap(0,1)$$ and construct an injection that moves the rational numbers into a reserved countable collection of irrational numbers.


