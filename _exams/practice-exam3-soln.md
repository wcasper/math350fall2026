---
layout: page
title: Practice Exam 3 Solutions
permalink: /exams/practice-exam3-soln
---

## Problem 1 (True or False)

**a) TRUE.** A continuous image of a compact set is compact. Since $$[0,1]$$ is compact but $$(0,2]$$ is not compact, there can be no continuous surjection from $$[0,1]$$ onto $$(0,2]$$.

**b) TRUE.** The real line is connected, and the continuous image of a connected space is connected. The set $$(-\infty,-1]\cup[1,\infty)$$ is not connected, so no continuous surjection as stated exists.

**c) TRUE.** The Extreme Value Theorem guarantees that a continuous real-valued function on the compact interval $$[0,1]$$ attains its maximum (and minimum).

**d) FALSE.** For the constant continuous function $$f(x)=0$$, we have $$f((0,1))=\{0\}$$, which is not open in $$\mathbb R$$.

**e) TRUE.** Differentiability at a point implies continuity there (proved in Problem 2).

**f) FALSE.** For example, $$a_n=1/n\to0$$, but the harmonic series $$\sum_{n=1}^{\infty}1/n$$ diverges.

## Problem 2

**Claim:** If $$f$$ is differentiable at $$c$$, then $$f$$ is continuous at $$c$$.

**Proof.** Since $$f$$ is differentiable at $$c$$, the limit

$$
\lim_{x\to c}\frac{f(x)-f(c)}{x-c}=f'(c)
$$

exists and is finite. For $$x\neq c$$, we can write

$$
f(x)-f(c)=\frac{f(x)-f(c)}{x-c}(x-c).
$$

Taking limits as $$x\to c$$ and using the limit laws gives

$$
\lim_{x\to c}(f(x)-f(c))=f'(c)\cdot0=0.
$$

Therefore $$\lim_{x\to c}f(x)=f(c)$$, which is exactly continuity at $$c$$. $$\square$$

## Problem 3

**a) Definition of uniform continuity.** The function $$f:S\to T$$ is *uniformly continuous on* $$A\subseteq S$$ if for every $$\varepsilon>0$$ there exists $$\delta>0$$ such that **for every** $$x,y\in A$$,

$$
d_S(x,y)<\delta\quad\Longrightarrow\quad d_T(f(x),f(y))<\varepsilon.
$$

The same $$\delta$$ must work for every pair $$x,y$$ in $$A$$; it may depend on $$\varepsilon$$, but not on the particular points.

**b) Inequality.** We claim that for all $$x,y\geq0$$,

$$
\lvert\sqrt{x}-\sqrt{y}\rvert\leq\sqrt{\lvert x-y\rvert}.
$$

**Proof.** By symmetry, suppose $$x\geq y$$. Then $$\sqrt{x}\geq\sqrt{y}$$ and

$$
\begin{aligned}
(\sqrt{x}-\sqrt{y})^2
&=x+y-2\sqrt{xy}\\
&\leq x-y,
\end{aligned}
$$

because $$\sqrt{xy}\geq y$$ when $$x\geq y\geq0$$. Both sides are nonnegative, so taking square roots yields

$$
\sqrt{x}-\sqrt{y}\leq\sqrt{x-y}.
$$

This is the desired inequality. $$\square$$

**c) Uniform continuity of the square root.**

**Proof.** Let $$\varepsilon>0$$. Choose $$\delta=\varepsilon^2$$. If $$x,y\in[0,\infty)$$ and $$\lvert x-y\rvert<\delta$$, then by part (b),

$$
\lvert\sqrt{x}-\sqrt{y}\rvert
\leq\sqrt{\lvert x-y\rvert}
<\sqrt{\delta}=\varepsilon.
$$

Thus $$f(x)=\sqrt{x}$$ is uniformly continuous on $$[0,\infty)$$. $$\square$$

## Problem 4

**a) Rolle's Theorem.** Suppose $$a<b$$, $$f:[a,b]\to\mathbb R$$ is continuous on $$[a,b]$$, differentiable on $$(a,b)$$, and $$f(a)=f(b)$$. Then there exists $$c\in(a,b)$$ such that $$f'(c)=0$$.

**b) Proof of Rolle's Theorem.** By the Extreme Value Theorem, $$f$$ attains an absolute maximum $$M$$ and an absolute minimum $$m$$ on $$[a,b]$$.

If $$M=m$$, then $$f$$ is constant on $$[a,b]$$, so $$f'(c)=0$$ for every $$c\in(a,b)$$.

Otherwise $$M>m$$. Since $$f(a)=f(b)$$, at least one of the maximum or minimum values differs from the common endpoint value. That extremum must therefore be attained at some interior point $$c\in(a,b)$$. At $$c$$, the function has a local maximum or minimum. By the theorem that a differentiable function has derivative zero at an interior local extremum, $$f'(c)=0$$. $$\square$$

**c) Mean Value Theorem.** If $$a<b$$ and $$f:[a,b]\to\mathbb R$$ is continuous on $$[a,b]$$ and differentiable on $$(a,b)$$, then there exists $$c\in(a,b)$$ such that

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

**d) Proof of the Mean Value Theorem.** Define

$$
g(x)=f(x)-\frac{f(b)-f(a)}{b-a}(x-a).
$$

The function $$g$$ is continuous on $$[a,b]$$ and differentiable on $$(a,b)$$. Furthermore,

$$
g(a)=f(a),\qquad
 g(b)=f(b)-(f(b)-f(a))=f(a).
$$

Thus $$g(a)=g(b)$$. By Rolle's Theorem, there is a $$c\in(a,b)$$ such that $$g'(c)=0$$. Since

$$
g'(c)=f'(c)-\frac{f(b)-f(a)}{b-a},
$$

we obtain

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

This proves the Mean Value Theorem. $$\square$$

## Problem 5

**a) Definition of series convergence.** Let

$$
s_N=\sum_{n=1}^{N}a_n
$$

be the $$N$$th partial sum. We say $$\sum_{n=1}^{\infty}a_n$$ *converges to* $$s\in\mathbb R$$ if $$s_N\to s$$ as $$N\to\infty$$. In other words, for every $$\varepsilon>0$$ there exists an integer $$N_0$$ such that

$$
N\geq N_0\quad\Longrightarrow\quad\lvert s_N-s\rvert<\varepsilon.
$$

**b) Convergence implies the terms tend to zero.** If the series converges, then $$s_N\to s$$. For $$N\geq2$$,

$$
a_N=s_N-s_{N-1}.
$$

Both $$s_N$$ and $$s_{N-1}$$ converge to $$s$$, so by the limit laws,

$$
\lim_{N\to\infty}a_N=s-s=0.
$$

Hence $$a_N\to0$$. $$\square$$

**c) The converse is false.** Take $$a_n=1/n$$. We know $$1/n\to0$$, but the harmonic series diverges. One elementary proof groups terms:

$$
\begin{aligned}
1+\frac12
&+\left(\frac13+\frac14\right)
+\left(\frac15+\cdots+\frac18\right)
+\cdots.
\end{aligned}
$$

Each block after the first contains $$2^{k-1}$$ terms, each at least $$1/2^k$$, so each block has sum at least $$1/2$$. The partial sums are therefore unbounded and cannot converge.

**d) Telescoping sum.** The identity

$$
\frac1{n(n+1)}=\frac1n-\frac1{n+1}
$$

follows by putting the right-hand side over a common denominator. Consequently,

$$
\begin{aligned}
s_N&=\sum_{n=1}^{N}\left(\frac1n-\frac1{n+1}\right)\\
&=\left(1-\frac12\right)+\left(\frac12-\frac13\right)+\cdots+\left(\frac1N-\frac1{N+1}\right)\\
&=1-\frac1{N+1}.
\end{aligned}
$$

Since $$1/(N+1)\to0$$, we have $$s_N\to1$$. Therefore, by the definition of a convergent series,

$$
\boxed{\displaystyle\sum_{n=1}^{\infty}\frac1{n(n+1)}=1.}
$$

## Problem 6

**a) Definition of differentiability.** A function $$f:(a,b)\to\mathbb R$$ is *differentiable at* $$c\in(a,b)$$ if the finite limit

$$
f'(c)=\lim_{h\to0}\frac{f(c+h)-f(c)}{h}
$$

exists (where $$h\neq0$$ and $$c+h\in(a,b)$$).

**b) Product Rule.** If $$f$$ and $$g$$ are differentiable at $$c$$, then $$fg$$ is differentiable at $$c$$ and

$$
(fg)'(c)=f'(c)g(c)+f(c)g'(c).
$$

**c) Proof directly from the definition.** For $$h\neq0$$, add and subtract $$f(c+h)g(c)$$ in the numerator:

$$
\begin{aligned}
&\frac{f(c+h)g(c+h)-f(c)g(c)}{h}\\
&\qquad= f(c+h)\frac{g(c+h)-g(c)}{h}
+g(c)\frac{f(c+h)-f(c)}{h}.
\end{aligned}
$$

Because differentiability implies continuity (Problem 2), $$f(c+h)\to f(c)$$ as $$h\to0$$. By differentiability, the two difference quotients tend to $$g'(c)$$ and $$f'(c)$$, respectively. Taking the limit and applying the limit laws,

$$
\begin{aligned}
(fg)'(c)
&=f(c)g'(c)+g(c)f'(c).
\end{aligned}
$$

Thus the Product Rule follows directly from the definition. $$\square$$

**d) Quotient Rule.** If $$f$$ and $$g$$ are differentiable at $$c$$ and $$g(c)\neq0$$, then $$f/g$$ is differentiable at $$c$$ (on a neighborhood where the quotient is defined), and

$$
\boxed{\displaystyle
\left(\frac fg\right)'(c)
=\frac{g(c)f'(c)-f(c)g'(c)}{[g(c)]^2}.}
$$

## Problem 7

We give the definition in terms of **separations by relatively open sets**.

**a) Definition of connectedness.** A metric space $$X$$ is *connected* if it is impossible to write

$$
X=U\cup V,
$$

where $$U,V$$ are disjoint, nonempty sets that are both open in $$X$$. Equivalently, there is no separation of $$X$$ into two nonempty relatively open sets.

**b) Connected subsets of the integers.** Let $$A\subseteq\mathbb Z$$ contain at least two distinct integers. Choose $$k\in A$$ such that $$A$$ also contains an integer different from $$k$$. Since distinct integers are at least distance $$1$$ apart, the singleton $$\{k\}$$ is open in $$\mathbb Z$$ (it is the ball $$B_{1/2}(k)$$). Its complement $$\mathbb Z\setminus\{k\}$$ is also open in $$\mathbb Z$$: it is the union of the open balls $$B_{1/2}(j)$$ over $$j\neq k$$.

Therefore $$\{k\}$$ and $$A\setminus\{k\}$$ are disjoint, nonempty sets open in the subspace $$A$$ whose union is $$A$$. Thus $$A$$ is not connected.

Conversely, a singleton cannot be partitioned into two disjoint nonempty sets, so it is connected. Consequently, **the only nonempty connected subsets of $$\mathbb Z$$ are the singleton sets.** $$\square$$

**c) Continuous maps from connected spaces into $$\mathbb Z$$.** Suppose $$X$$ is connected and $$g:X\to\mathbb Z$$ is continuous. By the theorem that the continuous image of a connected space is connected, $$g(X)$$ is a connected subset of $$\mathbb Z$$. By (b), if $$X$$ is nonempty, $$g(X)$$ must be a singleton. Therefore $$g$$ is constant. (If $$X$$ is empty, the conclusion is vacuous.) $$\square$$

**d) Constant functions are continuous.** Suppose $$g(x)=k$$ for all $$x\in X$$, with fixed $$k\in\mathbb Z$$. Let $$\varepsilon>0$$ and choose $$\delta=1$$. For any $$x,y\in X$$ with $$d_X(x,y)<\delta$$,

$$
\lvert g(x)-g(y)\rvert=\lvert k-k\rvert=0<\varepsilon.
$$

Thus $$g$$ is continuous at every point (indeed, uniformly continuous). $$\square$$

**e) Conclusion.** A function $$g:\mathbb R\to\mathbb Z$$ is continuous **if and only if** it is constant.

Indeed, $$\mathbb R$$ is connected, so (c) shows that every continuous such function is constant. Conversely, (d) shows that every constant such function is continuous. $$\square$$

## Problem 8

We check the hypotheses of each test and distinguish absolute convergence from conditional convergence.

**a)** $$\displaystyle\sum_{n=1}^{\infty}\frac{n}{n+1}$$

**Diverges — nth-term test.** The terms satisfy

$$
\lim_{n\to\infty}\frac{n}{n+1}=1\neq0.
$$

A necessary condition for series convergence is that its terms tend to zero (Problem 5(b)). Hence this series diverges.

**b)** $$\displaystyle\sum_{n=1}^{\infty}\frac1{n^2+\sin^2 n}$$

**Converges absolutely — direct comparison test.** For every $$n\geq1$$, $$\sin^2n\geq0$$, so

$$
0\leq\frac1{n^2+\sin^2 n}\leq\frac1{n^2}.
$$

The $$p$$-series $$\sum 1/n^2$$ converges because $$p=2>1$$. All terms here are nonnegative, so the direct comparison test implies convergence, which is automatically absolute convergence.

**c)** $$\displaystyle\sum_{n=1}^{\infty}\frac{n}{n^2+1}$$

**Diverges — direct comparison test.** For every integer $$n\geq1$$, $$n^2+1\leq2n^2$$, hence

$$
\frac{n}{n^2+1}\geq\frac{n}{2n^2}=\frac1{2n}>0.
$$

The harmonic series $$\sum1/n$$ diverges, so $$\sum1/(2n)$$ diverges as well. Since each term of the given series is at least the corresponding term of this divergent nonnegative series, the direct comparison test implies divergence.

**d)** $$\displaystyle\sum_{n=1}^{\infty}\frac{n^2}{3^n}$$

**Converges absolutely — ratio test.** Set $$a_n=n^2/3^n>0$$. Then

$$
\begin{aligned}
\lim_{n\to\infty}\left\lvert\frac{a_{n+1}}{a_n}\right\rvert
&=\lim_{n\to\infty}\frac{(n+1)^2}{3n^2}\\
&=\frac13\lim_{n\to\infty}\left(1+\frac1n\right)^2
=\frac13<1.
\end{aligned}
$$

The ratio test guarantees absolute convergence.

**e)** $$\displaystyle\sum_{n=1}^{\infty}\left(\frac{2+(-1)^n}{4}\right)^n$$

**Converges absolutely — direct comparison with a geometric series.** For each integer $$n\geq1$$, we have $$(-1)^n\in\{-1,1\}$$, hence

$$
0<\frac{2+(-1)^n}{4}\leq\frac34<1.
$$

Raising these nonnegative quantities to the positive integer power $$n$$ gives

$$
0\leq\left(\frac{2+(-1)^n}{4}\right)^n\leq\left(\frac34\right)^n.
$$

The geometric series $$\sum_{n=1}^{\infty}(3/4)^n$$ converges because its ratio has absolute value less than $$1$$. The direct comparison test now gives absolute convergence. **Caution:** A direct application of the root test with a claimed limit would be incorrect: the $$n$$th roots alternate between $$1/4$$ and $$3/4$$ and do not have a limit.

**f)** $$\displaystyle\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}{\sqrt n}$$

**Converges conditionally — alternating series test, then $$p$$-series test.** Let $$b_n=1/\sqrt n$$. We have $$b_n>0$$, $$b_{n+1}\leq b_n$$ for all $$n\geq1$$, and $$b_n\to0$$. Thus the hypotheses of the alternating series test are satisfied, and the given series converges.

However, the series of absolute values is

$$
\sum_{n=1}^{\infty}\left\lvert\frac{(-1)^{n+1}}{\sqrt n}\right\rvert
=\sum_{n=1}^{\infty}\frac1{n^{1/2}},
$$

which is a divergent $$p$$-series because $$p=1/2\leq1$$. The original series is therefore **conditionally convergent**, not absolutely convergent.


