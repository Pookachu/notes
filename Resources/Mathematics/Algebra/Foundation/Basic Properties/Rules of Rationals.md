---
aliases:
  - Rational Number
  - Rational Function
  - Rational
  - Fraction
---
#### **What is a Rational Number?**

> A **rational number** is any number that can be expressed as a fraction $p\over q$​, where $p$ and $q$ are [[Integers]] and $q$ is not zero. This includes whole numbers (e.g., $5={5\over1 }$​), fractions, and terminating or repeating decimals.

#### **What is a Rational Function?**

> A **rational function** is a function that is the ratio of two [[Polynomial]]s, written $f(x)= {P(x)\over Q(x)}$​, where $Q(x)$ is not the zero polynomial.

The most important thing to analyze in a rational function is its **asymptotes** and **intercepts**.

---

#### Domain and Points of Discontinuity
> The **domain** of a rational function includes all real numbers except for the values of $x$ that make the denominator, $Q(x)$, equal to zero. These points where the function is undefined are called points of dis[[continuity]].

There are two types of discontinuities:

1. **Vertical Asymptotes (VA)**
>A vertical asymptote is a vertical line that the graph of the function approaches but never touches.

- **How to find it:** Factor the numerator and the denominator completely. A vertical asymptote occurs at any value of $x$ for which a factor in the **denominator is zero**, but the corresponding factor in the **numerator is not zero**.

**Example:**
	For the function $f(x)=\frac{x+2}{(x-3)(x+1)}$, the vertical asymptotes are $x=3$ and $x=-1$.

2. **Holes**
> A hole is a single point where the function is undefined, but the graph otherwise continues smoothly.

- **How to find it:** After factoring, a hole occurs at any value of $x$ for which a factor is zero in **both the numerator and the denominator**. To find the coordinates of the hole, cancel the common factor and substitute the x-value into the simplified function to find the y-coordinate.

**Example**:
For $f(x) = \frac{(x-2)(x+5)}{x-2}$, the common factor is $(x-2)$.
- There is a hole at $x=2$ 
- The simplified function is $f(x)= x+5$.
- The y-coordinate of the hole is $2+5=7$ so the hole is at $(2,7)$.

---

#### Horizontal Asymptotes (HA)
> A horizontal asymptote is a horizontal line that the graph approaches as $x$ approaches $∞$ or $−∞$. To find it, compare the degree of the numerator, $N$, to the degree of the denominator, $D$.

- **Case 1:** $N < D$
	The HA is the x-axis, y = 0.
	**Example:** $f(x)= \frac{x}{x^2+1}$

- **Case 2:** $N = D$ 
	The HA is the line $y = \frac{\text{leading coefficient of numerator}}{\text{leading coefficient of denominator}}$.
	**Example:** For $f(x)={3x^2+2\over2x^2-1}$, the HA is $y = {3\over 2}$

- **Case 3:** $N > D$
> There is **no horizontal asymptote**. If the degree of the numerator is exactly one greater than the degree of the denominator $(N=D+1)$, there is a **slant (or oblique) asymptote**. You can find it by performing [[polynomial long division]].

---

#### Intercepts
- **$x$-intercepts:** These occur when the graph crosses the $x$-axis $(y=0)$. To find them, **set the numerator equal to zero** and solve for $x$.
	**Example**: For $f(x)= \frac{x-4}{x+1}$, the $x$-intercept is at $x=4$.

- **$y$-intercept:** This occurs where the graph crosses the $y$-axis $(x=0)$. To find it, **evaluate the function at $f(0)$.**
	**Example:** For $f(x) = \frac{x-4}{x+1}$, the $y$-intercept is $f(0) = \frac{-4}{1} = -4$
