
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
a) - $A(B+\bar A C)$
> $= AB+A\bar A C \quad=\quad AB+0 \quad=\quad \boxed{AB}$
  
b) - $A\overline{(A+B)} +C + \overline{(A+C})$
> $\overline{(A+B)} = \overline{AB}$ and $\overline{(A+C)} = \overline{AC}$
>$A(\overline{AB})+C+\overline{AC} = 0\bar{B}+C+\overline{AC} = $




c)

4. 2.15(d,e,f)
5. 2.16
6. 3.1(a)
7. 3.3
8. 3.5
9. 3.17(assume F(a,b,c))
10. 3.21 (just draw the truth table and write as a sum of minterms)