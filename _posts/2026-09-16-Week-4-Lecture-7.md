---
layout: post
title: "Lecture 7"
date: 2026-09-16
---

## Accumulation points and closure

### Key words

adherent point, accumulation point, isolated point, closure, closed set, dense set, closed ball, derived set, neighborhood characterization

### Reading assignment

Apostol, Chapter 3: Theorems 3.17–3.22 and the surrounding sections on adherent points, accumulation points, closures, and closed sets.

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec07/lec07.pdf)

## Practice problems

Throughout, let

$$
B(\mathbf{x};r)
=
\{\mathbf{y}\in\mathbb{R}^n:
\lVert\mathbf{x}-\mathbf{y}\rVert<r\}.
$$

Recall that $$\mathbf{x}$$ is an adherent point of $$A$$ if every ball centered at $$\mathbf{x}$$ contains a point of $$A$$. It is an accumulation point of $$A$$ if every ball centered at $$\mathbf{x}$$ contains a point of $$A$$ different from $$\mathbf{x}$$. The closure of $$A$$, denoted by $$\overline{A}$$, is the set of all adherent points of $$A$$.

1. **Adherent, accumulation, and isolated points.** Let

   $$
   A=
   (0,1)\cup\{2\}\cup
   \left\{3+\frac1n:n\in\mathbb{N}\right\}.
   $$

   Determine each of the following sets and prove your answers:

   1. the interior points of $$A$$;
   2. the adherent points of $$A$$;
   3. the accumulation points of $$A$$;
   4. the points of $$A$$ that are not accumulation points of $$A$$;
   5. the closure $$\overline{A}$$.

   For every point that you claim is isolated, exhibit an open ball containing no other point of $$A$$.

2. **Finite sets have no accumulation points.** Let

   $$
   F=\{\mathbf{x}_1,\ldots,\mathbf{x}_m\}
   \subseteq\mathbb{R}^n
   $$

   be a nonempty finite set.

   1. Fix $$\mathbf{x}\in\mathbb{R}^n$$. Explain why the set

      $$
      \{
      \lVert\mathbf{x}-\mathbf{x}_j\rVert:
      \mathbf{x}_j\ne\mathbf{x}
      \}
      $$

      is either empty or has a positive minimum.

   2. Use this observation to prove that $$F$$ has no accumulation points.
   3. Prove that

      $$
      \overline{F}=F.
      $$

   4. Conclude that every finite subset of $$\mathbb{R}^n$$ is closed.

3. **Accumulation points contain infinitely many nearby points.** Let $$\mathbf{x}$$ be an accumulation point of $$A\subseteq\mathbb{R}^n$$.

   1. Prove that for every $$r>0$$, the ball $$B(\mathbf{x};r)$$ contains infinitely many points of $$A$$.
   2. Prove that one can choose distinct points

      $$
      \mathbf{x}_k\in A
      $$

      such that

      $$
      0<
      \lVert\mathbf{x}_k-\mathbf{x}\rVert
      <
      \frac1k
      $$

      for every $$k\in\mathbb{N}$$.

   3. Explain why the points $$\mathbf{x}_k$$ necessarily become arbitrarily close to $$\mathbf{x}$$.
   4. Is the conclusion of part 2 possible if $$\mathbf{x}$$ is merely an adherent point? Give a counterexample.

4. **Closures of familiar sets.** Determine the closure and the set of accumulation points of each set below. Prove your answers.

   1. $$\mathbb{Z}\subseteq\mathbb{R}$$;
   2. $$\mathbb{Q}\subseteq\mathbb{R}$$;
   3. $$(0,1)\cap\mathbb{Q}$$;
   4.
      $$
      \left\{\frac{(-1)^n}{n}:n\in\mathbb{N}\right\};
      $$

   5.
      $$
      \left\{
      \left(\frac1n,\frac1m\right):
      n,m\in\mathbb{N}
      \right\}
      \subseteq\mathbb{R}^2.
      $$

   You may use the fact that every open interval contains a rational number.

5. **Closure and set operations.** Let $$A,B\subseteq\mathbb{R}^n$$.

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

6. **Closure as the smallest closed set.** Let $$A\subseteq\mathbb{R}^n$$.

   1. Prove that $$A\subseteq\overline{A}$$.
   2. Prove that $$\overline{A}$$ is closed.
   3. Suppose that $$F$$ is closed and $$A\subseteq F$$. Prove that

      $$
      \overline{A}\subseteq F.
      $$

   4. Deduce that

      $$
      \overline{A}
      =
      \bigcap
      \left\{
      F\subseteq\mathbb{R}^n:
      F\text{ is closed and }A\subseteq F
      \right\}.
      $$

   Thus $$\overline{A}$$ is the smallest closed set containing $$A$$.

7. **Accumulation points of a union.** For $$A\subseteq\mathbb{R}^n$$, write $$A'$$ for the set of accumulation points of $$A$$.

   1. Prove that

      $$
      A'\cup B'
      \subseteq
      (A\cup B)'.
      $$

   2. Suppose that

      $$
      \mathbf{x}\notin A'
      \qquad\text{and}\qquad
      \mathbf{x}\notin B'.
      $$

      Find radii $$r_A,r_B>0$$ such that the corresponding balls contain no points of $$A$$ or $$B$$ other than possibly $$\mathbf{x}$$.

   3. Use the radius

      $$
      r=\min\{r_A,r_B\}
      $$

      to prove that $$\mathbf{x}\notin(A\cup B)'$$.
   4. Conclude that

      $$
      (A\cup B)'=A'\cup B'.
      $$

   5. Give an example showing that the corresponding identity can fail for an infinite union.

8. **The set of accumulation points is closed.** Let

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

9. **Closed balls and spheres.** Fix $$\mathbf{a}\in\mathbb{R}^n$$ and $$R>0$$. Define

   $$
   D=
   \{\mathbf{x}\in\mathbb{R}^n:
   \lVert\mathbf{x}-\mathbf{a}\rVert\le R\}
   $$

   and

   $$
   S=
   \{\mathbf{x}\in\mathbb{R}^n:
   \lVert\mathbf{x}-\mathbf{a}\rVert=R\}.
   $$

   1. Let $$\mathbf{x}\notin D$$ and define

      $$
      r=
      \lVert\mathbf{x}-\mathbf{a}\rVert-R.
      $$

      Prove that $$r>0$$ and that

      $$
      B(\mathbf{x};r)\cap D=\varnothing.
      $$

   2. Deduce that $$D$$ is closed.
   3. Prove that $$S$$ is closed.
   4. Determine the interior and closure of $$D$$.
   5. Determine the interior and closure of $$S$$.

10. **Dense subsets of Euclidean space.** A set $$A\subseteq\mathbb{R}^n$$ is called dense if

    $$
    \overline{A}=\mathbb{R}^n.
    $$

    1. Prove that $$A$$ is dense if and only if every nonempty open ball contains a point of $$A$$.
    2. Prove that $$\mathbb{Q}$$ is dense in $$\mathbb{R}$$.
    3. Prove that $$\mathbb{R}-\mathbb{Q}$$ is also dense in $$\mathbb{R}$$.
    4. Prove that $$\mathbb{Q}^n$$ is dense in $$\mathbb{R}^n$$.

       *Hint:* If

       $$
       \mathbf{x}=(x_1,\ldots,x_n)
       $$

       and $$r>0$$, choose rational numbers $$q_i$$ satisfying

       $$
       \lvert q_i-x_i\rvert<\frac{r}{\sqrt n}.
       $$

    5. Give an example of two disjoint dense subsets of $$\mathbb{R}$$.




