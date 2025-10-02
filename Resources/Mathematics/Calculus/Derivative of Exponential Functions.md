The derivative of $a^x$:
$$\begin{aligned}
\frac{d}{dx}a^x &= \lim_{h\to0}\frac{a^{x+h}-a^x}{h} \\
&=\lim_{h\to0}\frac{a^x\cdot a^h-a^x}{h} \\
&=\lim_{h\to0}a^x\cdot\frac{a^h-1}{h} \\
&=a^x\lim_{h\to0}\frac{a^h-1}{h} \\
&=\left(\lim_{h\to0}\frac{a^h-1}{h} \right)\cdot a^x \\\\
&\left(\lim_{h\to0}\frac{a^h-1}{h} \right)= L \\\\
\frac{d}{dx}a^x &= La^x
\end{aligned}$$