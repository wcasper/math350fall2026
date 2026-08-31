---
layout: post
title: Homework 1
permalink: /homework/hw1
---

### Directions
Solve the following problems and write up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

You will be graded based on *completion* of all of the assigned problems, along with in-depth grading of *select* problems which will not be revealed until after the homework is graded.

**Remember:** Success in any math class is based on *practice*.  The assigned homework problems are the **bare minimum**.  You should strive to do as many problems as possible from the textbook.

**Note:** All sets will be subsets of $$\mathbb R$$ unless otherwise stated.

## Problems

1. **Consequences of the field axioms.** Let $$x,y,z\in\mathbb{R}$$. Prove each statement directly from the field axioms and previously established consequences of those axioms.

   1. If $$x+z=y+z$$, then $$x=y$$.
   2. If $$xz=yz$$ and $$z\ne0$$, then $$x=y$$.
   3. Prove that

      $$
      (-x)y=-(xy).
      $$

   4. Deduce that

      $$
      (-x)(-y)=xy.
      $$

   5. Prove that if $$xy=0$$, then $$x=0$$ or $$y=0$$.

2. **Order and reciprocals.** Suppose that

   $$
   0<a<b.
   $$

   1. Prove that $$ab>0$$.
   2. Prove that $$a^{-1}>0$$ and $$b^{-1}>0$$.
   3. Prove that

      $$
      \frac1b<\frac1a.
      $$

   4. Prove the more precise identity

      $$
      \frac1a-\frac1b=\frac{b-a}{ab},
      $$

      and explain how it gives another proof of the preceding inequality.
   5. Give an example showing that the conclusion in part 3 need not hold if the hypothesis $$0<a<b$$ is replaced by only $$a<b$$.

3. **A proof by induction.** Prove that for every $$n\in\mathbb{N}$$,

   $$
   1+3+5+\cdots+(2n-1)=n^2.
   $$

   Your proof must proceed by defining

   $$
   S=
   \left\{
   n\in\mathbb{N}:
   1+3+\cdots+(2n-1)=n^2
   \right\},
   $$

   proving that $$S$$ is inductive, and then using the definition of $$\mathbb{N}$$.

   Next, use this identity to prove that

   $$
   n^2\ge 2n-1
   $$

   for every $$n\in\mathbb{N}$$, and determine exactly when equality holds.

4. **Finding a supremum.** Define

   $$
   A=
   \left\{
   \frac{3n+2}{n+1}:n\in\mathbb{N}
   \right\}.
   $$

   1. Rewrite the elements of $$A$$ in the form

      $$
      3-\frac{c}{n+1}
      $$

      for an appropriate constant $$c$$.
   2. Prove that $$A$$ is nonempty and bounded above.
   3. Prove that $$3$$ is an upper bound of $$A$$.
   4. Given $$\varepsilon>0$$, use the Archimedean property to find $$n\in\mathbb{N}$$ such that

      $$
      3-\varepsilon<
      \frac{3n+2}{n+1}.
      $$

   5. Deduce that

      $$
      \sup(A)=3.
      $$

   6. Determine $$\inf(A)$$ and decide whether $$A$$ has a maximum or minimum.

5. **Suprema of products.** Let $$A,B\subseteq[0,\infty)$$ be nonempty sets that are bounded above. Define

   $$
   C=\{xy:x\in A,\ y\in B\}.
   $$

   Let

   $$
   a=\sup(A)
   \qquad\text{and}\qquad
   b=\sup(B).
   $$

   1. Prove that $$C$$ is bounded above and that

      $$
      \sup(C)\le ab.
      $$

   2. Suppose that $$a>0$$ and $$b>0$$. Given $$\varepsilon>0$$, use the approximation property to choose $$x\in A$$ and $$y\in B$$ sufficiently close to $$a$$ and $$b$$ to prove that

      $$
      xy>ab-\varepsilon.
      $$

      *Hint:* Choose $$x$$ and $$y$$ so that

      $$
      x>a-\frac{\varepsilon}{2b}
      $$

      and

      $$
      y>b-\frac{\varepsilon}{2a}.
      $$

   3. Handle separately the cases $$a=0$$ or $$b=0$$.
   4. Conclude that

      $$
      \sup(C)=\sup(A)\sup(B).
      $$

6. **An indexed family of intervals.** For each $$n\in\mathbb{N}$$, define

   $$
   A_n=
   \left(-\frac1n,\,2+\frac1n\right).
   $$

   Determine each of the following sets:

   $$
   \bigcup_{n\in\mathbb{N}}A_n,
   \qquad
   \bigcap_{n\in\mathbb{N}}A_n,
   \qquad
   \bigcup_{n\in\mathbb{N}}(\mathbb{R}-A_n),
   \qquad
   \bigcap_{n\in\mathbb{N}}(\mathbb{R}-A_n).
   $$

   Prove your answers using the definitions of indexed unions and intersections. You may then use De Morgan's laws to check the last two answers.

   In proving your answer for the intersection, use the Archimedean property to show that every $$x<0$$ and every $$x>2$$ is excluded from at least one of the sets $$A_n$$.

7. **Images and inverse images.** Let $$f:A\to B$$ be a function. For $$S\subseteq A$$ and $$T\subseteq B$$, define

   $$
   f(S)=\{f(x):x\in S\}
   $$

   and

   $$
   f^{-1}(T)=\{x\in A:f(x)\in T\}.
   $$

   Prove the following statements:

   1. For all $$S_1,S_2\subseteq A$$,

      $$
      f(S_1\cup S_2)=f(S_1)\cup f(S_2).
      $$

   2. For all $$S_1,S_2\subseteq A$$,

      $$
      f(S_1\cap S_2)\subseteq f(S_1)\cap f(S_2).
      $$

   3. Equality holds in part 2 for every pair $$S_1,S_2\subseteq A$$ if $$f$$ is injective.
   4. Give a specific example showing that equality in part 2 can fail when $$f$$ is not injective.
   5. For all $$T_1,T_2\subseteq B$$,

      $$
      f^{-1}(T_1\cap T_2)
      =
      f^{-1}(T_1)\cap f^{-1}(T_2).
      $$

8. **Composition and inverse functions.** Let

   $$
   f:A\to B
   \qquad\text{and}\qquad
   g:B\to C.
   $$

   1. Prove that if $$g\circ f$$ is injective, then $$f$$ is injective.
   2. Prove that if $$g\circ f$$ is surjective, then $$g$$ is surjective.
   3. Give an example in which $$g\circ f$$ is injective but $$g$$ is not injective.
   4. Give an example in which $$g\circ f$$ is surjective but $$f$$ is not surjective.
   5. Suppose that $$f$$ and $$g$$ are bijective. Prove that $$g\circ f$$ is bijective and that

      $$
      (g\circ f)^{-1}=f^{-1}\circ g^{-1}.
      $$

9. **Countability of finite sequences.** For each $$n\in\mathbb{N}$$, let

   $$
   S_n=\mathbb{Z}^n
   $$

   be the set of all integer sequences of length $$n$$.

   1. Prove that $$S_n$$ is countable for every $$n\in\mathbb{N}$$.
   2. Let

      $$
      S=\bigcup_{n\in\mathbb{N}}S_n.
      $$

      Interpret $$S$$ as the set of all finite sequences of integers and prove that $$S$$ is countable.
   3. Let $$P$$ be the set of all polynomials with integer coefficients. Construct a surjection from $$S$$ onto $$P$$.
   4. Deduce that the set of all polynomials with integer coefficients is countable.

10. **Algebraic and transcendental numbers.** A real number is called algebraic if it is a root of a nonzero polynomial with integer coefficients. A real number that is not algebraic is called transcendental.

    1. For each nonzero polynomial $$p$$ with integer coefficients, let

       $$
       Z_p=\{x\in\mathbb{R}:p(x)=0\}.
       $$

       Explain why $$Z_p$$ is finite.
    2. Prove that the set $$\mathcal{A}$$ of all algebraic real numbers can be written as

       $$
       \mathcal{A}
       =
       \bigcup_{\substack{p\in\mathbb{Z}[x]\\p\ne0}}Z_p.
       $$

    3. Use Problem 9 and the theorem on countable unions to prove that $$\mathcal{A}$$ is countable.
    4. Use the uncountability of $$\mathbb{R}$$ to prove that transcendental real numbers exist.
    5. Prove the stronger statement that the set of transcendental real numbers is uncountable.

