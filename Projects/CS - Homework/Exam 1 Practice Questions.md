> Note: The following is a list of questions related to concepts that we have covered in class. This list is not exhaustive, so the exam might have questions not listed here.
1. **What is OO programming?**
Object Oriented programming is a style of programming that revolves around classes and objects and their interactions between each other which are managed by 'getters' and 'setters.'

2. **What is the difference between a class and an object? Show code explaining the**
**difference.**
A class is a blueprint to construct an object that details what fields (attributes) and methods (behaviors) that each instances will require to define on initialization.
```java
// This is a class. It details what sort of attributes 
public class BouncyBall {
	//attributes (fields)
	int bouncyness;
	int size;
	
	//constructor (to initialize the class as an object)
	public BouncyBall(int bouncyness, int size) {
		this.bouncyness = bouncyness;
		this.size = size;
	}
	//behavior (method)
	public void bounce() {
		System.out.println("i am this big: "     + this.size);
		System.out.println("bounced this high: " + this.bouncyness);
	}
}

//This is an example of initializing an object from a class.
public static main(string[] args) {

	//     \/---- new keyword to make an object with a class' constructor  
	ball = new BouncyBall(10, 1 ); // 10 = bouncyness, and 1 = size
	ball.bounce();
}
```

3. **What are the JRE, JDK, JVM? Explain in depth.**
**JRE**: The **J**ava **R**untime **E**nvironment provides a space for java programs to function.  It contains common libraries for programs to use when they run, and it contains the JVM to actually run java bytecode.

**JDK**: The **J**ava **D**evelopment **K**it contains tools and libraries for developers writing Java programs. It has debuggers, compilers and documentation generation tools.

**JVM**: The **J**ava **V**irtual **M**achine actually processes Java programs 

4. **What is a compiler? What does it do?**
5. **What does it mean Write-once Run-Everywhere?**
6. **Explain the Von Neumann architecture.**
7. **Write down a simple Java program that prints a message to the command line.**
8. **What is the difference between declaring and initializing a variable in Java?**
9. **What is a constructor in Java?**
10. **What is the default constructor in Java?**
11. **What happens in Java to the default constructor if you define another constructor for that**
**same class? Explain.**
12. **Write Java code showing a class with a constructor initializing an attribute.**
13. **Write Java code that calls a constructor for a class.**
14. **What does the new keyword do in Java?**
15. **What is the purpose of the keyword “this” in Java? Show a code example using it.**
16. **Under which circumstances is the keyword this required? Show a code example.**
17. **What is a getter? Show a code example declaring a getter and then calling it.**
18. **What is a setter? Show a code example declaring a setter and then calling it.**
19. **What is the difference between private and public attributes/methods? Show code**
**examples.**
20. **What are the other two access modifiers of Java besides public and private?**
21. **Why is it recommended to declare all attributes of a class private?**
22. **What is the purpose of the toString() method? What is its signature (return type and**
**inputs)?**
23. **Show a Java example of a Class having a custom toString() method.**
24. **When is the toString() method called?**
25. **What is the Java convention for naming a Class? Show examples of class names**
**following the convention and others that do not.**
26. **What is the Java convention for naming variables? Show examples of variable names**
**following the convention and others that do not.**
27. **What is the requirement that Java makes regarding the name of the file and the name of**
**a class contained in it? Explain with an example.**
28. **What is a static function? Write Java code showing how to call a static function.**
29. **What is a non-static function? Write Java code showing how to call a non-static function.**
30. **What does it mean to instantiate an object? Write down code showing how to instantiate**
**an object.**
31. **What is the heap?**
32. **What does the heap store? Write down code showing something stored in the heap.**
33. **What is the call stack?**
34. **What is the purpose of the call stack?**
35. **What is a stack frame? Show an example.**
36. **Does each function get a frack frame? True or false? Explain.**
37. **What does the call stack store? Write down code showing something stored in the stack.**
38. **Trace the evolution of the call stack during the execution of the Fibonacci function when**
**called as fib(3), as seen in class.**
39. **Explain step by step what happens when you run the Java statement:**
**Mechanic m = new Mechanic(“Leal”);**
**Assuming that Mechanic is a class with a name attribute and that the above statement is**
**correctly placed inside a main function in a class.**
40. **Write code that creates a single-dimensional array of int in Java and initializes it with the**
**{2,3,8} list.**
41. **Write code that creates a single-dimensional array of int in Java and initializes it with a**
**for loop.**
42. **Write code that creates a single-dimensional array of Mechanic in Java and initializes**
**each entry in that array. The class Mechanic should have name and rank attributes.**
43. **Explain with a concrete Java example the Single Responsibility Principle (SRP). Show a**
**class that does not follow it, explain why it doesn’t follow it, and explain how to modify it**
**to respect SRP.**
44. **What is a debugger? What can you do with it?**
45. **What is Git? Explain with a concrete example some of the features it offers.**
46. **Explain step-by-step the basic workflow for using Git.**
47. **What is a commit in Git?**
48. **What is a Git repository?**
49. **Why is it important to learn to use Git?**
50. **What is the purpose of Javadoc? Show an example class that uses Javadoc.**