---
layout: post
title: Homework 5
permalink: /homework/hw5
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

**Note:** All sets will be subsets of $$\mathbb R$$ unless otherwise stated. The metric on $\mathbb R^n$ will be Euclidean unless otherwise stated.



## Problems

1. **Algebra of continuous functions on a compact set.** Let $$(S,d)$$ be a metric space, let $$K\subseteq S$$ be a nonempty compact set, and let

   $$
   f,g:K\to\mathbb{R}
   $$

   be continuous. Define

   $$
   H(x)=\frac{f(x)^2+g(x)^2}{1+f(x)^2+g(x)^2}.
   $$

   1. Use the algebraic rules for continuous functions to prove that

      $$
      x\longmapsto f(x)^2+g(x)^2
      $$

      and

      $$
      x\longmapsto 1+f(x)^2+g(x)^2
      $$

      are continuous on $$K$$.

   2. Prove that the denominator in the definition of $$H$$ is never zero. Use the quotient theorem to conclude that $$H$$ is continuous on $$K$$.

   3. Prove that

      $$
      0\leq H(x)<1
      $$

      for every $$x\in K$$.

   4. Use the extreme value theorem to prove that $$H$$ attains both a minimum and a maximum on $$K$$.

   5. Suppose that $$f$$ and $$g$$ have no common zero on $$K$$. Prove that there exists $$m>0$$ such that

      $$
      H(x)\geq m
      $$

      for every $$x\in K$$.

   6. Explain why $$H(K)$$ is compact. Conclude that $$H(K)$$ is a closed and bounded subset of $$[0,1)$$.

   7. Show that compactness is essential in part 5 by taking

      $$
      K=(0,1),
      \qquad
      f(x)=x,
      \qquad
      g(x)=0.
      $$

      Verify that $$f$$ and $$g$$ have no common zero on $$K$$, but that no positive constant $$m$$ satisfies $$H(x)\geq m$$ for every $$x\in K$$.

2. **Continuous functions cannot change order without meeting.** Let $$S$$ be a connected metric space, and let

   $$
   f,g:S\to\mathbb{R}
   $$

   be continuous functions.

   1. Prove that the function

      $$
      h=f-g
      $$

      is continuous.

   2. Prove that the coincidence set

      $$
      E=\{x\in S:f(x)=g(x)\}
      $$

      is closed in $$S$$.

   3. Prove that the sets

      $$
      U=\{x\in S:f(x)<g(x)\}
      $$

      and

      $$
      V=\{x\in S:f(x)>g(x)\}
      $$

      are open in $$S$$.

   4. Suppose that $$f(x)\ne g(x)$$ for every $$x\in S$$. Prove that

      $$
      S=U\cup V
      $$

      and that $$U$$ and $$V$$ are disjoint.

   5. Use connectedness to prove that either

      $$
      f(x)<g(x)
      $$

      for every $$x\in S$$, or

      $$
      f(x)>g(x)
      $$

      for every $$x\in S$$.

   6. Let $$f,g:[a,b]\to\mathbb{R}$$ be continuous. Prove that if

      $$
      f(a)<g(a)
      \qquad\text{and}\qquad
      f(b)>g(b),
      $$

      then there exists $$c\in(a,b)$$ such that $$f(c)=g(c)$$.

3. **Disjoint compact sets are separated by a positive distance.** Let $$(S,d)$$ be a metric space, and let $$K,L\subseteq S$$ be nonempty, disjoint compact sets.

   1. Fix $$x\in S$$ and define

      $$
      \varphi_x:L\to\mathbb{R},
      \qquad
      \varphi_x(y)=d(x,y).
      $$

      Prove that $$\varphi_x$$ is continuous.

   2. Use the extreme value theorem to prove that there exists $$b_x\in L$$ such that

      $$
      d(x,b_x)=\min\{d(x,y):y\in L\}.
      $$

      Define

      $$
      D(x)=d(x,b_x).
      $$

   3. Prove that for every $$x,z\in S$$,

      $$
      D(x)\leq d(x,z)+D(z).
      $$

      *Hint:* Use the point $$b_z\in L$$ and the triangle inequality.

   4. Deduce that

      $$
      \lvert D(x)-D(z)\rvert\leq d(x,z).
      $$

      Conclude that $$D:S\to\mathbb{R}$$ is continuous.

   5. Apply the extreme value theorem to the restriction of $$D$$ to $$K$$ to prove that there exists $$a\in K$$ such that

      $$
      D(a)=\min\{D(x):x\in K\}.
      $$

   6. Prove that $$D(a)>0$$. Conclude that there exists $$\eta>0$$ such that

      $$
      d(x,y)\geq\eta
      $$

      for every $$x\in K$$ and $$y\in L$$.

   7. Give an example of two disjoint closed subsets of $$\mathbb{R}^2$$ whose distance from one another is $$0$$. Explain why this does not contradict the result above.

4. **Uniform continuity: three useful tests.**

   1. Let $$(M,d_M)$$ and $$(N,d_N)$$ be metric spaces, and suppose that $$f:M\to N$$ is uniformly continuous. Prove directly from the definitions that if $$(x_n)$$ is Cauchy in $$M$$, then $$(f(x_n))$$ is Cauchy in $$N$$.

   2. Use part 1 and the Cauchy sequence

      $$
      x_n=\frac1{n+1}
      $$

      to prove that

      $$
      f(x)=\frac1x
      $$

      is not uniformly continuous on $$(0,1)$$.

   3. Prove that for all $$x,y\geq0$$,

      $$
      \lvert\sqrt{x}-\sqrt{y}\rvert
      \leq \sqrt{\lvert x-y\rvert}.
      $$

      Use this inequality to prove directly that $$f(x)=\sqrt{x}$$ is uniformly continuous on $$[0,\infty)$$.

   4. Define

      $$
      x_n=\sqrt{2\pi n+\frac\pi2}
      \qquad\text{and}\qquad
      y_n=\sqrt{2\pi n+\frac{3\pi}2}.
      $$

      Prove that

      $$
      \lvert x_n-y_n\rvert\longrightarrow0.
      $$

   5. Compute

      $$
      \sin(x_n^2)
      \qquad\text{and}\qquad
      \sin(y_n^2),
      $$

      and use these values to prove that

      $$
      f(x)=\sin(x^2)
      $$

      is not uniformly continuous on $$\mathbb{R}$$.

   6. Explain why $$f(x)=\sin(x^2)$$ is nevertheless uniformly continuous on every closed bounded interval.

5. **A differentiable function built from an absolute value.** Define

   $$
   f(x)=x\lvert x\rvert.
   $$

   1. Prove that

      $$
      f(x)=
      \begin{cases}
      x^2,&x\geq0,\\
      -x^2,&x<0.
      \end{cases}
      $$

   2. Show that

      $$
      f(x)-f(0)=x\lvert x\rvert.
      $$

      Use the chord-slope function

      $$
      f^*(x)=\lvert x\rvert
      $$

      to prove that $$f$$ is differentiable at $$0$$.

   3. Compute $$f'(0)$$.

   4. Use the piecewise formula from part 1 and the usual differentiation rules to compute $$f'(x)$$ for $$x\ne0$$.

   5. Prove that

      $$
      f'(x)=2\lvert x\rvert
      $$

      for every $$x\in\mathbb{R}$$.

   6. Prove directly from the definition that

      $$
      g(x)=\lvert x\rvert
      $$

      is not differentiable at $$0$$.

   7. Explain how these examples illustrate both of the following facts:

      - differentiability implies continuity;
      - continuity does not imply differentiability.

6. **The chain rule and an application.** Let $$f$$ be differentiable at $$c$$, let $$g$$ be differentiable at $$f(c)$$, and define

   $$
   h=g\circ f.
   $$

   1. Use the chord-function theorem to choose functions $$f^*$$ and $$g^*$$ such that

      $$
      f(x)-f(c)=(x-c)f^*(x)
      $$

      and

      $$
      g(u)-g(f(c))=(u-f(c))g^*(u),
      $$

      where $$f^*$$ is continuous at $$c$$ and $$g^*$$ is continuous at $$f(c)$$.

   2. Substitute $$u=f(x)$$ and prove that

      $$
      h(x)-h(c)
      =(x-c)f^*(x)g^*(f(x)).
      $$

   3. Explain why

      $$
      x\longmapsto f^*(x)g^*(f(x))
      $$

      is continuous at $$c$$.

   4. Use the chord-function theorem to prove the chain rule

      $$
      h'(c)=g'(f(c))f'(c).
      $$

   5. Use the product rule and induction to prove the power rule

      $$
      \frac{d}{dx}x^n=nx^{n-1}
      $$

      for every positive integer $$n$$.

   6. Let

      $$
      H(x)=\frac{(1+x^2)^5}{2+x^3}.
      $$

      State the domain of $$H$$ and explain why $$H$$ is differentiable on its domain.

   7. Use the power, chain, and quotient rules to compute $$H'(x)$$. Factor your final numerator as much as reasonably possible.


