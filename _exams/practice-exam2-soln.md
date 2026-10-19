---
layout: page
title: Practice Exam 2 Solutions
permalink: /exams/practice-exam2-soln
---

## Problem 1 (True or False)

a) **TRUE.**

Every Cauchy sequence is bounded. Indeed, the Cauchy condition places some tail of the sequence inside a ball of radius $$1$$ around one fixed term. The finitely many earlier terms can then be included in a larger ball.

b) **FALSE.**

For example, every set in the family

$$
U_n=\left(-\frac1n,\frac1n\right),
\qquad n\in\mathbb{Z}_+,
$$

is open in $$\mathbb{R}$$, but

$$
\bigcap_{n=1}^{\infty}U_n=\{0\},
$$

which is not open in $$\mathbb{R}$$.

c) **TRUE**, provided that “closed” and “bounded” refer to the given metric.

Every compact subset of a metric space is closed and bounded. This result does not require the metric to be the Euclidean metric. The converse, however, is special: a closed and bounded set need not be compact in an arbitrary metric space.

d) **TRUE.**

If $$(x_n)$$ is Cauchy in the discrete metric, use $$\varepsilon=1/2$$. There is some $$N$$ such that

$$
d(x_m,x_n)<\frac12
$$

whenever $$m,n\geq N$$. Since the discrete metric takes only the values $$0$$ and $$1$$, this forces

$$
d(x_m,x_n)=0,
$$

and hence $$x_m=x_n$$, whenever $$m,n\geq N$$. Thus the sequence is eventually constant.

e) **FALSE.**

For example, the sequence

$$
s_n=(-1)^n
$$

has the convergent subsequence $$s_{2n}=1$$, but the original sequence does not converge.

## Problem 2

### Part a

A sequence $$(x_n)$$ in a metric space $$(M,d)$$ is **Cauchy** if, for every $$\varepsilon>0$$, there exists $$N\in\mathbb{Z}_+$$ such that

$$
d(x_m,x_n)<\varepsilon
$$

whenever $$m,n\geq N$$.

The sequence $$(x_n)$$ **converges to** $$L\in M$$ if, for every $$\varepsilon>0$$, there exists $$N\in\mathbb{Z}_+$$ such that

$$
d(x_n,L)<\varepsilon
$$

whenever $$n\geq N$$.

The key distinction is that the Cauchy condition compares late terms with one another, whereas convergence compares late terms with a specified point $$L$$ in the space.

### Part b

Let $$A$$ be a subset of a metric space $$M$$. An **open cover** of $$A$$ is a family

$$
\mathcal{U}=\{U_\alpha:\alpha\in I\}
$$

of open subsets of $$M$$ such that

$$
A\subseteq\bigcup_{\alpha\in I}U_\alpha.
$$

A **finite subcover** is a finite subcollection

$$
U_{\alpha_1},\ldots,U_{\alpha_N}
$$

from the original cover that still covers $$A$$:

$$
A\subseteq U_{\alpha_1}\cup\cdots\cup U_{\alpha_N}.
$$

### Part c

**Heine--Borel Theorem.** A subset of $$\mathbb{R}^m$$ with the Euclidean metric is compact if and only if it is closed and bounded.

**Bolzano--Weierstrass Theorem.** Every bounded sequence in $$\mathbb{R}^m$$ has a convergent subsequence.

Equivalently, every infinite bounded subset of $$\mathbb{R}^m$$ has an accumulation point.

**Cantor Intersection Theorem.** Let $$(M,d)$$ be a complete metric space, and suppose that

$$
F_1\supseteq F_2\supseteq F_3\supseteq\cdots
$$

is a nested sequence of nonempty closed subsets of $$M$$ satisfying

$$
\operatorname{diam}(F_n)\longrightarrow0.
$$

Then there is exactly one point in

$$
\bigcap_{n=1}^{\infty}F_n.
$$

**Lindelöf's Theorem.** Every open cover of a subset of $$\mathbb{R}^m$$ has a countable subcover. More generally, every open cover of a separable metric space has a countable subcover.

## Problem 3

### Part a

A **metric space** is a pair $$(M,d)$$ consisting of a set $$M$$ and a function

$$
d:M\times M\longrightarrow\mathbb{R}
$$

such that, for all $$x,y,z\in M$$:

1. $$d(x,y)\geq0$$.
2. $$d(x,y)=0$$ if and only if $$x=y$$.
3. $$d(x,y)=d(y,x)$$.
4. $$d(x,z)\leq d(x,y)+d(y,z)$$.

The function $$d$$ is called a metric on $$M$$.

### Part b

Let $$y\in B_M(x,r)$$. Then

$$
d(x,y)<r.
$$

Define

$$
\rho=r-d(x,y).
$$

Since $$d(x,y)<r$$, we have $$\rho>0$$. We claim that

$$
B_M(y,\rho)\subseteq B_M(x,r).
$$

Let $$z\in B_M(y,\rho)$$. By the triangle inequality,

$$
d(x,z)\leq d(x,y)+d(y,z)
<d(x,y)+\rho
=r.
$$

Therefore $$z\in B_M(x,r)$$. Thus every point $$y\in B_M(x,r)$$ has an open ball centered at $$y$$ contained in $$B_M(x,r)$$. Consequently, $$B_M(x,r)$$ is open.

## Problem 4

### Part a

A metric space $$(M,d)$$ is **complete** if every Cauchy sequence in $$M$$ converges to a point of $$M$$.

### Part b

Consider the sequence in $$S=[0,1)$$ defined by

$$
x_n=1-\frac1n.
$$

We first show directly that $$(x_n)$$ is Cauchy. Let $$\varepsilon>0$$, and choose $$N$$ so large that

$$
\frac{2}{N}<\varepsilon.
$$

If $$m,n\geq N$$, then

$$
\begin{aligned}
\lvert x_m-x_n\rvert
&=\left\lvert\frac1n-\frac1m\right\rvert\\
&\leq\frac1n+\frac1m\\
&\leq\frac{2}{N}\\
&<\varepsilon.
\end{aligned}
$$

Thus $$(x_n)$$ is Cauchy in $$S$$.

In $$\mathbb{R}$$, the sequence converges to $$1$$. It cannot converge to any other point because limits in a metric space are unique. But $$1\notin S$$. Therefore $$(x_n)$$ does not converge to any point of $$S$$, so $$S$$ is not complete.

### Part c

Let $$(x_n)$$ be a Cauchy sequence in a set $$M$$ equipped with the discrete metric. Apply the Cauchy condition with $$\varepsilon=1/2$$. There exists $$N$$ such that

$$
d(x_m,x_n)<\frac12
$$

whenever $$m,n\geq N$$. The only value of the discrete metric smaller than $$1/2$$ is $$0$$, so

$$
x_m=x_n
$$

whenever $$m,n\geq N$$.

Thus $$(x_n)$$ is eventually constant. In particular,

$$
x_n\longrightarrow x_N.
$$

Therefore every Cauchy sequence in $$M$$ converges in $$M$$, and $$M$$ is complete.

## Problem 5

### Part a

The statement

$$
\lim_{x\to a}f(x)=L
$$

means that, for every $$\varepsilon>0$$, there exists $$\delta>0$$ such that, for every $$x\in A$$,

$$
0<d_S(x,a)<\delta
$$

implies

$$
d_T(f(x),L)<\varepsilon.
$$

The condition $$0<d_S(x,a)$$ excludes the point $$a$$ itself. Thus the value of $$f(a)$$, when it is defined, has no effect on the limit.

### Part b

We claim that

$$
\lim_{(x,y)\to(0,0)}f(x,y)=0.
$$

If $$x\ne0$$ and $$y\ne0$$, then

$$
\begin{aligned}
\lvert f(x,y)\rvert
&=\lvert2x-y\rvert\,
  \lvert\sin(1/x)\rvert\,
  \lvert\cos(1/y)\rvert\\
&\leq\lvert2x-y\rvert\\
&\leq2\lvert x\rvert+\lvert y\rvert.
\end{aligned}
$$

Since

$$
\lvert x\rvert\leq\sqrt{x^2+y^2}
\qquad\text{and}\qquad
\lvert y\rvert\leq\sqrt{x^2+y^2},
$$

we obtain

$$
\lvert f(x,y)\rvert
\leq3\sqrt{x^2+y^2}.
$$

The same inequality holds when $$x=0$$ or $$y=0$$ because then $$f(x,y)=0$$.

Let $$\varepsilon>0$$ and choose

$$
\delta=\frac{\varepsilon}{3}.
$$

If

$$
0<\sqrt{x^2+y^2}<\delta,
$$

then

$$
\lvert f(x,y)-0\rvert
\leq3\sqrt{x^2+y^2}
<3\delta
=\varepsilon.
$$

Therefore the limit exists and equals $$0$$.

## Problem 6

### Part a

A subset $$K$$ of a metric space $$M$$ is **compact** if every open cover of $$K$$ has a finite subcover.

Explicitly, if $$\{U_\alpha:\alpha\in I\}$$ is any family of open subsets of $$M$$ satisfying

$$
K\subseteq\bigcup_{\alpha\in I}U_\alpha,
$$

then there must be finitely many indices

$$
\alpha_1,\ldots,\alpha_N
$$

such that

$$
K\subseteq U_{\alpha_1}\cup\cdots\cup U_{\alpha_N}.
$$

### Part b

For each $$n\in\mathbb{Z}_+$$, define

$$
U_n=\left(\frac1n,3\right).
$$

Every $$U_n$$ is open in $$\mathbb{R}$$. We claim that

$$
\mathcal{U}=\{U_n:n\in\mathbb{Z}_+\}
$$

is an open cover of $$(0,2]$$.

Let $$x\in(0,2]$$. Since $$x>0$$, the Archimedean property gives an integer $$n$$ such that

$$
n>\frac1x.
$$

It follows that $$1/n<x<3$$, so $$x\in U_n$$. Hence the family covers $$(0,2]$$.

Now choose any finite subcollection

$$
U_{n_1},\ldots,U_{n_k},
$$

and let

$$
N=\max\{n_1,\ldots,n_k\}.
$$

Because the sets are nested,

$$
U_{n_1}\cup\cdots\cup U_{n_k}=U_N
=\left(\frac1N,3\right).
$$

But the point

$$
\frac1{N+1}
$$

belongs to $$(0,2]$$ and does not belong to $$U_N$$. Thus no finite subcollection covers $$(0,2]$$.

Therefore $$(0,2]$$ is not compact.

## Problem 7

Write

$$
x_n=\frac1{2^n}.
$$

### Part a

Fix a nonzero point $$x_n\in S$$. Choose

$$
r=\frac1{2^{n+2}}.
$$

The closest smaller point of the sequence is $$x_{n+1}$$, and

$$
x_n-x_{n+1}
=\frac1{2^n}-\frac1{2^{n+1}}
=\frac1{2^{n+1}}
>r.
$$

Every other point of $$S$$ is at least this far from $$x_n$$. Therefore

$$
B_{\mathbb{R}}(x_n,r)\cap S=\{x_n\}.
$$

Equivalently,

$$
B_S(x_n,r)=\{x_n\}.
$$

Thus $$\{x_n\}$$ is open in the subspace $$S$$.

### Part b

Suppose that $$\{0\}$$ were open in $$S$$. Then there would exist some $$r>0$$ such that

$$
B_S(0,r)\subseteq\{0\}.
$$

However,

$$
\frac1{2^n}\longrightarrow0.
$$

Consequently, there exists $$n$$ large enough that

$$
0<\frac1{2^n}<r.
$$

Then $$1/2^n$$ is a nonzero point of $$B_S(0,r)$$, which is a contradiction. Therefore $$\{0\}$$ is not open in $$S$$.

### Bonus practice

Yes, $$S$$ is compact.

Let $$\mathcal{U}$$ be an open cover of $$S$$. Choose some $$U_0\in\mathcal{U}$$ containing $$0$$. Since $$U_0$$ is open in the subspace $$S$$, there is some $$r>0$$ such that

$$
B_S(0,r)\subseteq U_0.
$$

Choose $$N$$ so large that

$$
\frac1{2^N}<r.
$$

Then $$U_0$$ contains $$0$$ and every point $$1/2^n$$ with $$n\geq N$$. Only the finitely many points

$$
\frac12,\frac1{2^2},\ldots,\frac1{2^{N-1}}
$$

remain. For each of these points, choose one member of $$\mathcal{U}$$ containing it. Together with $$U_0$$, these finitely many sets form a finite subcover of $$S$$. Hence $$S$$ is compact.

## Problem 8

### Part a

Let

$$
A=\{x_n:n\in\mathbb{Z}_+\}.
$$

The set $$A$$ is nonempty and bounded above. By the completeness axiom, it has a supremum. Let

$$
L=\sup A.
$$

We prove that $$x_n\to L$$. Let $$\varepsilon>0$$. Since $$L-\varepsilon<L$$ and $$L$$ is the least upper bound of $$A$$, the number $$L-\varepsilon$$ cannot be an upper bound of $$A$$. Therefore there is some $$N$$ such that

$$
x_N>L-\varepsilon.
$$

Because the sequence is increasing, whenever $$n\geq N$$ we have

$$
x_n\geq x_N>L-\varepsilon.
$$

Since $$L$$ is an upper bound of $$A$$, we also have

$$
x_n\leq L.
$$

Thus, for every $$n\geq N$$,

$$
L-\varepsilon<x_n\leq L,
$$

and hence

$$
\lvert x_n-L\rvert<\varepsilon.
$$

Therefore

$$
x_n\longrightarrow L.
$$

### Part b

Consider

$$
x_n=1-\frac1n.
$$

In the usual order on $$\mathbb{R}$$, this sequence is increasing and bounded above by $$1$$. It is not eventually constant.

Now equip $$\mathbb{R}$$ with the discrete metric. If $$(x_n)$$ converged to some $$L$$ in this metric, then using $$\varepsilon=1/2$$ would give an $$N$$ such that

$$
d(x_n,L)<\frac12
$$

whenever $$n\geq N$$. The discrete metric then forces

$$
x_n=L
$$

for every $$n\geq N$$. This would make the sequence eventually constant, which it is not.

Therefore $$(x_n)$$ does not converge in the discrete metric.

