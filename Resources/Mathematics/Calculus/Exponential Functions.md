#### Section 3.8 Derivatives of inverse functions and logarithms

##### Exponential Functions:
>${d\over dx}e^x = e^x$
  ${d\over dx}e^{f(x)} =e^{f(x)}\cdot f'(x)$
  ${d\over dx}(a^x)=a^x\cdot\ln a$
  $\boxed{{d\over dx}(a^{f(x)}) = a^{f(x)}\cdot\ln a \cdot f'(x)}$*
 Write down what you have, multiply by $\ln$ of base, multiply by derivative of exponent

Example: Find $f'(x)$ given $f(x)= 2\cdot8^{3x}+\cos(e^{-x})$
$$\begin{gather}
f'(x) = 2\cdot8^{3x}\cdot\ln8\cdot{d\over dx}(3x)+-\sin(e^{-x})\cdot{d\over dx}(e^{-x}) \\\\
= 2\cdot8^{3x}\cdot\ln8\cdot3-\sin(e^{-x})\cdot e^{-x}\cdot{d\over dx}(-x) \\\\
=6\cdot8^{3x}\cdot\ln8-\sin(e^{-x})\cdot e^{-x}\cdot(-1) \\\\
= \boxed{6\cdot8^{3x}\cdot \ln8+\sin(e^{-x})\cdot e^{-x}}
\end{gather}$$

Example: Find ${dy\over dx}$ for $\log_a x=y$ $\quad\Leftrightarrow\quad$ $a^y=x$
Use implicit differentiation for $a^y=x$
$$\begin{aligned}
{d\over dx}a^y={d\over dx}(x)\\\\
a^y\cdot\ln a\cdot{dy\over dx}=1 \\
\Rightarrow{dy\over dx} = \frac{1}{a^y\cdot\ln a}\\
\text{As stated earlier, $a^y=x$.} \\
{dy\over dx} = \frac{1}{x\cdot\ln a}
\end{aligned}$$

>$$\begin{aligned}
	&{d\over dx}(log_ax)={1\over x\cdot\ln a} \\
	&{d\over dx}(log_ex)= {d\over dx}(\ln x)= {1\over x \ln e} = {1\over x}\\
	&\boxed{{d\over dx}\left(log_af(x)\right)={1\over f(x)\cdot\ln a}\cdot f'(x)={f'(x)\over f(x)\cdot\ln a}} \\
	&\text{Need to know }
\end{aligned}$$


ex: Find $h'(x)$ given $h(x) = x\cdot\ln(\cot^2x)$
$$\begin{gather}
h'(x)=x\cdot{d\over dx}(\ln(\cot^2x))+{d\over dx}(x)\cdot\ln(\cot^2x) \\
\text{log chain}\quad\quad\quad\text{power}\\\\
=x\cdot {1\over\cot^2x\cdot\cancelto{1}{\ln e}}\cdot{d\over dx}(\cot^2x)+1\cdot\ln(\cot^2x) \\
\qquad\qquad\qquad\text{Chain out $()^2$ | in: $\cot x$}\\\\
={x\over \cot^\cancel2 x}\cdot2\cancel{(\cot x)}\cdot{d\over dx}(\cot x) + \ln(\cot^2x) \\
=\boxed{{2x\over\cot x} \cdot(-csc^2x)+\ln(\cot^2x)}
\end{gather}$$

#### Section 3.9 Inverse trig functions
Derivatives of inverse trigonometric functions

| **1** ${d\over dx}(\arcsin x) = {1\over \sqrt{1-x^2}}\quad(\vert x\vert < 1)$               | **4.**${d\over dx}(\arccos x) = -{1\over\sqrt{1-x^2}}\quad(\vert x\vert < 1)$                |
| ------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| **2.**${d\over dx}(\arctan x)= {1\over1+x^2}$                                               | **5.**${d\over dx}(\text{arccot }x)=-{1\over1+x^2}$                                          |
| **3.**${d\over dx}(\text{arcsec } x)={1\over\vert x\vert\sqrt{x^2-1}}\quad(\vert x\vert>1)$ | **6.**${d\over dx}(\text{arccsc } x)=-{1\over\vert x\vert\sqrt{x^2-1}}\quad(\vert x\vert>1)$ |
ex: w