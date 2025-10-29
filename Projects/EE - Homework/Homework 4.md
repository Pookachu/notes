13.1 (a, b)
Implement the function $F(A,B,C) = \Sigma m(1,3,5,6)$ using 
(a) an active high decoder and a single OR gate,

| A   | B   | C   | $m$ | F   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 1   | 1   |
| 0   | 1   | 0   | 2   | 0   |
| 0   | 1   | 1   | 3   | 1   |
| 1   | 0   | 0   | 4   | 0   |
| 1   | 0   | 1   | 5   | 1   |
| 1   | 1   | 0   | 6   | 1   |
| 1   | 1   | 1   | 7   | 0   |
$F=A'B'C + A'BC + AB'C  + ABC'$

Input A,B,C, into decoder, tie outputs 1,3,5,6, into the OR gate.

(b) an active-high decoder and a single NOR gate

Input A,B,C, into decoder, tie outputs 0,2,4,7, into the NOR gate.


13.2 (a, b)
Implement the function $F(A,B,C)=\Pi M(0,1,2,6)$ using 
(a) an active high decoder and a single OR gate,

| A   | B   | C   | $m$ | F   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 1   | 0   |
| 0   | 1   | 0   | 2   | 0   |
| 0   | 1   | 1   | 3   | 1   |
| 1   | 0   | 0   | 4   | 1   |
| 1   | 0   | 1   | 5   | 1   |
| 1   | 1   | 0   | 6   | 0   |
| 1   | 1   | 1   | 7   | 1   |
$F=A'BC+AB'C'+AB'C+ABC$
Input A,B,C, into decoder, tie outputs 3,4,5,7, into OR gate.

(b) an active high decoder and a single NOR gate

Input A,B,C, into decoder, tie outputs 0,1,2,6, into NOR gate


13.3 (a)
Implement the function $F(A,B,C,D) = \Sigma m(0,3,5,7,10,11,12,15)$ using
(a) two active high 3:8 decoders

| A   | B   | C   | D   | $m$ | F   |
| --- | --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   | 1   |
| 0   | 0   | 0   | 1   | 1   | 0   |
| 0   | 0   | 1   | 0   | 2   | 0   |
| 0   | 0   | 1   | 1   | 3   | 1   |
| 0   | 1   | 0   | 0   | 4   | 0   |
| 0   | 1   | 0   | 1   | 5   | 1   |
| 0   | 1   | 1   | 0   | 6   | 0   |
| 0   | 1   | 1   | 1   | 7   | 1   |
| 1   | 0   | 0   | 0   | 8   | 0   |
| 1   | 0   | 0   | 1   | 9   | 0   |
| 1   | 0   | 1   | 0   | 10  | 1   |
| 1   | 0   | 1   | 1   | 11  | 1   |
| 1   | 1   | 0   | 0   | 12  | 1   |
| 1   | 1   | 0   | 1   | 13  | 0   |
| 1   | 1   | 1   | 0   | 14  | 0   |
| 1   | 1   | 1   | 1   | 15  | 1   |

Decoder 1:
Inputs B,C,D, with A' as enable bit. Tie outputs 0,3,5,7 into into OR gate for F.

Decoder 2:
Inputs B,C,D, with A as enable bit, Tie outputs 2,3,4,7 into same OR gate for F.


13.14
Using the following **active-high** decoder and **NOR gates** to implement $f(a,b,c)=\Sigma m(2,5,6,7)$

| a   | b   | c   | $m$ | f   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 1   | 0   |
| 0   | 1   | 0   | 2   | 1   |
| 0   | 1   | 1   | 3   | 0   |
| 1   | 0   | 0   | 4   | 0   |
| 1   | 0   | 1   | 5   | 1   |
| 1   | 1   | 0   | 6   | 1   |
| 1   | 1   | 1   | 7   | 1   |
Input a,b,c, into decoder, tie outputs 0,1,3,4 into NOR gate for F.

12.1 (a, b)
Implement the following functions on 8:1 MUXes and on 4:1 MUXes:
(a) $F(A,B,C) = \Sigma _m(1,2,5,6,7)$

| A   | B   | C     | $m$ | F     |
| --- | --- | ----- | --- | ----- |
| 0   | 0   | **0** | 0   | **0** |
| 0   | 0   | **1** | 1   | **1** |
| 0   | 1   | **0** | 2   | **1** |
| 0   | 1   | **1** | 3   | **0** |
| 1   | 0   | **0** | 4   | **0** |
| 1   | 0   | **1** | 5   | **1** |
| 1   | 1   | **0** | 6   | **1** |
| 1   | 1   | **1** | 7   | **1** |
Using A and B as select lines, and C as input

| Input # | Variable |
| ------- | -------- |
| 0       | C        |
| 1       | C'       |
| 2       | GND      |
| 3       | PWR      |

For 8:1 MUX, add GND to Most Significant Bit select line, and GND for inputs 4-7

(b)  $F(A,B,C) = \Pi _M(0,1,4,7)$

| A   | B   | C   | $m$ | F   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 1   | 0   |
| 0   | 1   | 0   | 2   | 1   |
| 0   | 1   | 1   | 3   | 1   |
| 1   | 0   | 0   | 4   | 0   |
| 1   | 0   | 1   | 5   | 1   |
| 1   | 1   | 0   | 6   | 1   |
| 1   | 1   | 1   | 7   | 0   |
Using A and B as select lines, and C as input

| Input # | Variable |
| ------- | -------- |
| 0       | GND      |
| 1       | PWR      |
| 2       | C        |
| 3       | C'       |

For 8:1 MUX, add GND to Most Significant Bit select line, and GND for inputs 4-7

12.2 (a, b)
Implement the following functions on 16:1 MUXes and on 8:1 MUXes
(a) $F(A,B,C,D) = \Sigma_m (1,5,6,7,11,12,14)$

| A   | B   | C   | D   | $m$ | F     |
| --- | --- | --- | --- | --- | ----- |
| 0   | 0   | 0   | 0   | 0   | $0_0$ |
| 0   | 0   | 0   | 1   | 1   | $1_0$ |
| 0   | 0   | 1   | 0   | 2   | $0_1$ |
| 0   | 0   | 1   | 1   | 3   | $0_1$ |
| 0   | 1   | 0   | 0   | 4   | $0_2$ |
| 0   | 1   | 0   | 1   | 5   | $1_2$ |
| 0   | 1   | 1   | 0   | 6   | $1_3$ |
| 0   | 1   | 1   | 1   | 7   | $1_3$ |
| 1   | 0   | 0   | 0   | 8   | $0_4$ |
| 1   | 0   | 0   | 1   | 9   | $0_4$ |
| 1   | 0   | 1   | 0   | 10  | $0_5$ |
| 1   | 0   | 1   | 1   | 11  | $1_5$ |
| 1   | 1   | 0   | 0   | 12  | $1_6$ |
| 1   | 1   | 0   | 1   | 13  | $0_6$ |
| 1   | 1   | 1   | 0   | 14  | $1_7$ |
| 1   | 1   | 1   | 1   | 15  | $0_7$ |

For 16:1 MUX, use ABCD for select lines

| Input # | Variable |
| ------- | -------- |
| 0       | $0$      |
| 1       | $1$      |
| 2       | $0$      |
| 3       | $0$      |
| 4       | $0$      |
| 5       | $1$      |
| 6       | $1$      |
| 7       | $1$      |
| 8       | $0$      |
| 9       | $0$      |
| 10      | $0$      |
| 11      | $1$      |
| 12      | $1$      |
| 13      | $0$      |
| 14      | $1$      |
| 15      | $0$      |

For 8:1 MUX, use ABC as select lines

| Input # | Variable |
| ------- | -------- |
| 0       | D        |
| 1       | 0        |
| 2       | D        |
| 3       | 1        |
| 4       | 0        |
| 5       | D        |
| 6       | D'       |
| 7       | D'       |

(b) $F(A,B,C,D)=\Pi _M(3,4,7,8,10,12,13,14)$

| A   | B   | C   | D   | $m$ | F     | D   |
| --- | --- | --- | --- | --- | ----- | --- |
| 0   | 0   | 0   | 0   | 0   | $1_0$ | 0   |
| 0   | 0   | 0   | 1   | 1   | $1_0$ | 1   |
| 0   | 0   | 1   | 0   | 2   | $1_1$ | 0   |
| 0   | 0   | 1   | 1   | 3   | $0_1$ | 1   |
| 0   | 1   | 0   | 0   | 4   | $0_2$ | 0   |
| 0   | 1   | 0   | 1   | 5   | $1_2$ | 1   |
| 0   | 1   | 1   | 0   | 6   | $1_3$ | 0   |
| 0   | 1   | 1   | 1   | 7   | $0_3$ | 1   |
| 1   | 0   | 0   | 0   | 8   | $0_4$ | 0   |
| 1   | 0   | 0   | 1   | 9   | $1_4$ | 1   |
| 1   | 0   | 1   | 0   | 10  | $0_5$ | 0   |
| 1   | 0   | 1   | 1   | 11  | $1_5$ | 1   |
| 1   | 1   | 0   | 0   | 12  | $0_6$ | 0   |
| 1   | 1   | 0   | 1   | 13  | $0_6$ | 1   |
| 1   | 1   | 1   | 0   | 14  | $0_7$ | 0   |
| 1   | 1   | 1   | 1   | 15  | $1_7$ | 1   |

For 16:1 MUX, use ABCD as select lines

| Input # | Variable |
| ------- | -------- |
| 0       | $1$      |
| 1       | $1$      |
| 2       | $1$      |
| 3       | $0$      |
| 4       | $0$      |
| 5       | $1$      |
| 6       | $1$      |
| 7       | $0$      |
| 8       | $0$      |
| 9       | $1$      |
| 10      | $0$      |
| 11      | $1$      |
| 12      | $0$      |
| 13      | $0$      |
| 14      | $0$      |
| 15      | $1$      |

For 8:1 MUX, use ABC as select lines

| Input # | Variable |
| ------- | -------- |
| 0       | 1        |
| 1       | D'       |
| 2       | D        |
| 3       | D'       |
| 4       | D        |
| 5       | D        |
| 6       | 0        |
| 7       | D        |

12.3
Implement the function $F(A,B,C) = \Sigma _m(2,3,4,6)$ on a 4:1 MUX. However, reduce the variable A instead of the variable C. That is, make B and C the control inputs to the MUX.

| A   | B   | C   | $m$ | F     | A     |
| --- | --- | --- | --- | ----- | ----- |
| 0   | 0   | 0   | 0   | $0_0$ | $0_0$ |
| 0   | 0   | 1   | 1   | $0_1$ | $0_1$ |
| 0   | 1   | 0   | 2   | $1_2$ | $0_2$ |
| 0   | 1   | 1   | 3   | $1_3$ | $0_3$ |
| 1   | 0   | 0   | 4   | $1_0$ | $1_0$ |
| 1   | 0   | 1   | 5   | $0_1$ | $1_1$ |
| 1   | 1   | 0   | 6   | $1_2$ | $1_2$ |
| 1   | 1   | 1   | 7   | $0_3$ | $1_3$ |

Using B and C as the control lines,

| Input # | Variable |
| ------- | -------- |
| 0       | A        |
| 1       | 0        |
| 2       | 1        |
| 3       | A'       |


12.3 (but use A and C as the control lines) 

| A   | B   | C   | $m$ | F     | B   |
| --- | --- | --- | --- | ----- | --- |
| 0   | 0   | 0   | 0   | $0_0$ | $0_0$ |
| 0   | 0   | 1   | 1   | $0_1$ | $0_1$ |
| 0   | 1   | 0   | 2   | $1_0$ | $1_0$ |
| 0   | 1   | 1   | 3   | $1_1$ | $1_1$ |
| 1   | 0   | 0   | 4   | $1_2$ | $0_2$ |
| 1   | 0   | 1   | 5   | $0_3$ | $0_3$ |
| 1   | 1   | 0   | 6   | $1_2$ | $1_2$ |
| 1   | 1   | 1   | 7   | $0_3$ | $1_3$ |

Using A, and C as the control lines,

| Input # | Variable |
| ------- | -------- |
| 0       | B        |
| 1       | B        |
| 2       | 1        |
| 3       | 0        |
