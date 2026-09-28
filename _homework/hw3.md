---
layout: post
title: "Homework: Open Covers and Compactness"
date: 2026-09-28
---

## Instructions

Write complete explanations and proofs in full sentences. Clearly state every theorem that you use. When a problem asks for a proof directly from a definition, do not replace that argument with a stronger theorem.

This assignment is based on:

- [Lecture 8 slides](https://wcasper.github.io/math350fall2026/slides/lec08/lec08.pdf)
- [Lecture 10 slides](https://wcasper.github.io/math350fall2026/slides/lec10/lec10.pdf)

## Problems

1. **Three lessons about open covers.**

   1. Let

      $$
      A=\{0,1,2\}
      $$

      and

      $$
      \mathcal{U}
      =
      \left\{
      \left(-\frac14,\frac14\right),
      \left(\frac34,\frac54\right),
      \left(\frac74,\frac94\right)
      \right\}.
      $$

      Prove that $$\mathcal{U}$$ is an open cover of $$A$$. Explain why removing any member of $$\mathcal{U}$$ produces a collection that no longer covers $$A$$. Thus $$\mathcal{U}$$ has no proper subcover. Why would it be incorrect to say that $$\mathcal{U}$$ has no subcovers at all?

   2. For each $$n\in\mathbb{N}$$, let

      $$
      U_n=(-n,n).
      $$

      Prove that $$\{U_n:n\in\mathbb{N}\}$$ is an open cover of $$\mathbb{R}$$. If

      $$
      U_{n_1},\ldots,U_{n_k}
      $$

      is any finite collection of these sets, let

      $$
      N=\max\{n_1,\ldots,n_k\}.
      $$

      Prove that their union is $$(-N,N)$$, and exhibit a real number that is not in this union. Conclude that this open cover has no finite subcover.

   3. Now consider

      $$
      V_1=(-\infty,1)
      \qquad\text{and}\qquad
      V_2=(0,\infty).
      $$

      Prove that $$\{V_1,V_2\}$$ is a finite open cover of $$\mathbb{R}$$. Explain why the existence of this finite open cover does not imply that $$\mathbb{R}$$ is compact. Which word in the definition of compactness makes the difference?

   4. Explain why every subset of $$\mathbb{R}^m$$ has at least one finite open cover. Why, then, is compactness not defined by the existence of a finite open cover?

2. **Building new compact sets.** Work directly from the definition of compactness unless a part explicitly permits a theorem.

   1. Prove that every singleton set $$\{x\}\subseteq\mathbb{R}^m$$ is compact.
   2. Deduce that every finite subset of $$\mathbb{R}^m$$ is compact.
   3. Prove that if $$K_1$$ and $$K_2$$ are compact, then $$K_1\cup K_2$$ is compact.
   4. Use induction to prove that a finite union of compact sets is compact.
   5. Let $$K\subseteq\mathbb{R}^m$$ be compact, and let $$F\subseteq K$$ be closed as a subset of $$\mathbb{R}^m$$. If $$\mathcal{U}$$ is an open cover of $$F$$, explain why

      $$
      \mathcal{U}\cup\{\mathbb{R}^m-F\}
      $$

      is an open cover of $$K$$. Use this observation to prove that $$F$$ is compact.

   6. Prove that the intersection of two compact subsets of $$\mathbb{R}^m$$ is compact. You may use the theorem that compact subsets of $$\mathbb{R}^m$$ are closed.

3. **A missing endpoint makes a difference.**

   1. For each integer $$n\ge2$$, define

      $$
      U_n=\left(\frac1n,1\right).
      $$

      Prove that $$\{U_n:n\ge2\}$$ is an open cover of $$(0,1)$$ with no finite subcover. Conclude directly from the definition that $$(0,1)$$ is not compact.

   2. Now let

      $$
      K=
      \{0\}\cup
      \left\{\frac1n:n\in\mathbb{N}\right\}.
      $$

      Let $$\mathcal{U}$$ be an arbitrary open cover of $$K$$, and choose $$U\in\mathcal{U}$$ containing $$0$$. Explain why there is an $$r>0$$ such that

      $$
      (-r,r)\subseteq U.
      $$

   3. Use the Archimedean property to choose $$N\in\mathbb{N}$$ such that

      $$
      \frac1n<r
      $$

      whenever $$n\ge N$$. Explain why $$U$$ covers all but finitely many points of $$K$$.

   4. Cover the remaining points of $$K$$ with finitely many members of $$\mathcal{U}$$, and conclude directly from the definition that $$K$$ is compact.

   5. Explain why

      $$
      \left\{\frac1n:n\in\mathbb{N}\right\}
      $$

      is not compact. You may use the theorem that compact subsets of $$\mathbb{R}$$ are closed.

4. **The Heine--Borel theorem in action.** Recall that a subset of $$\mathbb{R}^m$$ is compact if and only if it is closed and bounded.

   1. Fix $$\mathbf{a}\in\mathbb{R}^m$$ and $$R>0$$. Use the Heine--Borel theorem to prove that the closed ball

      $$
      \left\{
      \mathbf{x}\in\mathbb{R}^m:
      \lVert\mathbf{x}-\mathbf{a}\rVert\le R
      \right\}
      $$

      is compact.

   2. Use the Heine--Borel theorem to prove that the sphere

      $$
      \left\{
      \mathbf{x}\in\mathbb{R}^m:
      \lVert\mathbf{x}-\mathbf{a}\rVert=R
      \right\}
      $$

      is compact.

   3. Determine which of the following sets are compact. Prove each answer.

      $$
      [-2,5],
      \qquad
      (-2,5),
      \qquad
      [0,\infty),
      \qquad
      \left\{
      \mathbf{x}\in\mathbb{R}^m:
      1\le\lVert\mathbf{x}\rVert\le3
      \right\}.
      $$

   4. Give an example in $$\mathbb{R}$$ of each of the following:

      - a closed set that is not compact;
      - a bounded set that is not compact;
      - a set that is neither closed nor bounded.

      Briefly justify each example using the Heine--Borel theorem.

5. **Cantor counter-examples.**  Let $$\{C_1,C_2,C_3,\dots\}$$ be an infinite family of sets and consider the following properties.

     - $$C_k$$ is nonempty for all $$k$$
     - $$C_k$$ is closed for all $$k$$
     - $$C_k$$ is bounded for all $$k$$
     - $$C_{k+1}\subseteq C_k$$ for all $$k$$

   1. Give an example showing that if you drop the second property, $$\bigcap_{k=1}^\infty C_k$$ can be empty.
   2. Give an example showing that if you drop the third property, $$\bigcap_{k=1}^\infty C_k$$ can be empty.
   3. Give an example showing that if you drop the fourth property, $$\bigcap_{k=1}^\infty C_k$$ can be empty.


6. **A nonempty compact subset of $$\mathbb{R}$$ has a maximum.** Let $$K\subseteq\mathbb{R}$$ be nonempty and compact.

   1. Explain why $$K$$ is bounded above.
   2. Use the completeness axiom to explain why

      $$
      M=\sup(K)
      $$

      exists.

   3. Let $$r>0$$. Use the approximation property of the supremum to prove that there exists $$x\in K$$ such that

      $$
      M-r<x\le M.
      $$

   4. Prove that every ball centered at $$M$$ contains a point of $$K$$. Conclude that $$M$$ is an adherent point of $$K$$.
   5. Compact subsets of $$\mathbb{R}$$ are closed. Use this theorem to prove that $$M\in K$$.
   6. Conclude that $$K$$ has a maximum and that

      $$
      \max(K)=\sup(K).
      $$

   7. Adapt the argument to prove that $$K$$ also has a minimum and that

      $$
      \min(K)=\inf(K).
      $$


