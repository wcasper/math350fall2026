---
layout: post
title: "Lecture 6"
date: 2026-09-14
---

## Open and closed sets

### Key words

arbitrary union, finite intersection, component interval, disjoint intervals, representation theorem for open subsets of the real line, closed set, complement, adherent point, accumulation point, isolated point

### Reading assignment

Apostol, Chapter 3: the sections on unions and intersections of open sets, the representation of open subsets of $$\mathbb{R}$$ by disjoint intervals, closed sets, adherent points, and accumulation points.

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec06/lec06.pdf)

## Practice problems

Throughout, for $$\mathbf{a}\in\mathbb{R}^n$$ and $$r>0$$, let

$$
B(\mathbf{a};r)
=
\{\mathbf{x}\in\mathbb{R}^n:
\lVert\mathbf{x}-\mathbf{a}\rVert<r\}.
$$

Recall that $$\mathbf{x}$$ is an adherent point of $$A$$ if every ball centered at $$\mathbf{x}$$ contains a point of $$A$$. It is an accumulation point of $$A$$ if every ball centered at $$\mathbf{x}$$ contains a point of $$A$$ different from $$\mathbf{x}$$.

1. **Open, closed, both, or neither.** Classify each set as open, closed, both open and closed, or neither. Prove each answer from the definitions or from the theorems established in lecture.

   1. $$(0,1]\subseteq\mathbb{R}$$;
   2. $$\mathbb{Z}\subseteq\mathbb{R}$$;
   3. $$\mathbb{Q}\subseteq\mathbb{R}$$;
   4. 
      $$
      \{(x,y)\in\mathbb{R}^2:y>0\};
      $$

   5.
      $$
      \{(x,y)\in\mathbb{R}^2:x^2+y^2=1\};
      $$

   6. $$\varnothing\subseteq\mathbb{R}^n$$ and $$\mathbb{R}^n\subseteq\mathbb{R}^n$$.

   You may use the fact that every open interval contains both a rational and an irrational number.

2. **Adherent and accumulation points.** Let

   $$
   A=(0,1)\cup\{2\}\cup
   \left\{3+\frac1n:n\in\mathbb{N}\right\}.
   $$

   Determine all of the following sets and justify your answers:

   1. the interior points of $$A$$;
   2. the adherent points of $$A$$;
   3. the accumulation points of $$A$$;
   4. the points of $$A$$ that are not accumulation points of $$A$$.

   For each claimed accumulation point, show directly that every ball contains a different point of $$A$$. For each point that is not an accumulation point, exhibit a ball that contains no other point of $$A$$.

3. **Closed sets and accumulation points.** Let $$F\subseteq\mathbb{R}^n$$.

   1. Suppose that $$F$$ is closed and that $$\mathbf{x}$$ is an accumulation point of $$F$$. Prove that $$\mathbf{x}\in F$$.
   2. Conversely, suppose that $$F$$ contains all of its accumulation points. Let $$\mathbf{x}\notin F$$. Prove that there exists $$r>0$$ such that

      $$
      B(\mathbf{x};r)\cap F=\varnothing.
      $$

   3. Deduce that $$\mathbb{R}^n-F$$ is open.
   4. Conclude that a set is closed if and only if it contains all of its accumulation points.

4. **Set operations with closed sets.** Use De Morgan's laws and the corresponding results for open sets to prove the following.

   1. The intersection of an arbitrary family of closed sets is closed.
   2. The union of finitely many closed sets is closed.
   3. Give an example showing that an infinite union of closed sets need not be closed.
   4. Give an example showing that an infinite intersection of open sets need not be open.
   5. Explain why the words “arbitrary” and “finite” occur in different places in the open-set and closed-set theorems.

5. **A closed set built from infinitely many points.** Define

   $$
   F=
   \left\{\frac1n:n\in\mathbb{N}\right\}\cup\{0\}.
   $$

   1. Prove that $$0$$ is an accumulation point of $$F$$.
   2. Prove that every point $$1/n$$ is not an accumulation point of $$F$$.
   3. Prove that no point outside $$F$$ is an accumulation point of $$F$$.
   4. Use the characterization from Problem 3 to conclude that $$F$$ is closed.
   5. Show that

      $$
      \left\{\frac1n:n\in\mathbb{N}\right\}
      $$

      is not closed.

6. **Finding component intervals.** Let

   $$
   U=
   \mathbb{R}-
   \left(
   \{0\}\cup
   \left\{\frac1n:n\in\mathbb{N}\right\}
   \right).
   $$

   1. Prove that $$U$$ is open.
   2. Show that the component intervals of $$U$$ are

      $$
      (-\infty,0),
      \qquad
      \left(\frac1{n+1},\frac1n\right)
      \quad(n\in\mathbb{N}),
      \qquad
      (1,\infty).
      $$

   3. Prove that each displayed interval is maximal among intervals contained in $$U$$.
   4. Verify directly that these intervals are pairwise disjoint and that their union is $$U$$.

7. **Why there are only countably many components.** Let $$U\subseteq\mathbb{R}$$ be open, and let $$\mathcal{C}$$ be the family of component intervals of $$U$$.

   1. Explain why every $$I\in\mathcal{C}$$ contains a rational number.
   2. For each $$I\in\mathcal{C}$$, choose a rational number $$q_I\in I$$.
   3. Prove that the function

      $$
      \Phi:\mathcal{C}\to\mathbb{Q},
      \qquad
      \Phi(I)=q_I,
      $$

      is injective.
   4. Deduce that $$\mathcal{C}$$ is countable.
   5. Explain why the same argument does not show that an arbitrary family of pairwise disjoint subsets of $$\mathbb{R}$$ is countable.

8. **Suprema and accumulation points.** Let $$A\subseteq\mathbb{R}$$ be nonempty and bounded above, and let

   $$
   s=\sup(A).
   $$

   1. Prove that $$s$$ is always an adherent point of $$A$$.
   2. Suppose that $$s\notin A$$. Prove that $$s$$ is an accumulation point of $$A$$.
   3. Give an example in which $$s\in A$$ but $$s$$ is not an accumulation point of $$A$$.
   4. Give an example in which $$s\in A$$ and $$s$$ is an accumulation point of $$A$$.
   5. State and prove the corresponding results for the infimum of a nonempty set bounded below.

9. **The set of accumulation points is closed.** For a set $$A\subseteq\mathbb{R}^n$$, let

   $$
   A'
   =
   \{\mathbf{x}\in\mathbb{R}^n:
   \mathbf{x}\text{ is an accumulation point of }A\}.
   $$

   Prove that $$A'$$ is closed.

   *Hint:* Suppose that $$\mathbf{x}\notin A'$$. Then there exists $$r>0$$ such that

   $$
   B(\mathbf{x};r)
   $$

   contains no point of $$A$$ other than possibly $$\mathbf{x}$$. Show that every point of

   $$
   B\left(\mathbf{x};\frac r2\right)
   $$

   also fails to be an accumulation point of $$A$$.

10. **A geometric example in the plane.** Define

    $$
    A=
    \{(x,y)\in\mathbb{R}^2:0<x^2+y^2<1\}.
    $$

    1. Prove that $$A$$ is open.
    2. Determine all adherent points of $$A$$.
    3. Determine all accumulation points of $$A$$.
    4. Is the origin an interior point, an adherent point, an accumulation point, or more than one of these?
    5. For a point $$\mathbf{a}$$ satisfying $$\lVert\mathbf{a}\rVert=1$$, prove directly that every ball centered at $$\mathbf{a}$$ contains a point of $$A$$.
    6. Determine whether $$A$$ is closed and justify your answer.



