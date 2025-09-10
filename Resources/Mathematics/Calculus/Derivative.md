---
aliases:
  - Differentiation
---
#### Definition of the Derivative

> The derivative of a function , denoted as , is the [[limit]] of the [[difference quotient]] as the interval width approaches zero. It represents the functions instantaneous rate of change at a specific point. 
$$f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}$$
---
#### Core interpretation 

> The derivative has two primary interpretations that are crucial to understand:

1. **Geometric Interpretation (Slope of the [[tangent]] line)**
	The derivative $f'(x)$ gives the **slope of the line tangent** to the graph of $f(x)$ at the point where $x=a$. This is the most important visual and conceptual meaning of the derivative.
![[Tangent and Secant Line.png]]

2. **Physical interpretation (Instantaneous Rate of Change)**
	The derivative measures how fast a function's output is changing relative to its input. If $f(t)$ represents an object's position at time $t$, then the derivative $f'(t)$ represents its instantaneous **velocity** at time $t$.

---
#### Notations of the Derivative
> There are several ways to write the derivative of the function $y = f(x)$:
- **Lagrange Notation:** $f'(x)$ (read "$f$ prime of $x$")
- **Leibniz Notation:** $\frac{dy}{dx}$ (read "d y d x")
- **Newton Notation:** $\dot{y}$ (used primarily in physics)  
---
#### Fundamental Differentiation Rules
> These are the essential shortcuts for finding derivatives without using the limit definition every time.

| Rule name               | Formula                                         |
| ----------------------- | ----------------------------------------------- |
| **Constant Rule**       | $\frac{d}{dx}(c) = 0$                           |
| **Power Rule**          | $\frac{d}{dx}(x^2) =nx^{n-1}$                   |
| **Sum/Difference Rule** | $\frac{d}{dx}(f \pm g) = f' \pm g'$             |
| **Product Rule**        | $\frac{d}{dx}(fg)=f'g+fg'$                      |
| **Quotient Rule**       | $\frac{d}{dx}(\frac{f}{g})=\frac{f'g-fg'}{g^2}$ |
| **Chain Rule**          | $\frac{d}{dx}(f(g(x))) =f'(g(x))\cdot g'(x)$    |

---
#### Key Concepts
- **Differentiability and [[Continuity]]:** If a function is **Differentiable** at a point, it must be **Continuous** at that point. However, a function can be continuous but not differentiable (e.g., a sharp corner like in $y=|x|$ at $x=0$).

- **The Derivative and Function Behavior:**
	- If $f'(x) > 0$ on an interval, then $f(x)$ is **increasing** on that interval.
	- If $f'(x) < 0$ on an interval, then $f(x)$ is **decreasing** on that interval.
	- if $f'(x) = 0$, the function has a **[[critical point]]** (a potential local maximum, minimum, or saddle point).
