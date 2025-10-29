## Math 1296

The exam covers material from sec 3.6-3.11, 4.1. This includes material from class, homework, practice problems, LA sessions, and quizzes.

Please answer all questions carefully and show all your work. Proper notation must be used for full credit on the exam. A non-graphing calculator may be used.

---

### Derivative Rules
1.  $\frac{d}{dx}(arc~sin~x)=\frac{1}{\sqrt{1-x^{2}}}(|x|<1)$
2.  $\frac{d}{dx}(arctan~x)=\frac{1}{1+x^{2}}$
3.  $\frac{d}{dx}(arcsec~x)=\frac{1}{|x|\sqrt{x^{2}-1}}(|x|>1)$
4.  $\frac{d}{dx}(arccos~x)=-\frac{1}{\sqrt{1-x^{2}}}(|x|<1)$
5.  $\frac{d}{dx}(arccot~x)=-\frac{1}{1+x^{2}}$
6.  $\frac{d}{dx}(arccsc~x)=-\frac{1}{|x|\sqrt{x^{2}-1}}(|x|>1)$

---

## Problems

1.  Use the derivative rules to find the derivatives of the following functions. You do NOT have to simplify.
    a) $f(x)=\cot(x^{5})-\frac{1}{2}x^{4}+3x^{2}\ln(x+1)$
		$$\begin{aligned}
		{dy \over dx} &= {d \over dx}(\cot(x^5))-{1\over2}{d \over dx}(x^4)+3{d \over dx}(x^2 \ln(x+1)) \\\\
		&= -\csc^2({x^5})5x^4-{1\over2}4x^3+3\left({d \over dx}(x^2)\ln(x+1)+{d \over dx}(\ln(x+1)x^2)\right) \\\\
		&= \boxed{-\csc^2({x^5})5x^4-{1\over2}4x^3+3\left(2x\ln(x+1)+{x^2\over x+1}\right)} \\\\
		\end{aligned}$$
		
    b) $f(x)=\frac{e^{-2x}+\log_{7}(2x^{3}-9\cdot \sin x)}{x^{2}+3^{5x}}$
	    $$\begin{aligned}
	    
	    1.~ {dy \over dx} &= \frac{{d \over dx}\left(e^{-2x}+\log_7(2x^3-9\cdot\sin x\right))(x^2+3^{5x}) -{d \over dx}\left(x^2+3^{5x}\right)(e^{-2x}+\log_{7}(2x^3-9\cdot \sin x))}{(x^2+3^{5x})^2} \\\\
	    
	    2.~ {d \over dx} &\left(e^{-2x}+\log_7(2x^3-9\cdot\sin x\right)) = {d \over dx}(e^{-2x}) +{d \over dx}\left(\log_7(2x^3-9\sin x)\right) \\\\
	    
	    3.~~~\quad &= -2e^{-2x}+ \frac{{d \over dx}(2x^3-9\sin x)}{(2x^3-9\sin x)\ln7} \\\\
	    
	    4.~ {d \over dx} &(2x^3-9\sin x) = 6x^2 -9\cos x  \\\\
	    
	    5.~ {dy \over dx} &= \frac{-2e^{-2x}(\frac{6x^2-9\cos x}{(2x^3-9\sin x)\ln7})(x^2+3^{5x}) -{d \over dx}\left(x^2+3^{5x}\right)(e^{-2x}+\log_{7}(2x^3-9\cdot \sin x))}{(x^2+3^{5x})^2} \\\\
	    
	    6.~ {d \over dx}& \left(x^2+3^{5x}\right) = {d \over dx}x^2+{d \over dx}3^{5x} = 2x+ 3^{5x}\ln3\cdot5\\\\
	    
	    7.~ {dy \over dx} &= \boxed{\frac{-2e^{-2x}(\frac{6x^2-9\cos x}{(2x^3-9\sin x)\ln7})(x^2+3^{5x}) -\left(2x+3^{5x}\ln3\cdot5\right)(e^{-2x}+\log_{7}(2x^3-9\cdot \sin x))}{(x^2+3^{5x})^2}} \\\\
	    
	    \end{aligned}$$
	    
    c) $f(x)=\left(\log_{3}(x^{2}-7^{x+\csc~x})\right)^{4}$
	    $$\begin{aligned} 
	    1.~ {dy \over dx}& = 4\left(\log_3(x^2-7^{x+\csc x}\right)^3 \cdot{d\over dx}(\log_3(x^2-7^{x+\csc x})) \\\\
	    
	    2.~ {d\over dx}& (\log_3(x^2-7^{x+\csc x})) = \frac{{d\over dx}(x^2-7^{x+\csc x})}{\ln3(x^2-7^{x+\csc x})} \\\\
	    
	    3.~ {d\over dx}& (x^2-7^{x+\csc x}) = 2x-7^{x+\csc x}\ln(7)(1-(\csc x \cot x)) \\\\
	    
	    4.~ {dy \over dx}& = \boxed{4\left(\log_3(x^2-7^{x+\csc x}\right)^3 \cdot \frac{2x-7^{x+\csc x}\ln(7)(1-(\csc x \cot x))}{\ln3(x^2-7^{x+\csc x})}}
	    \end{aligned}$$
	    
    d) $f(x)=\sqrt{tan^{2}(3x)+5}$
	    $$\begin{aligned} 
	    1.~& {dy \over dx} = \frac{1}{2\sqrt{\tan^2(3x)+5}} \cdot {d \over dx}\left(\tan^2(3x)+5\right)\\\\
	    
	    2.~& {d \over dx}\left(\tan^2(3x)+5\right) = 6\tan(3x)\sec^2(3x) \\\\
	    
	    3.~& {dy \over dx} = \boxed{\frac{3\tan(3x)\sec^2(3x)}{\sqrt{\tan^2(3x)+5}}}
	    \end{aligned}$$
    e) $f(x)=5x^{2}\sec^{9}x+4x+\cos(2-x)$
	    $$\begin{aligned}
	    1.~& {dy \over dx} = \left({d \over dx}\left( 5x^2\right)(\sec^9x)+ {d \over dx}\left(\sec^9x\right)(5x^2) \right) + {d \over dx}(4x)+{d \over dx}(\cos(2-x))
	    \\\\
	    2.~& {d \over dx}\left( 5x^2\right)(\sec^9x)+ {d \over dx}\left(\sec^9x\right)(5x^2) = 10x\cdot\sec^9x+5x^2\cdot9\sec^8x\sec x\tan x
	    \\\\
	    3.~& {d \over dx}(\cos(2-x)) = -\sin(2-x)(-1)=\sin(2-x)
	    \\\\
	    4.~& {dy \over dx} = \boxed{10x\cdot\sec^9x +45x^2\sec^8x\sec x\tan x +4 +\sin(2-x)}
	    \end{aligned}$$
	    
    f) $f(x)=\sin^{-1}(6x)-10\cdot2^{x}+e^{x}\tan^{-1}(3x^{2}-2)$
		$$\begin{aligned}
		1.~& {dy \over dx} = {d \over dx}(\sin^{-1}(6x))-10{d \over dx}(2^x)+{d \over dx}(e^x)(\tan^{-1}(3x^2-2)) +{d \over dx}(\tan^{-1}(3x^2-2)(e^x)
		\\\\
		2.~& {d \over dx}\sin^{-1}(6x) = \frac{6}{\sqrt{1-(6x)^2}}
		\\\\
		3.~& -10{d \over dx}(2^x)= -10(2^x\ln2)
		\\\\
		4.~& {d \over dx}(\tan^{-1}(3x^2-2))) = \frac{6x}{1+(3x^2-2)^2}
		\\\\
		5.~& {dy \over dx} = \boxed{\frac{6}{\sqrt{1-(6x)^2}} -10(2^x\ln2) +e^xtan^{-1}(3x^2-2)+\frac{6x\cdot e^x}{1+(3x^2-2)^2}}
		\end{aligned}$$
		
    g) $f(x)=sec^{-1}(x^{2}-1+e^{2x})$
		$$\begin{aligned} 
		1.~& {dy \over dx} = \frac{1}{|x^2-1+e^{2x}|\sqrt{(x^2-1+e^{2x})^2-1}}\cdot{d \over dx}(x^2-1+e^{2x})
		\\\\
		2.~&{d \over dx}(x^2-1+e^{2x}) = 2x+2e^{2x}
		\\\\
		3.~& {dy\over dx} = \frac{2x+2e^{2x}}{|x^2-1+e^{2x}|\sqrt{(x^2-1+e^{2x})^2-1}}
		\end{aligned}$$

1.  Find $\frac{dy}{dx}$ for the equation $e^{2y}=3x~\sec y$
	$$\begin{aligned}
	1.~& {dy\over dx} = {d \over dx}(e^{2y})={d \over dx}(3x\sec y)
	\\\\
	2.~& {d \over dx}e^{2y}=2e^{2y}{dy \over dx}
	\\\\
	3.~& {d \over dx}(3x\sec y) = 3\sec y + 3x\sec y \tan y {dy \over dx}
	\\\\
	4.~& {dy \over dx} \to 2e^{2y}{dy \over dx} = 3\sec y + 3x\sec y \tan y {dy \over dx}
	\\\\
	5.~& {dy \over dx} \to 2e^{2y}{dy \over dx} -3x\sec y \tan y {dy \over dx} = 3 \sec y
	\\\\
	6.~& {dy \over dx} \to {dy \over dx}(2e^{2y}-3x\sec y\tan y) = 3\sec y
	\\\\
	7.~& {dy \over dx} = \boxed{\frac{3\sec y}{2e^{2y}-3x\sec y\tan y}}
	\end{aligned}$$

2.  Find the slope of $\sqrt{x}+2xy=3y$ at the point $(4,-\frac{2}{5})$.
	$$\begin{aligned}
	1.~& {dy \over dx} \Rightarrow {d \over dx}x^{1/2} +2\left({d \over dx}(x)y+{d \over dx}(y)x\right) = 3{d \over dx}y
	\\\\
	2.~& {dy \over dx} \Rightarrow \frac{1}{2\sqrt x} +2\left({d \over dx}(x)y+{d \over dx}(y)x\right) = 3{dy \over dx}
	\\\\
	3.~& 2{d \over dx}(x)y+2{d \over dx}(y)x = 2y+2x{dy \over dx}
	\\\\
	4.~& {dy \over dx} \Rightarrow \frac{1}{2\sqrt x} +2y+2x{dy \over dx} = 3{dy \over dx}
	\\\\
	5.~& {dy \over dx} \Rightarrow \frac{1}{2\sqrt x}+2y = 3{dy \over dx} -2x{dy \over dx}
	\\\\
	6.~& {dy \over dx} \Rightarrow \frac{1}{2\sqrt x}+2y = {dy \over dx}(3-2x)
	\\\\
	7.~& {dy \over dx} = \frac{\frac{1}{2\sqrt x}+2y}{3-2x}
	\\\\ &\text{pt } (4, -{2 \over 5}) \\\\
	8.~& m_{\tan} = \frac{\frac{1}{2\sqrt 4}+2({-2\over5})}{3-2(4)} = \frac{\frac{1}{4}-\frac{4}{5}}{3-8}
	\\\\
	9.~& m_{\tan}=\frac{\frac{5}{20}-\frac{16}{20}}{-5} = \frac{\frac{11}{20}}{5} = \boxed{{11\over100}}
	\end{aligned}$$

3.  A spherical snowball's radius is shrinking 0.25 cm each minute. How fast is the volume of the snowball changing when the radius is 6cm? Note: $V_{sphere}=\frac{4}{3}\pi r^{3}$
	$$\begin{aligned}
	{dr \over dt} &= -0.25 {\text{cm} \over \text{min}} \\\\
	{dV \over dt} &= {4\over3}\pi{d \over dt}(r^3) = {4\over3}\pi3r^2 {dr\over dt} \\\\
	{dV \over dt} &= 4\pi (6 ~\text{cm})^2(-0.25 {\text{cm} \over \text{min}}) \\\\
	{dV \over dt} &= 4\pi 36 ~\text{cm}^2(-0.25 {\text{cm} \over \text{min}}) \\\\
	{dV \over dt} &= \boxed{-36\pi {\text{cm}^3 \over \text{min}}}
	\end{aligned}$$

4.  A rocket launched vertically is tracked by a radar station located on the ground 3 miles from the launch site. What is the vertical speed of the rocket at the instant its distance from the radar station is 5 miles and this distance is increasing at the rate of 5000 mph?
	$$\begin{aligned}
	h &= 5~\text{miles} \quad\text{Hypotenuse}\\
	x &= 3 ~\text{miles} \quad\text{Horizontal distance (constant)}\\
	{dh \over dt} &= 5,000 \frac{\text{miles}}{\text{hour}} \quad\text{Rocket speed}\\
	y &= \text{Vertical height of the rocket} \\
	x^2+y^2 h^2 \quad&\Rightarrow\quad y^2=h^2-x^2 \quad\Rightarrow\quad y=\sqrt{h^2-x^2} \\
	y=&\sqrt{25-9} =\sqrt{16}= 4 
	\\\\\\
	1.~& {dy \over dt} \Rightarrow {d \over dt}(y^2)={d \over dt}(h^2)-{d \over dt}(9)
	\\\\
	2.~& {dy \over dt} \Rightarrow 2y{dy \over dt}=2h{dh \over dt}
	\\\\
	3.~& {dy \over dt} \Rightarrow 8 {dy \over dt} = 2(5 )(5,000 \frac{\text{miles}}{\text{hour}})
	\\\\
	4.~& {dy \over dt} = {50,000\over 8} \frac{\text{miles}}{\text{hour}} = \boxed{6,250 \frac{\text{miles}}{\text{hour}}}
	\end{aligned}$$

5.  Use a linear approximation to estimate $(3.05)^{2}$.
	$$\begin{aligned}
	y-y_1&=m(x-x_1) \\
	y&=y_1+m(x-x_1)\\
	L(x) &= f(a) +f'(a)(x-a) \\\\
	f(x) &= x^2\\
	a&=3 \\
	L(x) &= f(3)+f'(3)(x-3) \\
	L(x) &= 9+6(x-3) \\\\
	L(3.05)&= 9+6(3.05 -3) = \boxed{9.30}
	\end{aligned}$$

6.  Find $\Delta y$ and $dy$ and sketch a diagram showing $\Delta y$, $dy$ and $\Delta x=dx.$
    $y=x^{2}+1$ $x=1$ $dx=-0.2$

$\Delta y$ is the Actual Change in the $y$-value. The true difference in height on the curve when you move from the starting x value to the new x value
- Formula: $\Delta y = f(x_0+\Delta x)- f(x_0)$

$dy$ is the Estimated change in the $y$-value. It's the amount the height would change if you moved along the tangent line instead of the curve
- Formula: $dy = f'(x) \cdot dx$

7.  If possible, find the absolute max value and absolute min value of the following functions.
    a) $f(x)=\frac{1}{3}x^{3}+x^{2}-3x+1$ on the interval $[-4,4]$
		$$\begin{aligned}
		f'(x) &= x^2+2x-3 \\
		\text{critical points} &\Rightarrow x^2+2x-3=0 \\
		&\Rightarrow (x+3)(x-1)=0 \\
		&\Rightarrow x= -3,~ x= 1
		\\\\
		&\text{Identifdy candidates for min/max} \\
		1.~& \text{endpoints of interval} \\
		2.~& \text{Critical points within interval}
		\\\\
		&\text{Test all candidates} \\
		\min &= \min(f(-4), f(4), f(-3), f(1)) \\
		\max &= \max(f(-4), f(4), f(-3), f(1)) \\
		f(-4) &= -{64\over3}+29 \\
		f(4)  &= {64\over3}+5 \\
		f(1)  &= -{2\over3} \\            
		f(-3) &= 10  
		
		
		\end{aligned}$$

    b) $f(x)=-2\sqrt[3]{x}$ on the interval $-8\le x\le-1$.

8.  Find all critical numbers for the following functions.
    a) $f(x)=\frac{2x^{2}}{x+2}$
    b) $f(x)=x^{7/3}-28x^{1/3}$

9. Use the graph to identify the locations of all absolute maximums, absolute minimums, local maximums, and local maximums.
    a) **
    b) **
    c) **