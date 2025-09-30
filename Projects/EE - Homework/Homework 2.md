
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

2. 2.12  
A majority function will be 1 when an input contains more 1’s than 0’s in its
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
Use the rules of Boolean Algebra to simplify the following expressions.

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
Use factoring to simplify the following Boolean expressions given in canonical form.

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
> $\to\quad ABD(\bar CC) +B\bar C\bar D(\bar AA)+\bar A\bar CD(B\bar B)$
> $\to\quad ABD+B\bar C\bar D+\bar A\bar CD$

6. 3.1(a)
For each of the following logic functions, write the truth table and the SOP
and POS canonical forms.
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

$\Sigma_m = \boxed{a\bar b\bar c+ab\bar c+abc}$
$\Pi_M = \boxed{(a+b+c)(a+b+\bar c)(a+\bar b+c)(a+\bar b+\bar c)(\bar a+\bar b+c)}$

6. 3.3
Give the canonical SOP form of the logic function $F(A, B, C) = \Sigma_M (1, 2, 5, 6, 7)$

| $A$ | $B$ | $C$ |     | $F$ |
| --- | --- | --- | --- | --- |
| $0$ | $0$ | $0$ |     | 0   |
| $0$ | $0$ | $1$ |     | 1   |
| $0$ | $1$ | $0$ |     | 1   |
| $0$ | $1$ | $1$ |     | 0   |
| $1$ | $0$ | $0$ |     | 0   |
| $1$ | $0$ | $1$ |     | 1   |
| $1$ | $1$ | $0$ |     | 1   |
| $1$ | $1$ | $1$ |     | 1   |

$F = \boxed{\bar A\bar BC+\bar AB\bar C+A\bar BC+AB\bar C+ABC}$

7. 3.5 
Give the SOP form of the function $F(A, B, C) =\Pi_M(0, 1, 5, 6, 7)$

| $A$ | $B$ | $C$ |     | $F$ |
| --- | --- | --- | --- | --- |
| $0$ | $0$ | $0$ |     | 0   |
| $0$ | $0$ | $1$ |     | 0   |
| $0$ | $1$ | $0$ |     | 1   |
| $0$ | $1$ | $1$ |     | 1   |
| $1$ | $0$ | $0$ |     | 1   |
| $1$ | $0$ | $1$ |     | 0   |
| $1$ | $1$ | $0$ |     | 0   |
| $1$ | $1$ | $1$ |     | 0   |
$F= \boxed{\bar A B \bar C + \bar A BC + A \bar B \bar C}$

7. 3.17(assume F(a,b,c))
If $F = \Sigma_m(0, 2, 3, 6, 7)$, find the algebraic SOP form of $\bar F$.

| $A$ | $B$ | $C$ |     | $F$ | $\bar F$ |                 |
| --- | --- | --- | --- | --- | -------- | --------------- |
| $0$ | $0$ | $0$ |     | 1   | 0        |                 |
| $0$ | $0$ | $1$ |     | 0   | 1        | $\bar A\bar BC$ |
| $0$ | $1$ | $0$ |     | 1   | 0        |                 |
| $0$ | $1$ | $1$ |     | 1   | 0        |                 |
| $1$ | $0$ | $0$ |     | 0   | 1        | $A\bar B\bar C$ |
| $1$ | $0$ | $1$ |     | 0   | 1        | $A\bar BC$      |
| $1$ | $1$ | $0$ |     | 1   | 0        |                 |
| $1$ | $1$ | $1$ |     | 1   | 0        |                 |
$F= \boxed{\bar A\bar BC+A\bar B\bar C+A\bar BC}$

8. 3.21 (just draw the truth table and write as a sum of minterms)
There are four adjacent parking spots in a particular parking area. There is a
sensor mounted on each spot whose output is equal to $0$ when a car is
occupying the spot and equal to $1$ otherwise (Note: we call this “active low”
logic because logic-0 is asserted when something happens). Design a
decoding system which will generate a $0$ output if and only if there are two
or more adjacent vacant spots available. Draw the truth table for this problem.
Include a diagram of the parking spots labeled with the variables you use in
your truth table. Find the canonical SOP form for your logic function.

| $x_3$ | $x_2$ | $x_1$ | $x_0$ | $F$ |
| ----- | ----- | ----- | ----- | --- |
| $0$   | $0$   | $0$   | $0$   | 1   |
| $0$   | $0$   | $0$   | $1$   | 1   |
| $0$   | $0$   | $1$   | $0$   | 1   |
| $0$   | $0$   | $1^*$ | $1^*$ | 0   |
| $0$   | $1$   | $0$   | $0$   | 1   |
| $0$   | $1$   | $0$   | $1$   | 1   |
| $0$   | $1^*$ | $1^*$ | $0$   | 0   |
| $0$   | $1$   | $1^*$ | $1^*$ | 0   |
| $1$   | $0$   | $0$   | $0$   | 1   |
| $1$   | $0$   | $0$   | $1$   | 1   |
| $1$   | $0$   | $1$   | $0$   | 1   |
| $1$   | $0$   | $1^*$ | $1^*$ | 0   |
| $1^*$ | $1^*$ | $0$   | $0$   | 0   |
| $1^*$ | $1^*$ | $0$   | $1$   | 0   |
| $1^*$ | $1^*$ | $1$   | $0$   | 0   |
| $1^*$ | $1^*$ | $1$   | $1$   | 0   |
$F=\Sigma_m(0,1,2,4,5,8,9,10)$