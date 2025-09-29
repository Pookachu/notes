
1. 2.9
The control unit in a computer needs to activate an active-high signal $s_1$ when
the three-bit opcode (given by $x_2x_1x_0$ ) is $100$ and $110$ and it needs to activate
an active-low signal $s_2$ when the three-bit opcode is $011$ or $101$. Write Boolean
equations for each signal.

| $x_2$ | $x_1$ | $x_0$ | $m$ | $s_1$ | $s_2$ |
| ----- | ----- | ----- | --- | ----- | ----- |
| 0     | 0     | 0     | 0   | 0     | 1     |
| 0     | 0     | 1     | 1   | 0     | 1     |
| 0     | 1     | 0     | 2   | 0     | 1     |
| 0     | 1     | 1     | 3   | 0     | 0     |
| 1     | 0     | 0     | 4   | 1     | 1     |
| 1     | 0     | 1     | 5   | 1     | 0     |
| 1     | 1     | 0     | 6   | 0     | 1     |
| 1     | 1     | 1     | 7   | 0     | 1     |
$s_1(x_0, x_1, x_2) = \Sigma _m(4,5)$
$s_2(x_0, x_1, x_2) \Pi _M(3,5)$

| $\boxed{s_1}$ | $x_2, x_1$ | $x_2, x_1$ | $x_2, x_1$ | $x_2, x_1$  |
| ------------- | ---------- | ---------- | ---------- | ----------- |
| $x_0$         | **00**     | **01**     | **11**     | **10**      |
| **0**         | 0          | 0          | 0          | $\boxed{1}$ |
| **1**         | 0          | 0          | 0          | $\boxed1$   |

$s_1 = x_0\;\bar{x_1}$   

| $\boxed{s_2}$ | $x_2, x_1$      | $x_2, x_1$  | $x_2, x_1$      | $x_2, x_1$  |
| ------------- | --------------- | ----------- | --------------- | ----------- |
| $x_0$         | **00**          | **01**      | **11**          | **10**      |
| **0**         | $\boxed1_{1,2}$ | $\boxed1_1$ | $\boxed1_{1,3}$ | $\boxed1_1$ |
| **1**         | $\boxed1_2$     | 0           | $\boxed1_3$     | 0           |
$s_2 = \bar{x_0} + \bar{x_2}\bar{x_1} + x_1 x_2$ 

2. 2.12  A majority function will be 1 when an input contains more 1’s than 0’s in its
representation.
Write the Boolean equation for the output F of a majority function which takes
a 4-bit input $x_3\;x_2\;x_1\;x_0$.

| $x_3$ | $x_2$ | $x_1$ | $x_0$ | $F$ | $m$  |
| ----- | ----- | ----- | ----- | --- | ---- |
| $0$   | $0$   | $0$   | $0$   | $0$ | $0$  |
| $0$   | $0$   | $0$   | $1$   | $0$ | $1$  |
| $0$   | $0$   | $1$   | $0$   | $0$ | $2$  |
| $0$   | $0$   | $1$   | $1$   | $0$ | $3$  |
| $0$   | $1$   | $0$   | $0$   | $0$ | $4$  |
| $0$   | $1$   | $0$   | $1$   | $0$ | $5$  |
| $0$   | $1$   | $1$   | $0$   | $0$ | $6$  |
| $0$   | $1$   | $1$   | $1$   | $1$ | $7$  |
| $1$   | $0$   | $0$   | $0$   | $0$ | $8$  |
| $1$   | $0$   | $0$   | $1$   | $0$ | $9$  |
| $1$   | $0$   | $1$   | $0$   | $0$ | $10$ |
| $1$   | $0$   | $1$   | $1$   | $1$ | $11$ |
| $1$   | $1$   | $0$   | $0$   | $0$ | $12$ |
| $1$   | $1$   | $0$   | $1$   | $1$ | $13$ |
| $1$   | $1$   | $1$   | $0$   | $1$ | $14$ |
| $1$   | $1$   | $1$   | $1$   | $1$ | $15$ |
$f=\Sigma_m(7,11,13,14,15)$

| $f$        | $x_3, x_2$ | $x_3, x_2$    | $x_3, x_2$            | $x_3, x_2$    |
| ---------- | ---------- | ------------- | --------------------- | ------------- |
| $x_1, x_0$ | $00$       | $01$          | $11$                  | $10$          |
| $00$       | $0$        | $0$           | $0$                   | $0$           |
| $01$       | $0$        | $0$           | $\boxed{1}_1$         | $0$           |
| $11$       | $0$        | $\boxed{1}_4$ | $\boxed{1}_{1,2,3,4}$ | $\boxed{1}_2$ |
| $10$       | $0$        | $0$           | $\boxed{1}_3$         | $0$           |
$f = x_3 x_2 x_0 + x_3 x_1 x_0 + x_3 x_2 x_1 + x_2 x_1 x_0$

3. 2.15(a,b,c)
Use the rules of Boolean Algebra to simplify the following expressions.
**a)** --- $A(B+\bar A C)$
> $= AB+A\bar A C \quad=\quad AB+0 \quad=\quad \boxed{AB}$
  
**b)** --- $A\overline{(A+B)} +C + \overline{(A+C})$
>$\to\quad \overline{(A+B)} = \overline{AB}$ and $\overline{(A+C)} = \overline{AC}$
>$\to\quad A(\overline{AB})+C+\overline{AC} \quad=\quad 0\bar{B}+C+\overline{AC} \quad=\quad C+\overline{AC}$
>$\to\quad \boxed{\bar{A}+C}$

**c)** --- $X+W\bar{X}\bar{Y}$
> $\to\quad \boxed{X+W\bar{Y}}$

4. 2.15(d,e,f)
**d)** --- $\overline{ABC}+\overline{\bar{B}\bar{C}}$
>$\to\quad \overline{ABC} + B + C$
>$\to\quad \bar{A} + \bar{B} + \bar{C} + B + C$
>$\to\quad \bar{A}+1+1 \quad=\quad \boxed{1}$

**e)** --- $\bar{X}Y+\bar{Y}+W(Z+\bar{W}X)$
>$\to\quad \bar{X}Y+\bar{Y}+WZ+W\bar{W}X$
>$\to\quad \bar{X}Y+\bar{Y} + WZ +0$
>$\to\quad \bar{X}Y+\bar{Y} + WZ$
>$\to\quad \boxed{\bar{X}+\bar{Y} + WZ}$

**f)** --- $ab+a\bar{b}+\bar{a}\bar{b}$
> $\to\quad (ab + a\bar{b})+(a\bar{b}+\bar{a}\bar{b})$
> $\to\quad a(b+\bar{b})+\bar{b}(a+\bar{a})$
> $\to\quad \boxed{a+\bar{b}}$

5. 2.16
**a)** --- $\bar{x}yz+\bar{x}y\bar{z}+xyz$
> $\to\quad yz(x+\bar{x})+\bar{x}y\bar{z}$
> $\to\quad yz+\bar{x}y\bar{z}$
> $\to\quad y(z+\bar{x}\bar{z})$
> $\to\quad y(z+\bar{x})$
> $\to\quad \boxed{yz+y\bar{x}}$

**b)** --- $\bar{A}\bar{B}\bar{C}+A\bar{B}C+ABC+AB\bar{C}$
> $\to\quad AB(C+\bar{C})+\bar{A}\bar{B}\bar{C}+A\bar{B}C$
> $\to\quad AB+\bar{A}\bar{B}\bar{C}+A\bar{B}C$
> $\to\quad \boxed{AB+\bar{A}\bar{B}\bar{C}+AC}$ (consensus term)

**c)** --- $\bar{A}\bar{B}C+\bar{A}B\bar{C}+A\bar{B}C+AB\bar{C}$
> $\to\quad B\bar C(\bar A +A)+\bar A\bar BC+A\bar BC$
> $\to\quad B\bar C+\bar A\bar BC+A\bar BC$
> $\to\quad B\bar C+\bar BC(\bar A+A)$
> $\to\quad \boxed{B\bar C+\bar BC}$

**d)** --- $\bar A\bar B\bar CD+\bar AB\bar C\bar D+AB\bar C\bar D+\bar AB\bar CD+AB\bar CD+ABCD$
        1              2                   3                  4                  5                  6
		5 6                        2 3                      1 4
> $\to\quad ABD(\bar CC) +B\bar C\bar D(\bar AA)+\bar A\bar CD(B\bar B)$
> $\to\quad ABD+B\bar C\bar D+\bar A\bar CD$

6. 3.1(a)
a) $F(a, b, c) = ab+a\bar c(b+\bar c)$

| $a$ | $b$ | $c$ |     | $ab$ | $b+\bar c$ | $a\bar c$ | $a\bar c(b+\bar c)$ | $F$ |
| --- | --- | --- | --- | ---- | ---------- | --------- | ------------------- | --- |
| $0$ | $0$ | $0$ |     | $0$  | $1$        | $0$       | $0$                 | $0$ |
| $0$ | $0$ | $1$ |     | $0$  | $0$        | $0$       | $0$                 | $0$ |
| $0$ | $1$ | $0$ |     | $0$  | $1$        | $0$       | $0$                 | $0$ |
| $0$ | $1$ | $1$ |     | $0$  | $1$        | $0$       | $0$                 | $0$ |
| $1$ | $0$ | $0$ |     | $0$  | $1$        | $1$       | $1$                 | $1$ |
| $1$ | $0$ | $1$ |     | $0$  | $0$        | $0$       | $0$                 | $0$ |
| $1$ | $1$ | $0$ |     | $1$  | $1$        | $1$       | $1$                 | $1$ |
| $1$ | $1$ | $1$ |     | $1$  | $1$        | $0$       | $0$                 | $1$ |

$\Sigma_m = a\bar b\bar c+ab\bar c+abc$
$\Pi_M = (a+b+c)(a+b+\bar c)(a+\bar b+c)(a+\bar b\bar c)(\bar a\bar bc)$

6. 3.3
Give the canonical SOP form of the logic function $F(A, B, C) = \Sigma_M (1, 2, 5, 6, 7)$

| $a$ | $b$ | $c$ |     | F   |
| --- | --- | --- | --- | --- |
| $0$ | $0$ | $0$ |     | 0   |
| $0$ | $0$ | $1$ |     | 1   |
| $0$ | $1$ | $0$ |     | 1   |
| $0$ | $1$ | $1$ |     | 0   |
| $1$ | $0$ | $0$ |     | 0   |
| $1$ | $0$ | $1$ |     | 1   |
| $1$ | $1$ | $0$ |     | 1   |
| $1$ | $1$ | $1$ |     | 1   |

$\Sigma_m = \bar a\bar bc+\bar ab\bar c+a\bar bc+ab\bar c+abc$

7. 3.5
8. 3.17(assume F(a,b,c))
9. 3.21 (just draw the truth table and write as a sum of minterms)