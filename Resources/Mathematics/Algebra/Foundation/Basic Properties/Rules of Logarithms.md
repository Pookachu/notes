---
aliases:
  - Logarithm
---
#### Anatomy of a logarithm
> A logarithm is the inverse operation of exponentiation. It answers the question: **"What exponent do I need to raise the base to in order to get a certain number?"**

**The relationship is expressed like this:**
	If $b^y =x$, then $log_b(x) = y$
	- $b$ is the **base**.
	- $y$ is the **exponent** (or the logarithm).
	- x is the **argument**,

**Example:** Since $2^3 = 8$, the logarithmic form is $log_2(8) = 3$

--- 
 #### **Special Logarithms**
 > There are two special logarithms that have their own notation:
- **Common Logarithm**: This is a logarithm with base 10. It's written as $log(x)$, so the base 10 is implied.
- **Natural Logarithm**: This is a logarithm with base $e$ ([[Euler's number]], approx. $2.718). It's written as $\ln(x)$. 

---
#### **Properties of Logarithms**
> These rules are crucial for manipulating and simplifying logarithmic expressions.

| Property             | Formula                                                  | Example                                                                |
| :------------------- | :------------------------------------------------------- | :--------------------------------------------------------------------- |
| **Product Rule**     | $\log_b(xy) = \log_b(x) + \log_b(y)$                     | $\log_2(8 \cdot 16) = \log_2(8) + \log_2(16) = 3 + 4 = 7$              |
| **Quotient Rule**    | $\log_b\left(\frac{x}{y}\right) = \log_b(x) - \log_b(y)$ | $\log_3\left(\frac{81}{3}\right) = \log_3(81) - \log_3(3) = 4 - 1 = 3$ |
| **Power Rule**       | $\log_b(x^y) = y \cdot \log_b(x)$                        | $\log_4(16^3) = 3 \cdot \log_4(16) = 3 \cdot 2 = 6$                    |
| **Change of Base**   | $\log_b(x) = \frac{\log_c(x)}{\log_c(b)}$                | $\log_3(7) = \frac{\ln(7)}{\ln(3)} \approx 1.77$                       |
| **Identity Rule**    | $\log_b(b) = 1$                                          | $\log_5(5) = 1$                                                        |
| **Zero Rule**        | $\log_b(1) = 0$                                          | $\ln(1) = 0$                                                           |
| **Inverse Property** | $\log_b(b^x) = x$ and $b^{\log_b(x)} = x$                | $10^{\log(5)} = 5$                                                     |

---
### **Solving Logarithmic Equations**
> Here are the primary strategies for solving equations involving logarithms.

1. **Isolate the Logarithm and Convert to Exponential Form**
> If the equation has a single logarithm, get it by itself on one side and then rewrite the equation in exponential form. 

**Example:** 
	Solve $log_4(x+3)=2$ 
	1. **Isolate the log:** the log is already isolated
	2. **Convert to exponential form:** $4^2 = x +3$
	3. **Solve for $x$ :
		$16=x+3$
		$x=13$

2. **Use the One-to-One Property**
> If you have a single logarithm with the same base on both sides of the equation, you can set their arguments equal to each other.

If $log_b(x) = log_b(y)$, then $x=y$. 

**Example:**
	Solve $\ln(3x -1) = \ln(x+5)$
		1. **Set the arguments equal:** $3x -1 = x +5$
		2. **Solve for $x$**
			$2x=6$
			$x=3$ 

---
**Important Note:** 
> You must always check your answers in the original equation. Logarithms are only defined for positive arguments, so any solution that results in taking the log of a negative number or zero is an extraneous solution and must be discarded.