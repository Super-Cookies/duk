---
title: Inequalities
enableToc: false
---

# What are they?

Inequalities are types of questions which involve two algebraic
expressions, one of which is lesser than the other. In school maths,
inequality questions generally ask you to find a range of values that
satisfy the inequality. For example, I’m sure most of you have seen
something similar to  
*’Find all x so that x + 3 ≥ 12’*. The other class of inequalities is
the main one that appears in olympiads, and the one this handout focuses
on. These types of questions provide you with two algebraic expressions,
and require that you prove that one is &lt;,≤,≥, or &gt; than the other.

# How to manipulate inequalities

You should probably know how to do this before moving on.

-   *a* &gt; *b* and *c* ≥ *d* ⟹ *a* + *c* &gt; *b* + *d*

-   If *c* &gt; 0, then *a* &gt; *b* ⟹ *a**c* &gt; *b**c*

-   And if *c* &lt; 0, then *a* &gt; *b* ⟹ *a**c* &lt; *b**c*

-   For *m* &gt; 0 and *a* &gt; *b*,
    *a*<sup>*m*</sup> &gt; *b*<sup>*m*</sup>. If *m* &lt; 0, then
    *a*<sup>*m*</sup> &lt; *b*<sup>*m*</sup>

# Some fundamental inequalities

**The trivial inequality:** *x*<sup>2</sup> ≥ 0 for any real *x*, with
equality at *x* = 0.  
This inequality is the foundation of several more, and something you
must know for any olympiad. It seems incredibly obvious, but it is also
quite powerful and can be used to derive a variety of results. For
example, try the following problem only using the trivial inequality:
Prove that for all triplets (*a*,*b*,*c*),  we have *a*<sup>2</sup> + *b*<sup>2</sup> + *c*<sup>2</sup> ≥ *a**b* + *b**c* + *a**c*
The more astute among you might immediately recognise what to do here.
If you can’t see it yet: don’t worry. It’s not very obvious to people
who are new to inequalities.  
We already know that we should be using the trivial inequality in some
way, so how?  
Well, let’s see what happens when we rearrange it: we have
*a*<sup>2</sup> + *b*<sup>2</sup> + *c*<sup>2</sup> − *a**b* − *a**c* − *b**c*.
It may remind you of the expansion of (*a*−*b*)<sup>2</sup>, but it’s
off by a factor of 2. So, consider the following
2*a*<sup>2</sup> + 2*b*<sup>2</sup> + 2*c*<sup>2</sup> − 2*a**b* − 2*a**c* − 2*b**c*,
which upon rearranging yields
*a*<sup>2</sup> − 2*a**b* + *b*<sup>2</sup> + *a*<sup>2</sup> − 2*a**c* + *c*<sup>2</sup> + *b*<sup>2</sup> − 2*b**c* + *c*<sup>2</sup> = (*a*−*b*)<sup>2</sup> + (*a*−*c*)<sup>2</sup> + (*b*−*c*)<sup>2</sup>.
By the trivial inequality, all of these squares must be at least 0, so
(*a*−*b*)<sup>2</sup> + (*a*−*c*)<sup>2</sup> + (*b*−*c*)<sup>2</sup> ≥ 0.
Upon dividing this by two, we get the original statement.  
  
We can now use the trivial inequality to prove a much more powerful
inequality.  
**The AM-GM inequality:**

$$\\text{For any positive reals } a\_1, a\_2, ..., a\_n \\text{ we have } \\frac{a\_1 + a\_2 + ... + a\_n}{n} \\geq \\sqrt\[n\]{a\_1a\_2\\cdots a\_n}$$
Ok, I lied a bit. While we can use the trivial inequality to prove it
for all *n*, the process is rather time-consuming, complicated, and just
generally annoying to write. We can, however, prove it fairly easy for
*n* = 2.
$$\\text{Prove that, for any two positive reals } a, b, \\hspace{10pt} \\frac{a+b}{2} \\geq \\sqrt{ab}$$
This looks weirdly close to a perfect square, except for that annoying
denominator on the LHS. So, we can double both sides and rearrange to
get:
$$a - 2\\sqrt{ab} + b \\geq 0$$
Which is indeed the expansion of $(\\sqrt{a} - \\sqrt{b})^2$, and so by
the trivial inequality we are done.  
  
  
Let’s try a simple inequality with the power of AM-GM:
Let *a*, *b*, *c* ≥ 0. Then, prove that (*a*+*b*)(*a*+*c*)(*b*+*c*) ≥ 8*a**b**c*
We can immediately see that we want to prove that a product of **sums**
is less than a **product**. In most of these kinds of problems, AM-GM
will do you just fine. So, we take a leap of faith and apply AM-GM to
each of the bracketed pairs (I divided each term by 2 to make it
clearer):
$$(a+b)(a+c)(b+c) = 8(\\frac{a+b}{2})(\\frac{a+c}{2})(\\frac{b+c}{2}) \\geq 8(\\sqrt{ab})(\\sqrt{ac})(\\sqrt{bc}) = 8 \\sqrt{a^2b^2c^2} = 8abc.$$
And we’re done. The AM-GM inequality is actually a corollary of a much
stronger, generalised inequality.  
  
  
**Warning:** Yes, what you are about to see is very complicated. You
don’t need to memorise this for AMO or ASC - only the most important
corollaries are required, which I will discuss after.  
**Power means inequality:**

$$\\text{For some positive reals } a\_1, a\_2,...,a\_n, \\text{ define} \\vspace{-10pt}$$

$$M\_r = (\\frac{a\_1^r+a\_2^r+...+a\_n^r}{n})^{\\frac{1}{r}} \\text{ for all non-zero reals } r \\text{ and } M\_0 = \\sqrt\[n\]{a\_1a\_2...a\_n}. \\vspace{-10pt}$$

Then, for *r* &gt; *s*, *M*<sub>*r*</sub> ≥ *M*<sub>*s*</sub> with equality if and only if *a*<sub>1</sub> = *a*<sub>2</sub> = ... = *a*<sub>*n*</sub>

You might notice that *M*<sub>1</sub> is actually just the AM, and
*M*<sub>0</sub> is just the GM. So, we already have the generalised
version of AM-GM just from this. But, there are only 4 means that are
actually relevant.  
**The actually important means: Quadratic - Arithmetic - Geometric -
Harmonic**

$$\\text{Define } QM = M\_2, AM = M\_1, GM = M\_0, HM = M\_{-1}.  \\vspace{-10pt}$$

$$\\text{Then, } M\_2 \\geq M\_1 \\geq M\_0 \\geq M\_{-1} \\text{ or, more clearly, }  \\vspace{-5pt}$$

$$\\sqrt{\\frac{a\_1^2 + a\_2^2 + ... + a\_n^2}{n}} \\geq \\frac{a\_1 + a\_2 + ... + a\_n}{n} \\geq \\sqrt\[n\]{a\_1a\_2...a\_n} \\geq \\frac{n}{\\frac{1}{a\_1} + \\frac{1}{a\_2} + ... + \\frac{1}{a\_n}}$$

It looks scary, but it’s actually a really powerful tool. Before we move
on, see if you can figure out how to prove GM-HM (i.e. the rightmost
part)! Hint: you’ll have to assume AM-GM is true and use that (I can’t
be bothered proving AM-GM for all *n* here, it’s far too long for me to
care. Just believe that it’s true and it will be - a surprisingly useful
strategy in olympiads)  
  
Now, let’s try tackle some problems using the powerful power means
inequality.
$$\\text{Suppose } x\_1, x\_2 ... x\_n \\text{ are positive reals so that } x\_1x\_2 \\cdots x\_n = 1. \\vspace{-16pt}$$

$$\\text{Then, for } r &gt; s &gt; 0, \\text{ we have } x\_1^r + x\_2^r + ... + x\_n^r \\geq x\_1^s + x\_2^s + ... + x\_n^s \\vspace{5pt}$$

This is about as close to power means as you can get, specifically
*M*<sub>*r*</sub> and *M*<sub>*s*</sub>. Writing this out:

$$(\\frac{x\_1^r+x\_2^r+...+x\_n^r}{n})^{\\frac{1}{r}} \\geq (\\frac{x\_1^s+x\_2^s+...+x\_n^s}{n})^{\\frac{1}{s}}$$
Which, upon raising both sides to the power of *r*, rearranges to
$$\\frac{x\_1^r + x\_2^r ... + x\_n^r}{n} \\geq (\\frac{x\_1^s+x\_2^s+...+x\_n^s}{n})^{\\frac{r}{s}} = (\\frac{x\_1^s+x\_2^s+...+x\_n^s}{n}) \\cdot (\\frac{x\_1^s+x\_2^s+...+x\_n^s}{n})^{\\frac{r}{s}-1}$$
But, by assumption we have $\\frac{r}{s} - 1 &gt; 0$, and by AM-GM we
have
$$\\frac{x\_1^s + x\_2^s + ... + x\_n^s}{n} \\geq \\sqrt\[n\]{x\_1^sx\_2^s...x\_n^s} = 1 \\implies (\\frac{x\_1^s + x\_2^s + ... + x\_n^s}{n})^{\\frac{r}{s} - 1} \\geq 1$$
$$\\text{So, } \\frac{x\_1^r + x\_2^r + ... + x\_n^r}{n} \\geq (\\frac{x\_1^s+x\_2^s+...+x\_n^s}{n}) \\cdot (\\frac{x\_1^s+x\_2^s+...+x\_n^s}{n})^{\\frac{r}{s}-1} \\geq \\frac{x\_1^s+x\_2^s+...+x\_n^s}{n}$$
And multiplying by *n* yields the desired inequality. This inequality is
also quite useful in it’s own right, so it’s definitely worth keeping in
mind.

**Cauchy-Schwarz:** Another powerful inequality.
$$\\text{For two sequences of real numbers } \\{ x\_1, x\_2, ..., x\_n\\} \\text{ and } \\{ y\_1, y\_2, ..., y\_n\\}, \\text{ we have } \\vspace{-5pt}$$
$$(x\_1^2 + x\_2^2 + ... + x\_n^2)(y\_1^2 + y\_2^2 + ... + y\_n^2) \\geq (x\_1y\_1 + x\_2y\_2 + ... + x\_ny\_n)^2 \\vspace{-1pt}$$
with equality if and only if there exists some constant *c* such that *y*<sub>*i*</sub> = *c**x*<sub>*i*</sub> for all *i*.
Cauchy-Schwarz is quite a powerful inequality, especially when it comes
to dealing with squares or square roots. As the holy grail of
mathematics, *Problem Solving Tactics*, says:
$$\\textit{If there are squares or square roots, try Cauchy-Schwarz.} \\vspace{-10pt}$$
$$\\textit{If there are products or fractions, try Cauchy-Schwarz.} \\vspace{-6pt}$$
*If all else fails, try Cauchy-Schwarz.*
So, with the power of Cauchy-Schwarz on our side, let’s try solve an
problem from a while back:
$$\\text{Prove AM-HM, that is, } \\frac{x\_1 + x\_2 + ... + x\_n}{n} \\geq \\frac{n}{\\frac{1}{x\_1} + \\frac{1}{x\_2} + ... + \\frac{1}{x\_n}}$$
Our first step when looking at this should probably be to recoil in fear
at the fractions-in-a-fraction. So, rearranging both sides allows us to
rephrase the problem statement as:
$$(x\_1 + x\_2 + ... + x\_n)(\\frac{1}{x\_1} + \\frac{1}{x\_2} + ... + \\frac{1}{x\_n}) \\geq n^2$$
Which is very Cauchy looking. Indeed, applying Cauchy-Schwarz to the
sequences $\\{\\sqrt{x\_1}, \\sqrt{x\_2}, ..., \\sqrt{x\_n}\\}$ and
$\\{ \\frac{1}{\\sqrt{x\_1}}, \\frac{1}{\\sqrt{x\_2}}, ..., \\frac{1}{\\sqrt{x\_n}}\\}$
yields
$$(x\_1 + x\_2 + ... + x\_n)(\\frac{1}{x\_1} + \\frac{1}{x\_2} + ... + \\frac{1}{x\_n}) \\geq (\\frac{\\sqrt{x\_1}}{\\sqrt{x\_1}} + \\frac{\\sqrt{x\_2}}{\\sqrt{x\_2}} + ... + \\frac{\\sqrt{x\_n}}{\\sqrt{x\_n}})^2 = n^2$$

**Rearrangment inequality:** This is quite cool.
$$\\text{If } a\_1 \\geq a\_2 \\geq ... \\geq a\_n \\text{ and } b\_1 \\geq b\_2 \\geq ... \\geq b\_n \\text{ are any two sequences of reals,} \\vspace{-10pt}$$
then for any permutation *β*<sub>1</sub>, *β*<sub>2</sub>, ..., *β*<sub>*n*</sub> of *b*<sub>1</sub>, *b*<sub>2</sub>, ..., *b*<sub>*n*</sub> we have the following inequality:
*a*<sub>1</sub>*b*<sub>2</sub> + *a*<sub>2</sub>*b*<sub>2</sub> + ... + *a*<sub>*n*</sub>*b*<sub>*n*</sub> ≥ *a*<sub>1</sub>*β*<sub>1</sub> + *a*<sub>2</sub>*β*<sub>2</sub> + ... + *a*<sub>*n*</sub>*β*<sub>*n*</sub> ≥ *a*<sub>1</sub>*b*<sub>*n*</sub> + *a*<sub>2</sub>*b*<sub>*n* − 1</sub> + ... + *a*<sub>*n*</sub>*b*<sub>1</sub>

It looks a bit complicated, so you can essentially think of it as saying
that the product of two sequences is maximised when the biggest ones are
paired up, and minimised when the biggest and smallest ones are paired
up. Let’s try a problem using this.
For positive reals, prove that *a*<sup>*a*</sup>*b*<sup>*b*</sup>*c*<sup>*c*</sup> ≥ *a*<sup>*b*</sup>*b*<sup>*c*</sup>*c*<sup>*a*</sup>
Handy trick for these kinds of problems: If there’s a lot of weird
powers, try logs!. Since the function *l**o**g*(*x*) is increasing, we
can take the logarithm of both sides without changing the inequality:
*a**l**o**g*(*a*) + *b**l**o**g*(*b*) + *c**l**o**g*(*c*) ≥ *a**l**o**g*(*b*) + *b**l**o**g*(*c*) + *c**l**o**g*(*a*)
(Simplified using log laws). But upon considering the two sequences
*a*, *b*, *c* and *l**o**g*(*a*), *l**o**g*(*b*), *l**o**g*(*c*), and
noting that *a* ≥ *b* ⟹ *l**o**g*(*a*) ≥ *l**o**g*(*b*), we find that,
by the rearrangement inequality, their products are maximised when
sorted the same way, easily solving the question.

# Weirder inequalities

The inequalities in this section are weirder, and while they are helpful
in higher level olympiads (AMO Q4/8’s, EGMO, IMO), you’ll almost never
need to use them. Also, they’re sort of fringe inequalities, so I
haven’t explained or provided example problems here, only their
statement.  
  
**Jensen’s inequality**
If the real numbers *x*<sub>1</sub>, *x*<sub>2</sub>, ..., *x*<sub>*n*</sub> lie on an interval where some function *f*(*x*) is convex, then 
$$\\frac{f(x\_1) + f(x\_2) + ... + f(x\_n)}{n} \\geq f(\\frac{x\_1 + x\_2 + ... + x\_n}{n})$$
$$\\text{and the inequality is reversed if $f(x)$ is concave on that interval.} \\vspace{10pt}$$
**Weighted Power Means**
$$\\text{Given positive reals } x\_1, x\_2, ..., x\_n \\text{ and weights } w\_1, w\_2, ..., w\_n, \\text{ with sum $w$, define $M\_r$ as } \\vspace{-5pt}$$
$$M\_r = (\\frac{w\_1a\_1^r+w\_2a\_2^r+...+w\_na\_n^r}{w})^{\\frac{1}{r}} \\text{ for all non-zero reals } r \\text{ and } M\_0 = \\sqrt\[w\]{a\_1^{w\_1}a\_2^{w\_2}...a\_n^{w\_n}}. \\vspace{-2pt}$$
Then, *M*<sub>*r*</sub> ≥ *M*<sub>*s*</sub> for *r* &gt; *s*, with equality if and only if *a*<sub>1</sub> = *a*<sub>2</sub> = ... = *a*<sub>*n*</sub> or *w*<sub>1</sub> = *w*<sub>2</sub> = ... = *w*<sub>*n*</sub> = 0
$$\\text{Setting } w\_1 = w\_2 = ... = w\_n = 1 \\text{ results in the original unweighted power means inequality.}  \\vspace{10pt}$$
**Hölder’s inequality**
$$\\text{Let } a\_1, a\_2, ..., a\_n \\text{ and } b\_1, b\_2, ..., b\_n \\text{ be two sets of non-negative reals. Let $p, q \\in \\mathbb{R}$ such that } \\frac{1}{p} + \\frac{1}{q} = 1. \\vspace{-15pt}$$
$$\\text{Then, } (a\_1^p + a\_2^p + ... + a\_n^p)^{\\frac{1}{p}}(b\_1^q + b\_2^q + ... + b\_n^q)^{\\frac{1}{q}} \\geq a\_1b\_1 + a\_2b\_2 + ... + a\_nb\_n \\vspace{10pt}$$
**Tangent-line trick:**
$$\\text{Suppose we have reals } x\_1, x\_2, ..., x\_n \\text{ that sum to $s$. Then, for some function} \\vspace{-6pt}$$
$$f(x) \\geq ax + b \\text{ for all $x$ and some constants $a,b$, we have } f(x\_1) + f(x\_2) + ... f(x\_n) \\geq as + bn. \\vspace{10pt}$$
**Muirhead’s inequality:** Very cool inequality but it will literally
never be useful.
$$\\text{A sequences of reals } A = (a\_1, a\_2, ..., a\_n) \\text{ is said to majorise another sequence } B = (b\_1, b\_2, ..., b\_n) \\text{ if} \\vspace{-8pt}$$
$$a\_1 \\geq a\_2 \\geq ... \\geq a\_n \\text{ and } b\_1 \\geq b\_2 \\geq ... \\geq b\_n \\text{ and for all } 1 \\leq i &lt; n, \\text{ we have} \\vspace{-3pt}$$
*a*<sub>1</sub> + *a*<sub>2</sub> + ... + *a*<sub>*i*</sub> ≥ *b*<sub>1</sub> + *b*<sub>2</sub> + ... + *b*<sub>*i*</sub>,  along with *a*<sub>1</sub> + *a*<sub>2</sub> + ... + *a*<sub>*n*</sub> = *b*<sub>1</sub> + *b*<sub>2</sub> + ... + *b*<sub>*n*</sub>.
So, Muirhead’s inequality says that if a sequence *A* majorises another sequence *B*, then we have:
$$\\sum\_{sym} x\_1^{a\_1}x\_2^{a\_2} \\cdots x\_n^{a\_n} \\geq \\sum\_{sym} x\_1^{b\_1}x\_2^{b\_2} \\cdots x\_n^{b\_n} \\hspace{10pt} \\text{ for any non-negative reals } x\_1, x\_2, ..., x\_n.  \\vspace{10pt}$$
**Schur’s inequality:** Also cool but probably useless.
For all non-negative reals *a*, *b*, *c*, *r*,  we have: *a*<sup>*r*</sup>(*a*−*b*)(*a*−*c*) + *b*<sup>*r*</sup>(*b*−*a*)(*b*−*c*) + *c*<sup>*r*</sup>(*c*−*a*)(*c*−*b*) ≥ 0

# Assorted problems to try

*Arranged in roughly increasing difficulty*  
  
**Problem 1:** Find the minimum value of *a**b**c* given
*a* + 4*b* + 16*c* = 256  
  
**Problem 2:** Suppose
*x*<sub>1</sub>, *x*<sub>2</sub>, ..., *x*<sub>*n*</sub> are positive
reals with product 1. Prove that

(1+*x*<sub>1</sub>)(1+*x*<sub>2</sub>)...(1+*x*<sub>*n*</sub>) ≥ 2<sup>*n*</sup>

**Problem 3:** If *a*, *b*, *c* are positive reals, prove that
$\\frac{a}{b+c} + \\frac{b}{a+c} + \\frac{c}{a + b} \\geq \\frac{3}{2}$
in three different ways  
  
**Problem 4:** For positive *a*, *b*, if *a* + *b* = 1, prove that
$$\\frac{(a+1)(b+1)}{ab} \\geq \\frac{9}{4}$$

**Problem 5:** For positive reals *a*, *b*, *c*, *d*, prove that
$$\\frac{1}{a} + \\frac{1}{b} + \\frac{4}{c} + \\frac{16}{d} \\geq \\frac{64}{a+b+c+d}$$

**Problem 6:** Let *A*, *B*, *C* be the angles of an acute triangle.
Prove that
$$\\text{ sin }A + \\text{ sin }B + \\text{ sin }C \\leq \\frac{3\\sqrt{3}}{2}$$

**Problem 7:** Let *x* &gt; 1 be a real number, and *n* &gt; 1 be an
integer. Prove that
$$1 + \\frac{x-1}{nx} &lt; \\sqrt\[n\]{x} &lt; 1 + \\frac{x-1}{n}$$

**Problem 8:** For positive reals *a*, *b*, *c*, prove that
$$\\frac{a+b+c}{3} \\geq \\sqrt{\\frac{ab + bc + ac}{3}}$$

**Problem 9:** For *n* ≥ 3, let
*a*<sub>2</sub>, *a*<sub>3</sub>, ..., *a*<sub>*n*</sub> be positive
reals such that *a*<sub>2</sub>*a*<sub>3</sub>...*a*<sub>*n*</sub> = 1.
Prove that

(1+*a*<sub>2</sub>)<sup>2</sup>(1+*a*<sub>3</sub>)<sup>3</sup>...(1+*a*<sub>*n*</sub>)<sup>*n*</sup> &gt; *n*<sup>*n*</sup>

**Problem 10:** Let *a* ≥ *b* ≥ *c* ≥ *d* &gt; 0 be reals so that
*a* + *b* + *c* + *d* = 1. Prove that
(*a*+2*b*+3*c*+4*d*)*a*<sup>*a*</sup>*b*<sup>*b*</sup>*c*<sup>*c*</sup>*d*<sup>*d*</sup> &lt; 1

**ISL Time!** These problems are from past IMO’s, and also IMO
Shortlist. A few of these are A6-8’s i.e. the hardest problems proposed
for the IMO, and insanely difficult to solve. So don’t feel bad if you
spend a month on one and can’t solve it. The last one is the legendary
IMO 2021 Q2, which only had 16 solves and an average score of 0.375/7.
Good luck!  
  
**Problem 11:** Prove that, for all positive reals *a*, *b*, *c*,
(*a*<sup>2</sup>+2)(*b*<sup>2</sup>+2)(*c*<sup>2</sup>+2) ≥ 9(*a**b*+*b**c*+*a**c*)

**Problem 12:** Suppose *a*, *b*, *c*, *d* are non-negative reals with
sum 4. Determine the minimal value of
$$\\frac{a}{b^3+4} + \\frac{b}{c^3+4} + \\frac{c}{d^3+4} + \\frac{d}{a^3+4}$$

**Problem 13:** Prove that for all positive reals *a*, *b*, *c*, *k*, we
have
$$\\frac{a}{\\sqrt{a^2 + kbc}} + \\frac{b}{\\sqrt{b^2 + kac}} + \\frac{c}{\\sqrt{c^2 + kab}} \\geq \\frac{3}{\\sqrt{1+k}}$$

**Problem 14:** Let
*a*<sub>1</sub>, *a*<sub>2</sub>, ..., *a*<sub>*n*</sub>, *b*<sub>1</sub>, *b*<sub>2</sub>, ..., *b*<sub>*n*</sub>
be non-negative real numbers. Prove that
$$\\sum\_{i=1}^n \\sum\_{j=1}^n \\text{min}(a\_ia\_j, b\_ib\_j) \\leq \\sum\_{i=1}^n \\sum\_{j=1}^n \\text{min}(a\_ib\_j, a\_jb\_i)$$

**Problem 15:** Let
*x*<sub>1</sub>, *x*<sub>2</sub>, ..., *x*<sub>*n*</sub>, *y*<sub>1</sub>, *y*<sub>2</sub>, ..., *y*<sub>*n*</sub> ∈ \[0,1\]
be reals such that *x*<sub>*i*</sub> + *y*<sub>*i*</sub> = 1 for all
*i* ≤ *n*.

For any positive integer *m*, prove
(1−*x*<sub>1</sub>*x*<sub>2</sub>...*x*<sub>*n*</sub>)<sup>*m*</sup> + (1−*y*<sub>1</sub><sup>*m*</sup>)(1−*y*<sub>2</sub><sup>*m*</sup>)...(1−*y*<sub>*n*</sub><sup>*m*</sup>) ≥ 1

**Problem 16:** Let *a*, *b*, *c* be positive reals such that
*a*<sup>2</sup> + *b*<sup>2</sup> + *c*<sup>2</sup> + *a**b**c* = 4.
Prove that
0 ≤ *a**b* + *b**c* + *a**c* − *a**b**c* ≤ 2

**Problem 17:** Let
*a*<sub>1</sub>, *a*<sub>2</sub>, ..., *a*<sub>*n*</sub> ∈ \[1,2<sup>*k*</sup>\]
for some *n*, *k*. Prove that
$$\\sum\_{i=1}^n \\frac{a\_i}{\\sqrt{a\_1^2 + ... + a\_i^2}} \\leq 4\\sqrt{kn}$$

**Problem 18:** If *a*, *b*, *c*, *d* are non-negative reals with sum
100, find the maximal value of
$$\\sqrt\[3\]{\\frac{a}{b+7}} + \\sqrt\[3\]{\\frac{b}{c+7}} + \\sqrt\[3\]{\\frac{c}{d+7}} + \\sqrt\[3\]{\\frac{d}{a+7}}$$

**Problem 19:** Prove that, for all
*x*<sub>1</sub>, *x*<sub>2</sub>, ...*x*<sub>*n*</sub> ∈ ℝ
$$\\sum\_{1 \\leq i \\leq j \\leq n}\\sqrt{|x\_i - x\_j|} \\leq \\sum\_{1 \\leq i \\leq j \\leq n}\\sqrt{|x\_i + x\_j|} \\\\$$