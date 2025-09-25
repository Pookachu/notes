#### Overview
> The chain rule is used to find the derivative of a **composite function**—a function that is nested inside another function, like $f(g(x))$.

> The rule states that you take the derivative of the **outer function** (while leaving the inner function unchanged) and then multiply it by the derivative of the **inner function**.

#### Formulas:
1. **Lagrange Notation (Prime Notation):**
$$\begin{gather}
\text{if } h(x) = f(g(x)) \text{, then:} \\\\
h'(x) = f'(g(x))\cdot g'(x)
\end{gather}$$
2. **Leibinz Notation**
$$\begin{gather}
\text{if $y=f(u)$ and $u=g(x)$, then the derivative of $y$ with respect to $x$ is:} \\\\
\frac{dy}{dx}=\frac{dy}{du}\cdot\frac{du}{dx}
\end{gather}$$

#### Example
Find the derivative of $h(x) =(x^2+5)^3$
- Outer function: $f(u) = u^3$
- Inner function: $g(x) = x^2+5$
1. **Derivative of the inner function:** $f'(u) =3u^2 \to 3(x^2+5)^2$
2. **Derivative of the outer function:** $g'(x)= 2x$
3. **Multiply them together:** $h'(x) = 3(x^2+5)^2 \cdot (2x) = 6x(x^2+5)^2$
4. 
