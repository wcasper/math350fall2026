---
layout: post
title: "Lecture 2"
date: 2026-08-26
---

## Natural numbers and completeness

### Key words

inductive sets, natural numbers, mathematical induction, upper bounds, lower bounds, maximum, minimum, supremum, infimum, completeness axiom, decimal expansions, approximation property, Archimedean property

### Reading assignment

Apostol, Chapter 1: the sections on integers and rational numbers, upper bounds and suprema, the completeness axiom, and properties of suprema, through the Archimedean property (Theorem 1.18).

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec02/lec02.pdf)

## Practice problems

Throughout, $$\mathbb{N}=\{1,2,3,\ldots\}$$. You may use results established in lecture, but justify your answers using definitions and those results rather than limits or other material not yet developed.

1. **Working with inductive sets.** Recall that a subset $$S\subseteq\mathbb{R}$$ is inductive if $$1\in S$$ and $$x\in S$$ implies $$x+1\in S$$.

   1. Determine which of the following sets are inductive, and justify each answer:

      $$
      [1,\infty),\qquad (1,\infty),\qquad
      \mathbb{Z}\cup\left\{\frac12\right\},\qquad
      \left\{\frac{k}{2}:k\in\mathbb{Z},\ k\ge 2\right\}.
      $$

   2. If $$A$$ and $$B$$ are inductive, prove that both $$A\cap B$$ and $$A\cup B$$ are inductive.
   3. Suppose $$A\cup B$$ is inductive. Must at least one of $$A$$ and $$B$$ be inductive? Give a proof or a counterexample.

2. **Induction as a statement about sets.** Prove that for every $$n\in\mathbb{N}$$,

   $$
   \frac{1}{1\cdot2}+\frac{1}{2\cdot3}+\cdots+
   \frac{1}{n(n+1)}=\frac{n}{n+1}.
   $$

   Write your proof by defining the set of positive integers for which the identity holds, showing that this set is inductive, and applying the definition of $$\mathbb{N}$$.

3. **Bounds versus extrema.** For each set below, determine its supremum, infimum, maximum, and minimum, whenever they exist. Also describe the set of all real upper bounds and the set of all real lower bounds.

   1. $$A=(-2,3].$$
   2. $$B=\{x\in\mathbb{R}:\lvert x-1\rvert<2\}.$$
   3. $$C=\{-4\}\cup(0,2).$$
   4. $$D=\left\{\dfrac{3n+1}{n+1}:n\in\mathbb{N}\right\}.$$

   For the last set, use the Archimedean property to prove that your proposed supremum is the least upper bound.

4. **Why the hypotheses matter.** The completeness axiom applies to nonempty sets that are bounded above.

   1. Show that every real number is an upper bound of the empty set.
   2. Explain why the empty set nevertheless has no supremum in $$\mathbb{R}$$.
   3. Show that $$[0,\infty)$$ has no real upper bound, and hence no supremum in $$\mathbb{R}$$.
   4. Give a nonempty bounded set whose supremum is not an element of the set. Explain why this does not contradict completeness.

5. **Comparing sets and their suprema.** Let $$A$$ and $$B$$ be nonempty subsets of $$\mathbb{R}$$ that are bounded above.

   1. Prove that if $$A\subseteq B$$, then $$\sup(A)\le\sup(B)$$.
   2. Give an example with $$A\subsetneq B$$ but $$\sup(A)=\sup(B)$$.
   3. Prove that

      $$
      \sup(A\cup B)=\max\{\sup(A),\sup(B)\}.
      $$

   4. If $$A\cap B\ne\varnothing$$, must

      $$
      \sup(A\cap B)=\min\{\sup(A),\sup(B)\}?
      $$

      Give a proof or a counterexample.

6. **Getting infima from completeness.** Let $$S\subseteq\mathbb{R}$$ be nonempty and bounded below, and define

   $$
   -S=\{-x:x\in S\}.
   $$

   1. Prove that $$-S$$ is nonempty and bounded above.
   2. Use the completeness axiom to prove that $$S$$ has an infimum and that

      $$
      \inf(S)=-\sup(-S).
      $$

   3. Deduce the lower-bound version of the approximation property: for every $$\varepsilon>0$$, there exists $$x\in S$$ such that

      $$
      \inf(S)\le x<\inf(S)+\varepsilon.
      $$

7. **Recognizing a supremum.** Suppose $$S\subseteq\mathbb{R}$$ is nonempty and $$b\in\mathbb{R}$$. Prove that $$b=\sup(S)$$ if and only if both of the following hold:

   - $$x\le b$$ for every $$x\in S$$;
   - for every $$\varepsilon>0$$, there exists $$x\in S$$ with $$x>b-\varepsilon$$.

   Then give an example showing that the second condition alone does not imply that $$b=\sup(S)$$. Your example should use a set that is bounded above.

8. **Differences of sets.** Let $$A,B\subseteq\mathbb{R}$$ be nonempty and bounded above and below. Define

   $$
   A-B=\{a-b:a\in A,\ b\in B\}.
   $$

   1. Use the additive property of suprema and Problem 6 to prove that

      $$
      \sup(A-B)=\sup(A)-\inf(B).
      $$

   2. Find a corresponding formula for $$\inf(A-B)$$ and prove it.
   3. Compute these bounds when $$A=(1,4]$$ and $$B=[-2,3)$$. Does $$A-B$$ attain either bound? Justify your answer.

9. **Decimals without limits.** For each $$k\in\mathbb{N}$$, let

   $$
   s_k=\frac{9}{10}+\frac{9}{10^2}+\cdots+\frac{9}{10^k}.
   $$

   Following the definition in lecture, define

   $$
   0.999\ldots=\sup\{s_k:k\in\mathbb{N}\}.
   $$

   1. Prove by induction that $$s_k=1-10^{-k}$$.
   2. Show that the set of these decimal approximations is nonempty and bounded above.
   3. Use the Archimedean property to prove that $$0.999\ldots=1$$.

   *Hint:* First prove by induction that $$10^k\ge k+1$$. Then, for a given $$\varepsilon>0$$, find $$k$$ such that $$10^{-k}<\varepsilon$$. Do not assume any facts about limits or infinite geometric series.

10. **Small positive numbers and large integers.** Use the Archimedean property to prove each statement.

    1. For every $$\varepsilon>0$$, there exists $$N\in\mathbb{N}$$ such that

       $$
       0<\frac1n<\varepsilon
       \qquad\text{for every }n\in\mathbb{N}\text{ with }n\ge N.
       $$

    2. If $$x\ge0$$ and $$x<1/n$$ for every $$n\in\mathbb{N}$$, then $$x=0$$.
    3. If $$a<b$$, then there exists $$n\in\mathbb{N}$$ such that

       $$
       a<a+\frac1n<b.
       $$

    In each part, indicate precisely how you choose the positive integer supplied by the Archimedean property.

