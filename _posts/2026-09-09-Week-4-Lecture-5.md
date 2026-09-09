---
layout: post
title: "Lecture 5"
date: 2026-09-09
---

## Euclidean space and open sets

### Key words

Euclidean space, vector addition, scalar multiplication, dot product, Euclidean norm, distance, positivity, symmetry, triangle inequality, scaling property, Cauchy-Schwarz inequality, open ball, interior point, open set

### Reading assignment

Apostol, Chapter 3: the sections introducing Euclidean space, open balls, interior points, and open sets.

### Slides

- [Link to slides](https://wcasper.github.io/math350fall2026/slides/lec05/lec05.pdf)

## Practice problems

Throughout, the Euclidean norm of a vector

$$
\mathbf{x}=(x_1,\ldots,x_n)\in\mathbb{R}^n
$$

is

$$
\lVert\mathbf{x}\rVert
=
\sqrt{x_1^2+\cdots+x_n^2},
$$

and the open ball of radius $$r>0$$ centered at $$\mathbf{a}$$ is

$$
B(\mathbf{a};r)
=
\{\mathbf{x}\in\mathbb{R}^n:
\lVert\mathbf{x}-\mathbf{a}\rVert<r\}.
$$

You may use the triangle inequality and the Cauchy-Schwarz inequality, but justify all claims about interior points and open sets directly from the definitions or from results already proved.

1. **Calculations in Euclidean space.** Let

   $$
   \mathbf{x}=(1,-2,3),
   \qquad
   \mathbf{y}=(4,0,-1).
   $$

   Compute each of the following:

   $$
   \mathbf{x}+\mathbf{y},
   \qquad
   2\mathbf{x}-3\mathbf{y},
   \qquad
   \mathbf{x}\cdot\mathbf{y},
   \qquad
   \lVert\mathbf{x}\rVert,
   \qquad
   \lVert\mathbf{x}-\mathbf{y}\rVert.
   $$

   Then determine whether the angle between $$\mathbf{x}$$ and $$\mathbf{y}$$ is acute, right, or obtuse. Justify your answer using the sign of their dot product.

2. **The reverse triangle inequality.** Let $$\mathbf{x},\mathbf{y}\in\mathbb{R}^n$$.

   1. Apply the triangle inequality to

      $$
      \mathbf{x}=(\mathbf{x}-\mathbf{y})+\mathbf{y}
      $$

      to prove that

      $$
      \lVert\mathbf{x}\rVert-\lVert\mathbf{y}\rVert
      \le
      \lVert\mathbf{x}-\mathbf{y}\rVert.
      $$

   2. Reverse the roles of $$\mathbf{x}$$ and $$\mathbf{y}$$ to prove that

      $$
      \big\lvert
      \lVert\mathbf{x}\rVert-\lVert\mathbf{y}\rVert
      \big\rvert
      \le
      \lVert\mathbf{x}-\mathbf{y}\rVert.
      $$

   3. Find two distinct vectors for which equality holds.

3. **Comparing distances coordinate by coordinate.** Let

   $$
   \mathbf{x}=(x_1,\ldots,x_n)
   \qquad\text{and}\qquad
   \mathbf{y}=(y_1,\ldots,y_n).
   $$

   1. Prove that for every $$i$$,

      $$
      \lvert x_i-y_i\rvert
      \le
      \lVert\mathbf{x}-\mathbf{y}\rVert.
      $$

   2. Prove that

      $$
      \lVert\mathbf{x}-\mathbf{y}\rVert
      \le
      \sqrt{n}\max_{1\le i\le n}\lvert x_i-y_i\rvert.
      $$

   3. Deduce that if

      $$
      \lvert x_i-y_i\rvert<\frac{r}{\sqrt n}
      $$

      for every $$i$$, then $$\mathbf{x}\in B(\mathbf{y};r)$$.

4. **Open balls in one dimension.** Let $$a\in\mathbb{R}$$ and $$r>0$$.

   1. Prove that

      $$
      B(a;r)=(a-r,a+r).
      $$

   2. Let $$x\in(a,b)$$. Show that

      $$
      r=\min\{x-a,b-x\}
      $$

      is positive and that

      $$
      B(x;r)\subseteq(a,b).
      $$

   3. Conclude directly from the definition that every open interval is an open subset of $$\mathbb{R}$$.
   4. Explain why neither endpoint of $$[a,b]$$ is an interior point of $$[a,b]$$.

5. **Determining interiors.** For each of the following subsets of the indicated Euclidean space, determine the set of all interior points. Prove your answers.

   1. $$[0,1]\subseteq\mathbb{R}$$;
   2. $$[0,1)\cup\{2\}\subseteq\mathbb{R}$$;
   3. $$\mathbb{Q}\subseteq\mathbb{R}$$;
   4. 
      $$
      \{(x,y)\in\mathbb{R}^2:x^2+y^2\le1\};
      $$

   5.
      $$
      \{(x,y)\in\mathbb{R}^2:y=0\}.
      $$

   You may use the fact that every open interval contains both a rational and an irrational number.

6. **A ball inside a ball.** Suppose

   $$
   \mathbf{x}\in B(\mathbf{a};r).
   $$

   Define

   $$
   \delta=r-\lVert\mathbf{x}-\mathbf{a}\rVert.
   $$

   1. Prove that $$\delta>0$$.
   2. If $$\mathbf{y}\in B(\mathbf{x};\delta)$$, use the triangle inequality to prove that

      $$
      \mathbf{y}\in B(\mathbf{a};r).
      $$

   3. Deduce that

      $$
      B(\mathbf{x};\delta)\subseteq B(\mathbf{a};r).
      $$

   4. Conclude that every open ball is an open set.

7. **Unions of open sets.** Let $$\{U_i:i\in I\}$$ be an arbitrary family of open subsets of $$\mathbb{R}^n$$. Prove that

   $$
   \bigcup_{i\in I}U_i
   $$

   is open.

   Your proof should begin with an arbitrary point

   $$
   \mathbf{x}\in\bigcup_{i\in I}U_i
   $$

   and explain why there is at least one index $$i\in I$$ for which an open ball centered at $$\mathbf{x}$$ is contained in the union.

8. **Finite intersections of open sets.** Let $$U_1,\ldots,U_m$$ be open subsets of $$\mathbb{R}^n$$.

   1. Given

      $$
      \mathbf{x}\in\bigcap_{i=1}^m U_i,
      $$

      explain why for each $$i$$ there exists $$r_i>0$$ such that

      $$
      B(\mathbf{x};r_i)\subseteq U_i.
      $$

   2. Define

      $$
      r=\min\{r_1,\ldots,r_m\}.
      $$

      Prove that

      $$
      B(\mathbf{x};r)
      \subseteq
      \bigcap_{i=1}^m U_i.
      $$

   3. Conclude that every finite intersection of open sets is open.
   4. Explain exactly where the finiteness of the family is used.

9. **An infinite intersection of open sets.** For each $$n\in\mathbb{N}$$, define

   $$
   U_n=\left(-\frac1n,\frac1n\right).
   $$

   1. Prove that every $$U_n$$ is open.
   2. Prove that

      $$
      \bigcap_{n\in\mathbb{N}}U_n=\{0\}.
      $$

      Use the Archimedean property to show that every nonzero real number is excluded from at least one $$U_n$$.

   3. Prove that $$\{0\}$$ is not open.
   4. Conclude that an infinite intersection of open sets need not be open.

10. **Open half-spaces and open strips.** Fix a nonzero vector $$\mathbf{v}\in\mathbb{R}^n$$ and a real number $$c$$. Define

    $$
    H=\{\mathbf{x}\in\mathbb{R}^n:
    \mathbf{x}\cdot\mathbf{v}<c\}.
    $$

    1. Let $$\mathbf{a}\in H$$ and define

       $$
       r=
       \frac{c-\mathbf{a}\cdot\mathbf{v}}
       {\lVert\mathbf{v}\rVert}.
       $$

       Prove that $$r>0$$.

    2. If $$\mathbf{x}\in B(\mathbf{a};r)$$, use the Cauchy-Schwarz inequality to show that

       $$
       \mathbf{x}\cdot\mathbf{v}<c.
       $$

    3. Deduce that $$H$$ is open.
    4. Use this result and the fact that finite intersections of open sets are open to prove that

       $$
       \{\mathbf{x}\in\mathbb{R}^n:
       a<\mathbf{x}\cdot\mathbf{v}<b\}
       $$

       is open whenever $$a<b$$.



