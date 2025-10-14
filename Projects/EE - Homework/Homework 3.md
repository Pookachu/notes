**Problem 4.4**
Write the logic function $F = AB +\bar B \bar C$ in canonical SOP and minimal sum forms.

$F= AB(C+\bar C) + \bar B \bar C (A + \bar A)$
$= ABC + AB\bar C + A\bar B\bar C + \bar A\bar B\bar C$
$= AB+ \bar B \bar C$


**Problem 4.5**
Write the the logic function $F = \Pi_{A,B,C}(0,1,3,6)$ in canonical POS and minimal product forms.

|     | AB  |     |     |     |
| --- | --- | --- | --- | --- |
| C   | 00  | 01  | 11  | 10  |
| 0   | 0   | 1   | 0   | 1   |
| 1   | 0   | 0   | 1   | 1   |
$F = (A+B+C) (A+B+\bar C) (A+\bar B + \bar C) (\bar A+\bar B+ C)$
$F = A\bar B + AC + \bar A B \bar C$
$F= (A+B)(A+\bar C)(\bar A + \bar B + C)$


**Problem 4.6**
Write $F=\sum_{A,B,C,D}(0,2,5,8,10,13) + X(4,6,7,9,14)$ in a K-map and solve for the minimal sum form.

|     | AB            |               |               |               |
| --- | ------------- | ------------- | ------------- | ------------- |
| CD  | 00            | 01            | 11            | 10            |
| 00  | $\boxed{1}_0$ | $\boxed X _1$ | $0$           | $\boxed{1}_0$ |
| 01  | $0$           | $\boxed{1}_1$ | $\boxed 1 _2$ | $\boxed X _2$ |
| 11  | $0$           | $\boxed X _1$ | $0$           | $0$           |
| 10  | $\boxed{1}_0$ | $\boxed X _1$ | $X$           | $\boxed{1}_0$ |
$= \bar B \bar C + \bar A B + A \bar C D$


**Problem 4.8**
Use Boolean Algebra to reduce $F = \overline{\overline{A+B} (\overline{AC} \oplus D)}$ to minimal SOP form. Also draw up the K-map for this function and find the SOP form from that as well. Your answer should be the same for both methods

$F = (A+B)''+(A'C'\oplus D)'$
$=(A+B) +(A'C'D+(A'C')'D')$
$= A+B+\bar A D + \bar C D + AC \bar D$
$=A+B+D$

|     | AB    |           |             |           |
| --- | ----- | --------- | ----------- | --------- |
| CD  | 00    | 01        | 11          | 10        |
| 00  | $0_0$ | $1_2$     | $1_{1,2}$   | $1_1$     |
| 01  | $1_0$ | $1_{0,2}$ | $1_{0,1,2}$ | $1_{0,1}$ |
| 11  | $1_0$ | $1_{0,2}$ | $1_{0,1,2}$ | $1_{0,1}$ |
| 10  | $0_0$ | $1_2$     | $1_{1,2}$   | $1_1$     |
$=A+B+D$


**Problem 4.27**
Find the NAND-NAND implementation of the logic function $F= (\bar A + B) (\bar C + D)$.

|     | AB  |     |     |     |
| --- | --- | --- | --- | --- |
| CD  | 00  | 01  | 11  | 10  |
| 00  | 1   | 1   | 1   | 0   |
| 01  | 1   | 1   | 1   | 0   |
| 11  | 1   | 1   | 1   | 0   |
| 10  | 0   | 0   | 0   | 0   |

$=\bar A \bar C + \bar A D + B\bar C + BD$

$=\overline{\overline{(\bar A \bar C + \bar A D + B\bar C + BD)}}$

$= \overline{(\overline{(\bar A \bar C)} \cdot \overline{(\bar A D)} \cdot \overline{(B\bar C)} \cdot \overline{(BD)})}$


**Problem 4.28**
Find the NOR-NOR implementation of the logic function $F= \bar A BC + C \bar D$

|     | AB  |     |     |     |
| --- | --- | --- | --- | --- |
| CD  | 00  | 01  | 11  | 10  |
| 00  | 0   | 0   | 0   | 0   |
| 01  | 0   | 0   | 0   | 0   |
| 11  | 0   | 1   | 0   | 0   |
| 10  | 1   | 1   | 1   | 1   |

$= (C)(\bar A+ \bar D)(B+\bar D)$

$= \overline{\overline{(C)(\bar A+ \bar D)(B+\bar D)}}$

$= \overline{\overline{(C)} + \overline{(\bar A+ \bar D)} + \overline{(B+\bar D)}}$

**Problem 6.1**
Implement an XNOR (exclusive-NOR) gate using only NAND gates. That is, draw the gate-level logic diagram for an XNOR function using only NAND gates.
![[Drawing 2025-10-13 11.32.16.excalidraw]]

**Problem 6.5**
Draw a logic diagram using only NOR and NOT gates that will perform the 3-input AND function.
$ABC = (A'+B'+C')'$
![[Drawing 2025-10-13 11.36.56.excalidraw]]

**Problem 6.10**
Implement the following logic function using only NAND gates: $F= \overline{AB} +C(A \oplus B)$

$= (\bar A + \bar B) +C(A\bar B+\bar A B)$
$= \bar A + \bar B +A\bar B C+ \bar A B C)$
$= \bar A + \bar B = \overline{AB}$ 

**Problem 6.15**
Find the minimal NAND gate realization of the logic function $F= \bar A B + \bar B C$. Show the algebraic formulation as well as the gate-level implementation.

$= (\bar A B + \bar B C)''$
$= \overline{(\bar A B)} \cdot \overline{(\bar B C)}$

![[Drawing 2025-10-13 11.49.09.excalidraw]]