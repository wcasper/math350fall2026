---
layout: post
title: Homework 2
permalink: /homework/hw2
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

**Note:** All sets will be subsets of $$\mathbb R$$ unless otherwise stated. Throughout,

$$
B(\mathbf{a};r)
=
\{\mathbf{x}\in\mathbb{R}^n:
\lVert\mathbf{x}-\mathbf{a}\rVert < r\}.
$$

For $$A\subseteq\mathbb{R}^n$$, the closure of $$A$$ is denoted by $$\overline{A}$$.


## Problems


1. **Well-ordering Principle.**
   Throughout this problem, let $$A$$ be a set and define $$B = \{-a: a\in A\}$$.

   1. Prove that $$A$$ is bounded below iff $$B$$ is bounded above.
   2. Use the Completeness Axiom to prove that if $$A$$ is non-empty and bounded below, then $$\inf(A)$$ exists and is equal to $$\sup(B)$$.
   3. Prove the \textbf{Well-Ordering Principle}: if $$A$$ is a nonempty set of positive integers, then it has a minimal element.

2. **Density of rationals and irrationals.**

   Let $$x$$ and $$y$$ be any real numbers with $$x < y$$.

   1. Use the Archimedian property to prove that there exists an integer $$n > 0$$ such that $$\frac{1}{n} < y-x$$.
   2. Use the Well-ordering Principle to prove that there is an integer $$m$$ with  $$m-1\leq nx < m$$.
   3. Prove that $$x < m/n < y$$.  This proves the **density property of the Rationals:** between any two real numbers, there's a rational number.
   4. Use the density property of the rationals to prove the **density property of the irrationals**: between any two real numbers, there's an irrational number.  [Hint: consider $$x+\sqrt{2}$$ and $$y+\sqrt{2}$$.]

3. **Interior and closure.** For each set below, determine its interior and closure. Then determine whether it is open, closed, both, or neither.

   1. $$(0,1]\subseteq\mathbb{R}$$;
   2. $$\mathbb{Z}\subseteq\mathbb{R}$$;
   3. $$\mathbb{Q}\subseteq\mathbb{R}$$;
   4.
      $$
      \{(x,y)\in\mathbb{R}^2:x^2+y^2<1\};
      $$

   5.
      $$
      \{(x,y)\in\mathbb{R}^2:x^2+y^2=1\};
      $$

   6.
      $$
      \{(x,y)\in\mathbb{R}^2:0<x<1,\ 0\le y\le1\}.
      $$

4. **Interior and set operations.** For $$A\subseteq\mathbb{R}^n$$, let $$A^\circ$$ denote the set of interior points of $$A$$.

   1. Prove that

      $$
      (A\cap B)^\circ=A^\circ\cap B^\circ.
      $$

   2. Prove that

      $$
      A^\circ\cup B^\circ
      \subseteq
      (A\cup B)^\circ.
      $$

   3. Give an example showing that the inclusion in part 2 can be strict.
   4. Prove that if $$A\subseteq B$$, then

      $$
      A^\circ\subseteq B^\circ.
      $$

   5. Prove that

      $$
      (A^\circ)^\circ=A^\circ.
      $$

5. **A two-dimensional accumulation set.** Define

   $$
   S=
   \left\{\frac1n:n\in\mathbb{N}\right\}
   $$

   and

   $$
   A=S\times S
   =
   \left\{
   \left(\frac1n,\frac1m\right):
   n,m\in\mathbb{N}
   \right\}.
   $$

   1. Prove that every point of $$A$$ is isolated: for each $$\mathbf{a}\in A$$, find an open ball centered at $$\mathbf{a}$$ containing no other point of $$A$$.
   2. Prove that every point of

      $$
      \big(\{0\}\times S\big)
      \cup
      \big(S\times\{0\}\big)
      \cup
      \{(0,0)\}
      $$

      is an accumulation point of $$A$$.

   3. Prove that there are no other accumulation points of $$A$$.
   4. Determine $$\overline{A}$$.
   5. Is $$A$$ closed? Is $$\overline{A}$$ closed? Justify both answers.

6. **Algebra of closures.** Let $$A,B\subseteq\mathbb{R}^n$$.

   1. Prove that if $$A\subseteq B$$, then

      $$
      \overline{A}\subseteq\overline{B}.
      $$

   2. Prove that

      $$
      \overline{A\cup B}
      =
      \overline{A}\cup\overline{B}.
      $$

   3. Prove that

      $$
      \overline{A\cap B}
      \subseteq
      \overline{A}\cap\overline{B}.
      $$

   4. Give an example in which the inclusion in part 3 is strict.
   5. Prove that

      $$
      \overline{\overline{A}}=\overline{A}.
      $$

7. **Component intervals.** Define

   $$
   U=
   \left\{
   x\in\mathbb{R}:
   (x^2-1)(x^2-4)>0
   \right\}.
   $$

   1. Solve the inequality and prove that

      $$
      U=(-\infty,-2)\cup(-1,1)\cup(2,\infty).
      $$

   2. Prove directly that $$U$$ is open.
   3. Prove that each of the three displayed intervals is a component interval of $$U$$.
   4. Prove that these are the only component intervals of $$U$$.
   5. Determine the closure of each component interval and the closure of $$U$$.

8. **Disjoint open intervals.** Let $$\mathcal{I}$$ be a family of pairwise disjoint, nonempty open intervals in $$\mathbb{R}$$.

   1. Explain why every interval $$I\in\mathcal{I}$$ contains a rational number.
   2. For each $$I\in\mathcal{I}$$, choose one rational number $$q_I\in I$$.
   3. Prove that the function

      $$
      I\longmapsto q_I
      $$

      from $$\mathcal{I}$$ to $$\mathbb{Q}$$ is injective.
   4. Deduce that $$\mathcal{I}$$ is countable.
   5. Use this result to explain why an open subset of $$\mathbb{R}$$ can have only countably many component intervals.
   6. Give an uncountable family of pairwise disjoint, nonempty subsets of $$\mathbb{R}$$ and explain why this does not contradict your result.

9. **Closed balls and spheres.** Fix $$\mathbf{a}\in\mathbb{R}^n$$ and $$r>0$$. Define

   $$
   D=
   \{\mathbf{x}\in\mathbb{R}^n:
   \lVert\mathbf{x}-\mathbf{a}\rVert\le r\}
   $$

   and

   $$
   S=
   \{\mathbf{x}\in\mathbb{R}^n:
   \lVert\mathbf{x}-\mathbf{a}\rVert=r\}.
   $$

   1. Let $$\mathbf{x}\notin D$$. Construct a ball centered at $$\mathbf{x}$$ that does not intersect $$D$$.
   2. Deduce that $$D$$ is closed.
   3. Express $$S$$ as an intersection of two closed sets, or prove directly that its complement is open.
   4. Deduce that $$S$$ is closed.
   5. Determine the interior and closure of both $$D$$ and $$S$$.

10. **The closure as the smallest closed set.** Let $$A\subseteq\mathbb{R}^n$$.

    1. Prove that

       $$
       A\subseteq\overline{A}.
       $$

    2. Prove that $$\overline{A}$$ is closed.
    3. Suppose that $$F$$ is closed and

       $$
       A\subseteq F.
       $$

       Prove that

       $$
       \overline{A}\subseteq F.
       $$

    4. Deduce that

       $$
       \overline{A}
       =
       \bigcap
       \{F\subseteq\mathbb{R}^n:
       F\text{ is closed and }A\subseteq F\}.
       $$

    5. Use this characterization to prove that

       $$
       \overline{\mathbb{Q}^n}=\mathbb{R}^n.
       $$

       You may use the fact that every open interval contains a rational number.




