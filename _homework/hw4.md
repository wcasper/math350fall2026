---
layout: post
title: Homework 4
permalink: /homework/hw4
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

**Note:** The metric we take on $$\mathbb R$$ or $$\mathbb R^n$$ will **always** be the Euclidean metric, unless otherwise stated in the problem.


## Problems

1. **The usual limit laws.** Let $$(a_n)$$ and $$(b_n)$$ be sequences of real numbers satisfying

   $$
   a_n\longrightarrow a
   \qquad\text{and}\qquad
   b_n\longrightarrow b.
   $$

   Prove each of the following directly from the definition of convergence. Each $$\varepsilon$$--$$N$$ proof should begin by letting $$\varepsilon>0$$.

   1. For every $$c\in\mathbb{R}$$,

      $$
      ca_n\longrightarrow ca.
      $$

   2. The sum and difference laws:

      $$
      a_n+b_n\longrightarrow a+b
      \qquad\text{and}\qquad
      a_n-b_n\longrightarrow a-b.
      $$

   3. Prove first that there exist $$M>0$$ and $$N_0\in\mathbb{N}$$ such that

      $$
      \lvert a_n\rvert\leq M
      $$

      whenever $$n\geq N_0$$. Use this to prove the product law

      $$
      a_nb_n\longrightarrow ab.
      $$

   4. Suppose that $$b\ne0$$. Prove that there exists $$N_0\in\mathbb{N}$$ such that

      $$
      \lvert b_n\rvert\geq\frac{\lvert b\rvert}{2}>0
      $$

      whenever $$n\geq N_0$$. Then prove

      $$
      \frac1{b_n}\longrightarrow\frac1b.
      $$

   5. Deduce the quotient law: if $$b\ne0$$, then

      $$
      \frac{a_n}{b_n}\longrightarrow\frac ab.
      $$

   6. Use the reverse triangle inequality to prove

      $$
      \lvert a_n\rvert\longrightarrow\lvert a\rvert.
      $$

   7. Prove that for every positive integer $$k$$,

      $$
      a_n^k\longrightarrow a^k.
      $$

   8. Prove the squeeze theorem for sequences: if

      $$
      a_n\leq c_n\leq b_n
      $$

      for all sufficiently large $$n$$ and

      $$
      a_n\longrightarrow L,
      \qquad
      b_n\longrightarrow L,
      $$

      then $$c_n\to L$$.

2. **A unique subsequential limit.** Let $$(x_n)$$ be a bounded sequence in $$\mathbb{R}^m$$, and suppose that there is a point $$L\in\mathbb{R}^m$$ with the following property:

   > Every convergent subsequence of $$(x_n)$$ converges to $$L$$.

   1. Suppose, toward a contradiction, that $$x_n$$ does not converge to $$L$$. Prove that there are some $$\varepsilon_0>0$$ and a subsequence $$(x_{n_k})$$ such that

      $$
      \lVert x_{n_k}-L\rVert\geq\varepsilon_0
      $$

      for every $$k$$.

   2. Use the Bolzano--Weierstrass theorem to find a convergent subsequence of $$(x_{n_k})$$.
   3. Show that the limit of this new subsequence cannot be $$L$$, and obtain a contradiction.
   4. Conclude that $$x_n\to L$$.
   5. Show that boundedness cannot be omitted by giving an unbounded sequence with no convergent subsequences.

3. **Newton's method as a monotone sequence.** Define

   $$
   x_1=2,
   \qquad
   x_{n+1}=\frac12\left(x_n+\frac3{x_n}\right).
   $$

   1. Prove by induction that $$x_n>0$$ for every $$n$$.
   2. Verify the identity

      $$
      x_{n+1}-\sqrt3
      =\frac{(x_n-\sqrt3)^2}{2x_n}.
      $$

      Deduce that

      $$
      x_n\geq\sqrt3
      $$

      for every $$n$$.

   3. Prove that $$(x_n)$$ is decreasing.
   4. Use the monotone convergence theorem to prove that $$(x_n)$$ converges.
   5. Use the limit laws from Problem 1 to determine its limit.
   6. If $$e_n=x_n-\sqrt3$$, prove that

      $$
      0\leq e_{n+1}\leq\frac{e_n^2}{2\sqrt3}.
      $$

      Explain what this estimate says about the speed of convergence.

4. **Completing the open interval.** Let

   $$
   M=(0,1)
   $$

   with the usual metric. Recall that two Cauchy sequences $$(x_n)$$ and $$(y_n)$$ in $$M$$ represent the same point in the completion when

   $$
   \lvert x_n-y_n\rvert\longrightarrow0.
   $$

   1. Prove that

      $$
      a_n=\frac1{n+1}
      \qquad\text{and}\qquad
      b_n=1-\frac1{n+1}
      $$

      are Cauchy sequences in $$M$$ but do not converge in $$M$$.

   2. Show that $$(a_n)$$ and $$(b_n)$$ represent two different points in the completion.
   3. Let $$(x_n)$$ be any Cauchy sequence in $$M$$. Explain why it converges, as a sequence in $$\mathbb{R}$$, to some point of $$[0,1]$$.
   4. Prove that two Cauchy sequences in $$M$$ are equivalent if and only if they have the same limit in $$\mathbb{R}$$.
   5. Explain why the completion of $$(0,1)$$ can be identified with $$[0,1]$$.

5. **Complete subspaces.** Let $$(M,d)$$ be a complete metric space and let $$S\subseteq M$$ have the relative metric.

   1. Suppose that $$S$$ is closed in $$M$$. Prove that every Cauchy sequence in $$S$$ converges to a point of $$S$$.
   2. Suppose instead that $$S$$ is complete. If $$x$$ is an adherent point of $$S$$, choose $$x_n\in S$$ satisfying

      $$
      d(x_n,x)<\frac1n.
      $$

      Prove that $$(x_n)$$ is Cauchy and use completeness of $$S$$ to show that $$x\in S$$.

   3. Conclude that, inside a complete metric space,

      $$
      S\text{ is complete}
      \quad\Longleftrightarrow\quad
      S\text{ is closed}.
      $$

   4. Use this result to determine which of the following subspaces of $$\mathbb{R}$$ are complete:

      $$
      [0,\infty),
      \qquad
      (0,\infty),
      \qquad
      \mathbb{Z},
      \qquad
      \left\{\frac1n:n\in\mathbb{N}\right\},
      \qquad
      \{0\}\cup\left\{\frac1n:n\in\mathbb{N}\right\}.
      $$

      For every incomplete space, give an explicit Cauchy sequence that does not converge in that space.

6.  **Convergent distances.** Let $$(M,d)$$ be a metric space and suppose that $$\{x_n\}$$ converges to $$x$$ and $$\{y_n\}$$ converges to $$y$$.  Consider the sequence of distances $$d_n = d(x_n,y_n)$$ in $$\mathbb R$$.  Prove that

$$\lim_{n\rightarrow\infty} d_n\rightarrow d(x,y).$$




