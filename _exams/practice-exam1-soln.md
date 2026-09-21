---
layout: page
title: Practice Exam 1 Solutions
permalink: /exams/practice-exam1-soln
---

Give complete explanations and proofs. You may use any theorem proved in class, but you must clearly state the theorem when you use it. Examples and counterexamples should be accompanied by a brief explanation showing that they have the required properties.

## 1. Vocabulary and definitions — 12 points

State each definition or axiom precisely.

1. **Completeness axiom.** (3 points)
2. **Interior point** and **open set** in $$\mathbb{R}^n$$. (3 points)
3. **Adherent point** and **accumulation point** of a set. Your definitions should make the distinction between them clear. (4 points)
4. **Algebraic numbers.** (2 points)

### Solution

1. **Completeness axiom.** Every nonempty subset $$A\subseteq\mathbb{R}$$ that is bounded above has a supremum in $$\mathbb{R}$$.

   In other words, if $$A\ne\varnothing$$ and there exists $$M\in\mathbb{R}$$ such that

   $$
   x\le M
   $$

   for every $$x\in A$$, then there exists a real number $$s$$ such that

   - $$x\le s$$ for every $$x\in A$$; and
   - if $$t<s$$, then $$t$$ is not an upper bound of $$A$$.

   The number $$s$$ is called the supremum of $$A$$ and is denoted by

   $$
   s=\sup(A).
   $$

2. Let $$A\subseteq\mathbb{R}^n$$ and let $$\mathbf{x}\in A$$. The point $$\mathbf{x}$$ is an **interior point** of $$A$$ if there exists $$r>0$$ such that

   $$
   B(\mathbf{x};r)\subseteq A.
   $$

   The set $$A$$ is **open** if every point of $$A$$ is an interior point of $$A$$.

3. Let $$A\subseteq\mathbb{R}^n$$.

   A point $$\mathbf{x}\in\mathbb{R}^n$$ is an **adherent point** of $$A$$ if, for every $$r>0$$,

   $$
   B(\mathbf{x};r)\cap A\ne\varnothing.
   $$

   A point $$\mathbf{x}\in\mathbb{R}^n$$ is an **accumulation point** of $$A$$ if, for every $$r>0$$,

   $$
   \big(B(\mathbf{x};r)-\{\mathbf{x}\}\big)\cap A
   \ne\varnothing.
   $$

   The difference is that the point of $$A$$ found in the ball must be different from $$\mathbf{x}$$ for an accumulation point. Thus every accumulation point is adherent, but an adherent point need not be an accumulation point.

4. A real or complex number $$\alpha$$ is called **algebraic** if it is a root of some nonzero polynomial with rational coefficients. That is, there exists a nonzero polynomial

   $$
   p(x)=a_0+a_1x+\cdots+a_nx^n,
   \qquad
   a_0,\ldots,a_n\in\mathbb{Q},
   $$

   such that

   $$
   p(\alpha)=0.
   $$

   Equivalently, $$\alpha$$ is algebraic if it is a root of a nonzero polynomial with integer coefficients.

## 2. Named theorems — 12 points

State each theorem precisely. No proof is required.

1. The **Archimedean property of the real numbers**. (3 points)
2. The **Cantor-Schröder-Bernstein theorem**. (3 points)
3. The **representation theorem for open subsets of** $$\mathbb{R}$$. (3 points)
4. The **density property of the rationals**. (3 points)

### Solution

1. **Archimedean property.** For every real number $$x$$, there exists $$n\in\mathbb{N}$$ such that

   $$
   n>x.
   $$

   Equivalently, if $$x,y\in\mathbb{R}$$ and $$x>0$$, then there exists $$n\in\mathbb{N}$$ such that

   $$
   nx>y.
   $$

2. **Cantor-Schröder-Bernstein theorem.** Let $$A$$ and $$B$$ be sets. If there is an injection

   $$
   f:A\to B
   $$

   and an injection

   $$
   g:B\to A,
   $$

   then there is a bijection between $$A$$ and $$B$$. Therefore,

   $$
   \lvert A\rvert=\lvert B\rvert.
   $$

3. **Representation theorem for open subsets of** $$\mathbb{R}$$. Every open subset of $$\mathbb{R}$$ can be expressed as a union of a countable family of pairwise disjoint open intervals.

   The intervals may be bounded or unbounded. The empty set corresponds to the empty union.

4. **Density property of the rationals.** If $$a,b\in\mathbb{R}$$ and $$a<b$$, then there exists $$q\in\mathbb{Q}$$ such that

   $$
   a<q<b.
   $$

   Thus every nonempty open interval contains a rational number.

## 3. Examples and counterexamples — 8 points

Give an example of each of the following. Briefly explain why your example works.

1. A subset of $$\mathbb{R}$$ that is both open and closed. (2 points)
2. A subset of $$\mathbb{R}$$ that is neither open nor closed. (2 points)
3. A set $$A\subseteq\mathbb{R}$$ and a point that is adherent to $$A$$ but is not an accumulation point of $$A$$. (2 points)
4. A countable subset of $$\mathbb{R}$$ whose closure is all of $$\mathbb{R}$$. (2 points)

### Solution

1. The set

   $$
   A=\mathbb{R}
   $$

   is both open and closed in $$\mathbb{R}$$. It is open because every ball centered at a real number lies in $$\mathbb{R}$$. It is closed because its complement is the empty set, which is open.

   The empty set is another example.

2. The set

   $$
   A=[0,1)
   $$

   is neither open nor closed.

   It is not open because $$0\in A$$, but every ball centered at $$0$$ contains negative numbers that are not in $$A$$. It is not closed because $$1$$ is an adherent point of $$A$$ but

   $$
   1\notin A.
   $$

3. Take

   $$
   A=\{0\}.
   $$

   The point $$0$$ is adherent to $$A$$ because every ball centered at $$0$$ contains $$0$$. However, it is not an accumulation point because no ball centered at $$0$$ contains a point of $$A$$ different from $$0$$.

4. Take

   $$
   A=\mathbb{Q}.
   $$

   The set $$\mathbb{Q}$$ is countable. By the density property of the rationals, every open ball in $$\mathbb{R}$$ contains a rational number. Therefore every real number is adherent to $$\mathbb{Q}$$, and hence

   $$
   \overline{\mathbb{Q}}=\mathbb{R}.
   $$

## 4. An ordered-field argument — 8 points

Suppose that

$$
0<a<b.
$$

Carefully use the field axioms and order axioms of the real numbers to prove that

$$
\frac1b<\frac1a.
$$

### Solution

We first show that

$$
a^{-1}>0
\qquad\text{and}\qquad
b^{-1}>0.
$$

Because $$a>0$$ and $$a\ne0$$, its multiplicative inverse exists. The number $$a^{-1}$$ cannot be zero because

$$
aa^{-1}=1\ne0.
$$

If $$a^{-1}<0$$, then multiplying this inequality by the positive number $$a$$ would give

$$
aa^{-1}<a\cdot0,
$$

so that

$$
1<0,
$$

which is impossible. Therefore,

$$
a^{-1}>0.
$$

The same argument shows that

$$
b^{-1}>0.
$$

Since the product of positive numbers is positive,

$$
a^{-1}b^{-1}>0.
$$

We are given that

$$
a<b.
$$

Multiplying both sides by the positive number $$a^{-1}b^{-1}$$ preserves the inequality:

$$
a(a^{-1}b^{-1})
<
b(a^{-1}b^{-1}).
$$

Using associativity and the inverse identities, we obtain

$$
(aa^{-1})b^{-1}
<
(bb^{-1})a^{-1}.
$$

Therefore,

$$
b^{-1}<a^{-1}.
$$

In fraction notation,

$$
\frac1b<\frac1a.
$$

## 5. A supremum problem — 12 points

Define

$$
A=
\left\{
\frac{3n-1}{n}:n\in\mathbb{N}
\right\}.
$$

1. Write down the definition of the supremum of a set $$A$$ in general.
2. Determine $$\sup(A)$$ and prove your answer from the definition of supremum. Your proof must use the Archimedean property.
3. Determine $$\inf(A)$$ and prove your answer.
4. Determine whether $$A$$ has a maximum and whether it has a minimum. Justify your answers.

### Solution

1. A number $$s\in\mathbb{R}$$ is the supremum of a set $$A\subseteq\mathbb{R}$$ if:

   - $$s$$ is an upper bound of $$A$$, meaning

     $$
     x\le s
     $$

     for every $$x\in A$$; and

   - $$s$$ is the least upper bound, meaning that if $$t<s$$, then $$t$$ is not an upper bound of $$A$$.

2. First observe that

   $$
   \frac{3n-1}{n}=3-\frac1n.
   $$

   Therefore,

   $$
   A=
   \left\{
   3-\frac1n:n\in\mathbb{N}
   \right\}.
   $$

   We claim that

   $$
   \sup(A)=3.
   $$

   For every $$n\in\mathbb{N}$$, we have $$1/n>0$$, so

   $$
   3-\frac1n<3.
   $$

   Thus $$3$$ is an upper bound of $$A$$.

   It remains to prove that no number smaller than $$3$$ is an upper bound. Let $$t<3$$ and set

   $$
   \varepsilon=3-t>0.
   $$

   By the Archimedean property, there exists $$n\in\mathbb{N}$$ such that

   $$
   n>\frac1\varepsilon.
   $$

   Since both sides are positive, taking reciprocals reverses the inequality:

   $$
   \frac1n<\varepsilon.
   $$

   It follows that

   $$
   3-\frac1n
   >
   3-\varepsilon
   =
   t.
   $$

   Therefore $$t$$ is not an upper bound of $$A$$. Hence $$3$$ is the least upper bound, and

   $$
   \sup(A)=3.
   $$

3. We claim that

   $$
   \inf(A)=2.
   $$

   Since $$n\ge1$$, we have

   $$
   \frac1n\le1.
   $$

   Consequently,

   $$
   3-\frac1n\ge2
   $$

   for every $$n\in\mathbb{N}$$. Thus $$2$$ is a lower bound of $$A$$.

   Moreover, when $$n=1$$,

   $$
   3-\frac11=2.
   $$

   Thus $$2\in A$$. Any lower bound of $$A$$ must be less than or equal to every element of $$A$$, and in particular it must be less than or equal to $$2$$. Therefore $$2$$ is the greatest lower bound:

   $$
   \inf(A)=2.
   $$

4. The set $$A$$ has a minimum because

   $$
   2\in A
   $$

   and every element of $$A$$ is at least $$2$$. Hence

   $$
   \min(A)=2.
   $$

   The set does not have a maximum. Indeed, for every $$n\in\mathbb{N}$$,

   $$
   3-\frac1{n+1}
   >
   3-\frac1n.
   $$

   Thus every element of $$A$$ is strictly smaller than another element of $$A$$. Also, the supremum $$3$$ is not an element of $$A$$. Therefore $$A$$ has no maximum.

## 6. Functions and cardinality — 12 points

1. Write down the definition of a function $$h:A\rightarrow B$$ being injective, surjective, and bijective.

2. Consider

   $$
   f:\mathbb{R}\to[0,\infty),
   \qquad
   f(x)=x^2.
   $$

   Determine whether $$f$$ is injective, surjective, or bijective. Prove your answers.

3. Now consider

   $$
   g:[0,\infty)\to[0,\infty),
   \qquad
   g(x)=x^2.
   $$

   Prove that $$g$$ is bijective and find $$g^{-1}$$.

4. Use the Cantor-Schröder-Bernstein theorem to prove that

   $$
   \mathbb{N}\times\mathbb{N}
   $$

   and $$\mathbb{N}$$ have the same cardinality.

   You may use the functions

   $$
   F(n)=(n,1)
   $$

   and

   $$
   G(m,n)=2^m3^n.
   $$

   Clearly identify the direction of each injection.

### Solution

1. A function $$h:A\to B$$ is **injective** if, for every $$x,y\in A$$,

   $$
   h(x)=h(y)
   \quad\Longrightarrow\quad
   x=y.
   $$

   It is **surjective** if, for every $$b\in B$$, there exists $$a\in A$$ such that

   $$
   h(a)=b.
   $$

   It is **bijective** if it is both injective and surjective.

2. The function

   $$
   f:\mathbb{R}\to[0,\infty),
   \qquad
   f(x)=x^2,
   $$

   is not injective. For example,

   $$
   f(1)=1=f(-1),
   $$

   but

   $$
   1\ne-1.
   $$

   The function is surjective. If $$y\in[0,\infty)$$, then the nonnegative square root $$\sqrt y$$ is a real number and

   $$
   f(\sqrt y)=(\sqrt y)^2=y.
   $$

   Thus every element of the codomain has a preimage.

   Since $$f$$ is surjective but not injective, it is not bijective.

3. Consider

   $$
   g:[0,\infty)\to[0,\infty),
   \qquad
   g(x)=x^2.
   $$

   To prove injectivity, suppose that

   $$
   g(x)=g(y).
   $$

   Then

   $$
   x^2=y^2,
   $$

   so

   $$
   (x-y)(x+y)=0.
   $$

   Since $$x,y\ge0$$, this implies $$x=y$$. Therefore $$g$$ is injective.

   To prove surjectivity, let $$z\in[0,\infty)$$. Taking

   $$
   x=\sqrt z
   $$

   gives $$x\in[0,\infty)$$ and

   $$
   g(x)=z.
   $$

   Therefore $$g$$ is surjective and hence bijective. Its inverse is

   $$
   g^{-1}(z)=\sqrt z.
   $$

4. Define

   $$
   F:\mathbb{N}\to\mathbb{N}\times\mathbb{N}
   $$

   by

   $$
   F(n)=(n,1).
   $$

   If $$F(n)=F(k)$$, then

   $$
   (n,1)=(k,1),
   $$

   so $$n=k$$. Therefore $$F$$ is injective.

   In the other direction, define

   $$
   G:\mathbb{N}\times\mathbb{N}\to\mathbb{N}
   $$

   by

   $$
   G(m,n)=2^m3^n.
   $$

   Suppose

   $$
   G(m,n)=G(j,k).
   $$

   Then

   $$
   2^m3^n=2^j3^k.
   $$

   By the fundamental theorem of arithmetic, prime factorizations are unique. Hence

   $$
   m=j
   \qquad\text{and}\qquad
   n=k.
   $$

   Thus $$G$$ is injective.

   We have constructed injections in both directions:

   $$
   \mathbb{N}\longrightarrow\mathbb{N}\times\mathbb{N}
   $$

   and

   $$
   \mathbb{N}\times\mathbb{N}\longrightarrow\mathbb{N}.
   $$

   By the Cantor-Schröder-Bernstein theorem, there exists a bijection between the two sets. Therefore,

   $$
   \lvert\mathbb{N}\times\mathbb{N}\rvert
   =
   \lvert\mathbb{N}\rvert.
   $$

## 7. Open balls are open — 14 points

Let $$\mathbf{a}\in\mathbb{R}^n$$ and let $$r>0$$. Prove that

$$
B(\mathbf{a};r)
=
\left\{
\mathbf{x}\in\mathbb{R}^n:
\lVert\mathbf{x}-\mathbf{a}\rVert<r
\right\}
$$

is an open set.

### Solution

Let

$$
\mathbf{x}\in B(\mathbf{a};r).
$$

By the definition of the open ball,

$$
\lVert\mathbf{x}-\mathbf{a}\rVert<r.
$$

Define

$$
\delta
=
r-\lVert\mathbf{x}-\mathbf{a}\rVert.
$$

Then $$\delta>0$$.

We claim that

$$
B(\mathbf{x};\delta)
\subseteq
B(\mathbf{a};r).
$$

Let

$$
\mathbf{y}\in B(\mathbf{x};\delta).
$$

Then

$$
\lVert\mathbf{y}-\mathbf{x}\rVert<\delta.
$$

By the triangle inequality,

$$
\begin{aligned}
\lVert\mathbf{y}-\mathbf{a}\rVert
&=
\lVert(\mathbf{y}-\mathbf{x})
     +(\mathbf{x}-\mathbf{a})\rVert\\
&\le
\lVert\mathbf{y}-\mathbf{x}\rVert
+
\lVert\mathbf{x}-\mathbf{a}\rVert\\
&<
\delta+\lVert\mathbf{x}-\mathbf{a}\rVert\\
&=
r.
\end{aligned}
$$

Therefore,

$$
\mathbf{y}\in B(\mathbf{a};r).
$$

This proves that

$$
B(\mathbf{x};\delta)
\subseteq
B(\mathbf{a};r).
$$

Thus every point of $$B(\mathbf{a};r)$$ is an interior point. Consequently, $$B(\mathbf{a};r)$$ is open.

## 8. Interior, closure, and accumulation points — 12 points

Let

$$
A=
(0,1)\cup\{2\}\cup
\left\{
3+\frac1n:n\in\mathbb{N}
\right\}.
$$

Determine each of the following and justify your answers:

1. Define the interior of a set and the closure of a set.
2. Determine the interior of $$A$$.
3. Determine the closure of $$A$$.
4. Decide whether $$A$$ is open and whether it is closed.

### Solution

1. The **interior** of a set $$A\subseteq\mathbb{R}^n$$ is the set

   $$
   A^\circ
   =
   \{
   \mathbf{x}\in A:
   \text{there exists }r>0
   \text{ such that }
   B(\mathbf{x};r)\subseteq A
   \}.
   $$

   The **closure** of $$A$$ is the set of all adherent points of $$A$$:

   $$
   \overline{A}
   =
   \{
   \mathbf{x}\in\mathbb{R}^n:
   B(\mathbf{x};r)\cap A\ne\varnothing
   \text{ for every }r>0
   \}.
   $$

2. We claim that

   $$
   A^\circ=(0,1).
   $$

   Every point $$x\in(0,1)$$ is an interior point. Indeed, if

   $$
   r=\frac12\min\{x,1-x\},
   $$

   then $$r>0$$ and

   $$
   B(x;r)\subseteq(0,1)\subseteq A.
   $$

   The point $$2$$ is not an interior point because every open interval centered at $$2$$ contains points other than $$2$$, and sufficiently small such intervals contain no other points of $$A$$.

   Similarly, each point

   $$
   3+\frac1n
   $$

   is isolated from the other listed points. Every open interval centered at it contains real numbers that are not elements of $$A$$. Therefore none of these points is an interior point.

   Consequently,

   $$
   A^\circ=(0,1).
   $$

3. We claim that

   $$
   \overline{A}
   =
   [0,1]\cup\{2\}
   \cup
   \left\{
   3+\frac1n:n\in\mathbb{N}
   \right\}
   \cup\{3\}.
   $$

   Every point of $$A$$ belongs to $$\overline{A}$$.

   The points $$0$$ and $$1$$ are adherent to $$(0,1)$$, since every open interval centered at either endpoint meets $$(0,1)$$.

   The point $$3$$ is adherent to $$A$$. Let $$r>0$$. By the Archimedean property, there exists $$n\in\mathbb{N}$$ such that

   $$
   n>\frac1r.
   $$

   Therefore,

   $$
   0<\frac1n<r,
   $$

   and hence

   $$
   3+\frac1n\in B(3;r)\cap A.
   $$

   Thus every ball centered at $$3$$ meets $$A$$.

   There are no other adherent points. Points outside $$[0,1]$$ can be separated from that interval unless they equal $$0$$ or $$1$$. The point $$2$$ is isolated. The sequence

   $$
   3+\frac1n
   $$

   has no adherent point other than its listed values and $$3$$: between consecutive terms there are open intervals containing no terms of the sequence, and points below $$3$$ or above $$4$$ can also be separated from it.

   Therefore,

   $$
   \overline{A}
   =
   [0,1]\cup\{2,3\}
   \cup
   \left\{
   3+\frac1n:n\in\mathbb{N}
   \right\}.
   $$

4. The set $$A$$ is not open because, for example, $$2\in A$$ but $$2$$ is not an interior point.

   The set $$A$$ is not closed because it does not contain all of its adherent points. In particular,

   $$
   0,1,3\in\overline{A},
   $$

   but

   $$
   0,1,3\notin A.
   $$

   Thus $$A$$ is neither open nor closed.

## 9. Intersections of closed sets — 10 points

Let $$\{C_i:i\in I\}$$ be an arbitrary family of closed subsets of $$\mathbb{R}^n$$. Prove that

$$
\bigcap_{i\in I}C_i
$$

is closed.

### Solution

Since each $$C_i$$ is closed, its complement

$$
\mathbb{R}^n-C_i
$$

is open.

By De Morgan’s law,

$$
\mathbb{R}^n-
\bigcap_{i\in I}C_i
=
\bigcup_{i\in I}
\left(\mathbb{R}^n-C_i\right).
$$

The right-hand side is an arbitrary union of open sets. By the open-union theorem, an arbitrary union of open sets is open. Therefore,

$$
\mathbb{R}^n-
\bigcap_{i\in I}C_i
$$

is open.

A set is closed precisely when its complement is open. Consequently,

$$
\bigcap_{i\in I}C_i
$$

is closed.

