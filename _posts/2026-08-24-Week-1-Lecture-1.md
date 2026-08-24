---
layout: post
title:  Lecture 1
---

## Properies of real numbers

### Key words
integers, rational numbers, real numbers, irrational numbers, algebraic numbers, transcendental numbers, field axioms, order axioms

### Practice problems




### Reading assignment
Apostol pp. 1.1-1.15
TH 350 - Lecture 1 Practice Problems

Based on [Lecture 1: Foundations and the Tenth Axiom](https://wcasper.github.io/math350fall2026/slides/lec01/lec01.pdf).

## Instructions

- Write complete sentences for conceptual questions.
- For proof problems, justify each step using a field axiom, an order axiom, or a result proved earlier in the assignment.
- Unless otherwise stated, \(F\) denotes a field and \(x,y,z\in F\).
- In Problems 7-10, assume \(F\) is an ordered field.

## Problems

1. **Classifying numbers.** For each number below, give the most specific classification justified by the lecture: natural, integer, rational, algebraic irrational, transcendental real, or nonreal complex.

   \[
   -4,\qquad \frac{7}{12},\qquad \sqrt{2},\qquad
   \sqrt[3]{5},\qquad \pi,\qquad e,\qquad
   \frac{1+\sqrt{5}}{2},\qquad 3-2i.
   \]

   For each algebraic irrational in the list, exhibit a nonzero polynomial in \(\mathbb{Q}[t]\) having it as a root.

2. **Algebraic and transcendental numbers.** Decide whether each statement is true, false, or currently unknown. Briefly justify your answer.

   1. Every rational number is algebraic.
   2. Every irrational number is transcendental.
   3. Every transcendental real number is irrational.
   4. The numbers \(e\) and \(\pi\) are transcendental.
   5. The number \(e+\pi\) is known to be transcendental.

3. **Basic consequences of the field axioms.** Prove each statement directly from the field axioms.

   1. The additive identity is unique.
   2. The multiplicative identity is unique.
   3. The right-distributive law holds:

      \[
      (x+y)z=xz+yz.
      \]

4. **Zero and multiplication.** Prove that

   \[
   x\cdot 0=0
   \]

   for every \(x\in F\). Your argument must not assume in advance that \(x(-1)=-x\).

   Then identify the unjustified step in the tempting argument

   \[
   x0=x(1+(-1))=x+x(-1)=x+(-x)=0
   \]

   and explain why using it would be circular.

5. **Inverses and signs.** Prove each identity, citing uniqueness of inverses when appropriate.

   1. Additive inverses are unique.
   2. Multiplicative inverses of nonzero elements are unique.
   3. \(-(-x)=x\).
   4. \(x(-1)=-x\).
   5. \((-x)(-y)=xy\).

6. **Examples and nonexamples of fields.**

   1. Explain precisely why \(\mathbb{Z}\) is not a field under its usual operations.
   2. Verify that the two-element set \(\mathbb{F}_2=\{0,1\}\), with \(1+1=0\), is a field by writing its addition and multiplication tables and identifying all inverses.
   3. Prove that a field has no zero divisors: if \(xy=0\), then \(x=0\) or \(y=0\).

7. **Reversing an inequality.** Using only the order axioms and field identities proved above, show that

   \[
   x<y\quad\Longrightarrow\quad -y<-x.
   \]

   Deduce that \(0<x\) if and only if \(-x<0\).

8. **Positivity in an ordered field.** Prove the following statements.

   1. \(0<1\).
   2. \(x^2\ge 0\) for every \(x\in F\).
   3. If \(x\neq 0\), then \(x^2>0\).

9. **Why \(\mathbb{F}_2\) cannot be ordered.** Prove that no relation \(<\) can make \(\mathbb{F}_2\) into an ordered field. Your proof should identify exactly which order axiom would be contradicted.

10. **Apostol's Theorem 1.1.** Suppose \(a,b\in F\) satisfy

    \[
    a<b+\varepsilon
    \qquad\text{for every }\varepsilon>0.
    \]

    Prove that \(a\le b\). If you argue by contradiction, explicitly choose a positive value of \(\varepsilon\) in terms of \(a\) and \(b\).


### Slides

* [Link to slides](http://wcasper.github.io/math350fall2026/slides/lec01/lec01.pdf)




