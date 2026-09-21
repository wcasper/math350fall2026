---
layout: post
title: "Lecture 8"
date: 2026-09-21
---

## Compactness

### Key words

point-set topology, open cover, subcover, finite subcover, countable subcover, Lindelöf covering theorem, compact set, bounded set, compact implies bounded, compact implies closed

### Reading assignment

Apostol, Chapter 3: the sections on open covers, the Lindelöf covering theorem, compactness, and the basic properties of compact subsets of Euclidean space.

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec08/lec08.pdf)

## Practice problems

Recall that an **open cover** of a set $$A\subseteq\mathbb{R}^n$$ is a family of open sets $$\{U_i:i\in I\}$$ such that

$$
A\subseteq\bigcup_{i\in I}U_i.
$$

A set is **compact** if every open cover of the set has a finite subcover.

1. **Understanding covers and subcovers.** For each $$n\in\mathbb{N}$$, define

   $$
   U_n=\left(-\frac1n,1+\frac1n\right).
   $$

   1. Prove that $$\{U_n:n\in\mathbb{N}\}$$ is an open cover of $$[0,1]$$.
   2. Find a subcover consisting of a single set.
   3. Is

      $$
      \{U_n:n\ge 2\}
      $$

      still a cover of $$[0,1]$$?
   4. Is

      $$
      \{U_{2n}:n\in\mathbb{N}\}
      $$

      a subcover?
   5. Explain why the existence of one finite open cover of a set does not by itself prove that the set is compact.

2. **Finite sets are compact.** Let

   $$
   F=\{\mathbf{x}_1,\ldots,\mathbf{x}_m\}
   \subseteq\mathbb{R}^n.
   $$

   1. Let $$\{U_i:i\in I\}$$ be an arbitrary open cover of $$F$$. For each $$k$$, choose an index $$i_k\in I$$ such that

      $$
      \mathbf{x}_k\in U_{i_k}.
      $$

   2. Prove that

      $$
      \{U_{i_1},\ldots,U_{i_m}\}
      $$

      is a finite subcover of $$F$$.
   3. Conclude that every finite subset of $$\mathbb{R}^n$$ is compact.
   4. Explain why the empty set is also compact.

3. **A bounded set that is not compact.** For each $$n\ge2$$, define

   $$
   U_n=\left(\frac1n,1\right).
   $$

   1. Prove that $$\{U_n:n\ge2\}$$ is an open cover of $$(0,1)$$.
   2. Let

      $$
      U_{n_1},\ldots,U_{n_k}
      $$

      be finitely many members of the cover, and let

      $$
      N=\max\{n_1,\ldots,n_k\}.
      $$

      Prove that their union is contained in $$U_N$$.
   3. Find a point of $$(0,1)$$ that is not contained in $$U_N$$.
   4. Conclude that this cover has no finite subcover.
   5. Deduce directly from the definition that $$(0,1)$$ is not compact.

4. **An unbounded set is not compact.** For each $$n\in\mathbb{N}$$, define

   $$
   V_n=B(\mathbf{0};n).
   $$

   Let $$A\subseteq\mathbb{R}^n$$ be unbounded.

   1. Prove that $$\{V_n:n\in\mathbb{N}\}$$ is an open cover of $$A$$.
   2. Prove that the union of any finite collection

      $$
      V_{n_1},\ldots,V_{n_k}
      $$

      is equal to one of the balls in that collection.
   3. Use the fact that $$A$$ is unbounded to show that no finite collection of the sets $$V_n$$ covers $$A$$.
   4. Conclude that every compact subset of $$\mathbb{R}^n$$ is bounded.

5. **Equivalent descriptions of boundedness.** Let $$A\subseteq\mathbb{R}^n$$. Prove that the following statements are equivalent:

   1. There exist $$\mathbf{a}\in\mathbb{R}^n$$ and $$r>0$$ such that

      $$
      A\subseteq B(\mathbf{a};r).
      $$

   2. There exists $$R>0$$ such that

      $$
      A\subseteq B(\mathbf{0};R).
      $$

   3. There exists $$M>0$$ such that

      $$
      \lVert\mathbf{x}\rVert\le M
      $$

      for every $$\mathbf{x}\in A$$.

   Your proof should use the triangle inequality to compare balls having different centers.

6. **Compact sets are closed.** Let $$K\subseteq\mathbb{R}^n$$ be compact, and fix

   $$
   \mathbf{x}\in\mathbb{R}^n-K.
   $$

   For each $$m\in\mathbb{N}$$, define

   $$
   U_m
   =
   \mathbb{R}^n-
   \left\{
   \mathbf{y}\in\mathbb{R}^n:
   \lVert\mathbf{y}-\mathbf{x}\rVert\le\frac1m
   \right\}.
   $$

   1. Prove that every $$U_m$$ is open.
   2. Prove that

      $$
      \bigcup_{m\in\mathbb{N}}U_m
      =
      \mathbb{R}^n-\{\mathbf{x}\}.
      $$

   3. Explain why $$\{U_m:m\in\mathbb{N}\}$$ is an open cover of $$K$$.
   4. Use compactness to choose a finite subcover, and show that there is some $$M\in\mathbb{N}$$ such that

      $$
      K\subseteq U_M.
      $$

   5. Deduce that

      $$
      B\left(\mathbf{x};\frac1M\right)\cap K=\varnothing.
      $$

   6. Conclude that $$\mathbb{R}^n-K$$ is open and hence that $$K$$ is closed.

7. **Closed subsets of compact sets.** Suppose that $$K\subseteq\mathbb{R}^n$$ is compact and $$F\subseteq K$$ is closed.

   1. Let $$\{U_i:i\in I\}$$ be an open cover of $$F$$.
   2. Prove that

      $$
      \{U_i:i\in I\}\cup\{\mathbb{R}^n-F\}
      $$

      is an open cover of $$K$$.
   3. Use compactness of $$K$$ to obtain a finite subcover of $$K$$.
   4. Remove $$\mathbb{R}^n-F$$ from this finite collection and prove that the remaining sets still cover $$F$$.
   5. Conclude that every closed subset of a compact set is compact.

8. **Finite unions of compact sets.** Let $$K_1,\ldots,K_m$$ be compact subsets of $$\mathbb{R}^n$$.

   1. Suppose that $$\{U_i:i\in I\}$$ is an open cover of

      $$
      K_1\cup\cdots\cup K_m.
      $$

   2. For each $$j$$, explain why the same family is an open cover of $$K_j$$.
   3. Choose a finite subcover of each $$K_j$$.
   4. Combine these finite collections to obtain a finite subcover of

      $$
      K_1\cup\cdots\cup K_m.
      $$

   5. Conclude that every finite union of compact sets is compact.
   6. Give an example showing that an infinite union of compact sets need not be compact.

9. **A proof of the Lindelöf covering theorem.** Let $$A\subseteq\mathbb{R}^n$$, and suppose that $$\{U_i:i\in I\}$$ is an open cover of $$A$$.

   Let $$\mathcal{B}$$ be the family of all open balls

   $$
   B(\mathbf{q};r)
   $$

   whose center $$\mathbf{q}$$ has rational coordinates and whose radius $$r$$ is a positive rational number.

   1. Prove that $$\mathcal{B}$$ is countable.
   2. Given $$\mathbf{x}\in A$$, choose $$i\in I$$ such that $$\mathbf{x}\in U_i$$. Prove that there is some ball $$B\in\mathcal{B}$$ such that

      $$
      \mathbf{x}\in B\subseteq U_i.
      $$

   3. Let $$\mathcal{B}_0$$ consist of the balls in $$\mathcal{B}$$ that are contained in at least one of the sets $$U_i$$. Prove that $$\mathcal{B}_0$$ covers $$A$$.
   4. For each $$B\in\mathcal{B}_0$$, choose one index $$i(B)$$ such that

      $$
      B\subseteq U_{i(B)}.
      $$

   5. Prove that

      $$
      \{U_{i(B)}:B\in\mathcal{B}_0\}
      $$

      is a countable subcover of $$A$$.

10. **The finite-intersection property.** Let $$K\subseteq\mathbb{R}^n$$ be compact, and let $$\{F_i:i\in I\}$$ be a family of closed subsets of $$K$$. Suppose that every finite subfamily has nonempty intersection; that is,

    $$
    F_{i_1}\cap\cdots\cap F_{i_m}\ne\varnothing
    $$

    for every finite collection $$i_1,\ldots,i_m\in I$$.

    1. Suppose, for contradiction, that

       $$
       \bigcap_{i\in I}F_i=\varnothing.
       $$

    2. Use De Morgan’s law to prove that

       $$
       \left\{
       \mathbb{R}^n-F_i:i\in I
       \right\}
       $$

       is an open cover of $$K$$.

    3. Use compactness to obtain a finite subcover.
    4. Apply De Morgan’s law again to show that the corresponding finite collection of the sets $$F_i$$ has empty intersection.
    5. Explain why this is a contradiction.
    6. Conclude that

       $$
       \bigcap_{i\in I}F_i\ne\varnothing.
       $$


