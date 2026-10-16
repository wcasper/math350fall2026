---
layout: page
title: Practice Exam 2
permalink: /exams/practice-exam2
---

Solve each of the following problems.
If a problem asks for a proof, be sure to carefully justify your work, including any theorems from class that you use.

**Note:** You may **not** use a theorem or result from class to prove something when doing so would make the problem entirely trivial. If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)

For each of the following, write **TRUE** if the statement is true and **FALSE** if the statement is false. No explanation is needed.

Assume that $$(s_n)$$ and $$(t_n)$$ are sequences of real numbers.

a) Every Cauchy sequence of real numbers is bounded.

b) The intersection of any family of open sets is open.

c) Every compact subset of $$\mathbb{R}$$ with the Euclidean metric is closed and bounded.

d) In a metric space with the discrete metric, every Cauchy sequence is eventually constant.

e) If $$(s_n)$$ has a convergent subsequence, then $$(s_n)$$ converges.

## Problem 2

a) Write down the definition of $$(x_n)$$ being a Cauchy sequence and the definition of $$(x_n)$$ converging to $$L$$ in a metric space $$(M,d)$$.

b) State the definition of an open cover of a set and the definition of a finite subcover.

c) Carefully state the Heine--Borel Theorem, the Bolzano--Weierstrass Theorem, the Cantor Intersection Theorem, and Lindelöf's Theorem.

## Problem 3

a) Write down the definition of a metric space.

b) Carefully prove that in a metric space $$(M,d)$$, the open ball

$$
B_M(x,r)=\{y\in M:d(x,y)< r\}
$$

is an open set.

## Problem 4

a) Write down the definition of a complete metric space.

b) Prove that the space $$[0,1)$$ with the Euclidean metric is not complete.

c) Let $$M$$ be any set equipped with the discrete metric. Prove that $$M$$ is complete.

## Problem 5

a) Let $$(S,d_S)$$ and $$(T,d_T)$$ be metric spaces, let $$A\subseteq S$$, and suppose that $$a\in S$$ is an accumulation point of $$A$$. If $$f:A\to T$$ is a function, write the definition of

$$
\lim_{x\to a}f(x)=L.
$$

b) Define $$f:\mathbb{R}^2\to\mathbb{R}$$ by

$$
f(x,y)=
\begin{cases}
(2x-y)\sin(1/x)\cos(1/y),&x\ne0\text{ and }y\ne0,\\
0,&x=0\text{ or }y=0.
\end{cases}
$$

Does the limit

$$
\lim_{(x,y)\to(0,0)}f(x,y)
$$

exist? Carefully explain.

## Problem 6

a) Write down the definition of a subset $$K\subseteq M$$ of a metric space $$(M,d)$$ being compact.

b) Let $$M=\mathbb{R}$$ with the Euclidean metric. Prove that the half-open interval $$(0,2]$$ is not compact directly from the definitions, without using the Heine--Borel Theorem.

Your proof must exhibit a specific open cover of $$(0,2]$$ that has no finite subcover.

## Problem 7

Let $$M=\mathbb{R}$$ with the Euclidean metric and consider the subspace

$$
S=\{0\}\cup\left\{\frac{1}{2^n}:n\in\mathbb{Z}_+\right\}.
$$

a) Show that if $$x\in S$$ is nonzero, then the singleton set $$\{x\}$$ is open in the subspace $$S$$.

b) Show that the singleton set $$\{0\}$$ is not open in $$S$$.

**Bonus practice:** Is $$S$$ a compact metric space? Why or why not?

## Problem 8

Suppose that $$(x_n)$$ is a monotone increasing sequence of real numbers that is bounded above.

a) Prove directly from the completeness axiom that $$(x_n)$$ converges. You may not use the Monotone Convergence Theorem.

b) Give an example showing that when the same underlying set $$\mathbb{R}$$ is equipped with the discrete metric, such a sequence need not converge.

