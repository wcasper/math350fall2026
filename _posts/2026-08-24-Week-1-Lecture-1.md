---
layout: post
title:  Lecture 1
---

## Properies of real numbers

### Key words
integers, rational numbers, real numbers, irrational numbers, algebraic numbers, transcendental numbers, field axioms, order axioms

### Reading assignment
Apostol pp. 1.1-1.15

### Slides

* [Link to slides](http://wcasper.github.io/math350fall2026/slides/lec01/lec01.pdf)

## Practice problems

1. **Finding polynomial equations.** For each number below, find a nonzero polynomial with rational coefficients having that number as a root.

   1. $$\sqrt{2}+\sqrt{3}$$
   2. $$\sqrt{2}-\sqrt{3}$$
   3. $$\frac{1}{1+\sqrt{2}}$$
   4. $$\sqrt{1+\sqrt{2}}$$

   You do not need to prove that your polynomial has the smallest possible degree.

2. **Relations among number classes.** Determine whether each statement is true or false. Prove the true statements and give counterexamples to the false ones.

   1. The sum of two irrational numbers is irrational.
   2. The product of two irrational numbers is irrational.
   3. The sum of a rational number and an irrational number is irrational.
   4. The product of a nonzero rational number and an irrational number is irrational.
   5. The square of an irrational number is irrational.

3. **A new operation.** Define an operation $$\star$$ on $$\mathbb{R}$$ by

   $$
   x\star y=x+y+1.
   $$

   1. Show that $$\star$$ is associative and commutative.
   2. Find the identity element for $$\star$$.
   3. Find the $$\star$$-inverse of an arbitrary element $$x$$.
   4. Explain why the identity and inverses for $$\star$$ differ from those for ordinary addition.

4. **A proposed field.** On $$\mathbb{R}$$, keep ordinary addition but define a new multiplication by

   $$
   x\odot y=2xy.
   $$

   1. Determine the multiplicative identity for $$\odot$$.
   2. Find the multiplicative inverse of a nonzero element $$x$$ with respect to $$\odot$$.
   3. Verify that $$\odot$$ distributes over ordinary addition.
   4. Decide whether these operations make $$\mathbb{R}$$ into a field.

5. **Cancellation without subtraction.** Suppose

   $$
   ax+b=ay+b.
   $$

   Prove that if $$a\neq 0$$, then $$x=y$$. Write the proof as a sequence of equations and identify the field property used at each stage.

6. **Finite fields cannot be ordered.** Suppose a field $$K$$ contains an element $$1$$ such that

   $$
   \underbrace{1+1+\cdots+1}_{n\text{ terms}}=0
   $$

   for some positive integer $$n$$.

   Prove that $$K$$ cannot be made into an ordered field.

   *Hint:* First prove inductively that every finite sum of copies of $$1$$ is positive.

7. **Solving inequalities axiomatically.** Let $$a,b,c\in F$$ with $$a>0$$. Prove that

   $$
   ax+b<c
   $$

   holds if and only if

   $$
   x<\frac{c-b}{a}.
   $$

   Then explain exactly what changes when $$a<0$$.

8. **Absolute value.** Define

   $$
   \lvert x\rvert=
   \begin{cases}
   x,&x\ge 0,\\
   -x,&x<0.
   \end{cases}
   $$

   Prove each statement using the order axioms.

   1. $$\lvert x\rvert\ge 0$$.
   2. $$\lvert x\rvert=0$$ if and only if $$x=0$$.
   3. $$\lvert -x\rvert=\lvert x\rvert$$.
   4. $$\lvert xy\rvert=\lvert x\rvert\lvert y\rvert$$.

9. **An elementary inequality.** Use the fact that squares are nonnegative to prove that

   $$
   2xy\le x^2+y^2
   $$

   for all $$x,y\in F$$.

   Determine exactly when equality holds.

10. **An epsilon application.** Suppose $$a,b\in F$$ and

    $$
    \lvert a-b\rvert<\varepsilon
    $$

    for every $$\varepsilon>0$$.

    Prove that $$a=b$$.

    Your proof should not merely quote Apostol's Theorem 1.1. Instead, assume $$a\neq b$$ and construct a particular positive value of $$\varepsilon$$ that contradicts the hypothesis.




