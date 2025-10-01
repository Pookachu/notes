
1. $\lim_{x\to\infty}\frac{\sqrt{49x^6+5x-1}}{7x^3+2}$
$$\begin{aligned}
&\lim_{x\to\infty}\frac{\sqrt{49x^6(1+{5\over49x^5}-{1\over49x^6})}}{7x^3+2} \\\\
=&\lim_{x\to\infty}\frac{\sqrt{49x^6}\sqrt{1+{5\over49x^5}-{1\over49x^6}}}{7x^3+2} \\\\
=& \lim_{x\to\infty} \frac{7x^3\sqrt{1+{5\over49x^5}-{1\over49x^6}}}{7x^3+2} \\\\
=& \boxed1
\end{aligned}$$

2. $\lim_{x\to-\infty}\frac{3x^5-1}{x^2+5}$
$$\begin{aligned}
=&\lim_{x\to-\infty}\frac{\frac{3x^5}{x^2}-\frac{1}{x^2}}{\frac{x^2}{x^2}+\frac{5}{x^2}} \\\\
=&\lim_{x\to-\infty}\frac{3x^3-\frac{1}{x^2}}{1+\frac{5}{x^2}} \\\\
=&\frac{-\infty-0}{1+0} = -\boxed{\infty}
\end{aligned}$$

3. Use limits to find the equation(s) of the horizontal asymptote(s) of
	$f(x)=\frac{5x}{x^2-9}$
$$\begin{aligned}
=&\lim_{x\to\infty} f(x)\cup \lim_{x\to-\infty}f(x) \\\\ 
&\lim_{x\to\infty} f(x) = 0
&\lim_{x\to\infty} f(x) = 0 \\\\
&\text{H.A.} = \boxed{y=0}
\end{aligned}$$

4. Evaluate the limit or state it does not exist. Support your answer.
	$\lim_{x\to1}\frac{2x}{x-1}$
$$\begin{aligned}
=&\lim_{x\to1^+}\frac{2x}{x-1},\quad\lim_{x\to1^-}\frac{2x}{x-1} \\\\
=&\lim_{x\to1^+}\frac{2(1^+)}{1^+-1}=\infty \\
=&\lim_{x\to1^-}\frac{2(1^-)}{1^--1}=-\infty \\\\
&\lim_{x\to1}=\boxed{\text{DNE}}
\end{aligned}$$
