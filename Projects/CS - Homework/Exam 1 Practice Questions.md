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

**JVM**: The **J**ava **V**irtual **M**achine actually processes Java programs. It takes in java bytecode that's created by the java compiler and translates the java bytecode into architecture specific CPU instructions.

4. **What is a compiler? What does it do?**
The java compiler converts human readable java code into java bytecode that a JVM can run.
Generally, compilers convert the human readable code into machine code that a computer can execute.

5. **What does it mean Write-once Run-Everywhere?**
A java program can run on any computer with the same bytecode. This is because the bytecode is translated by the JVM for computer specific instructions.

Normally, compilers only output code for a single kind of computer, but because the JVM translates java bytecode for you into whatever local computer you're using, you never have to worry about different processors in a computer.


6. **Explain the Von Neumann architecture.**
A computer consists of two parts:
- A brain (The CPU) which takes code and runs them instruction by instruction
- Memory (RAM / Disk) which remembers the code and all of your program's variables.
The CPU will take the memory for your program, and run the instructions that instruct it how to move variables and change variables until your program is done running.

6. **Write down a simple Java program that prints a message to the command line.**
```java
public class Main {
	public static void main(string[] args) {
		System.out.println("Hello!! :)");
	}
}
```

6. **What is the difference between declaring and initializing a variable in Java?**
Declaring a variable instructs the computer to reserve some space for the variable.
Initializing a variable fills that same space with the value you tell it to.
Example:
```java
public class Main {
	public static void main(String[] args) {
		int number; // Declares the variable. The computer will reserve the space for an int in your computer's memory.
		
		int number2 = 1234; //Intializes a variable with a value. This declares it AND intializes it
	}
}

```


7. **What is a constructor in Java?**
A constructor is part of a class. It is a special method for a class that is used when you want to make an object. It can have different inputs and have special logic for what to do when the object is initially made.

```Java
public class Box {
	int size; // A variable that the object has
	
	public Box(int size) { // A constructor method. It has the same name as the class
		this.size = size; // Assigns the constructor's input to the object's variable
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); // The constructor is called when you use "new"
		
		// The constructor returns the MEMORY ADDRESS of the object which is stored on the heap (somewhere random on the computer that wasn't being used already)
	}
}

```

8. **What is the default constructor in Java?**
If you don't specify your own constructor, the default constructor is implicitly allowed and it initializes an object with no arguments or logic. Constructors look like this.
```java
public class Box {
	int size;
	// NO CONSTRUCTOR DEFINED. Using the Java default constructor
}

public class Main {
	public static void Main(String[] args) {
		Box myBox = new Box(); // DEFAULT CONSTRUCTOR 
	}
}
```

9. **What happens in Java to the default constructor if you define another constructor for that same class? Explain.**
It is overridden and is no longer available. 

10. **Write Java code showing a class with a constructor initializing an attribute.**
```Java
public class Box {
	int size; // Attribute
	
	public Box(int size) { // Constructor
		this.size = size; // Intializes the attribute
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); // 10 is the value used to initialize my first Box object
	}
}

```

11. **Write Java code that calls a constructor for a class.**
See above

12. **What does the new keyword do in Java?**
The new keyword calls an object's constructor and returns the memory address the computer found for the new object.

```java
public class Box {
	int size;
	
	public Box(int size) {
		this.size = size;
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); // myBox will actually store the MEMORY ADDRESS of the new Box object. myBox ACTUALLY lives somewhere random on the computer's memory (the heap).
	}
}
```

13. **What is the purpose of the keyword “this” in Java? Show a code example using it.**
```java
public class Box {
	int size;
	
	public Box(int size) {
		this.size = size; // I use this here because this.size refer's to the object's size but the method also takes in a variable named size. It lets java know which one is which.
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); 
	}
}
```

14. **Under which circumstances is the keyword this required? Show a code example.**
```java
public class Box {
	int size;
	
	public Box(int size) {
		size = size; // This doesn't work!!! Because Java can't tell which size is supposed to mean the object's size and which size is supposed to mean the constructor's size.
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); 
	}
}
```

15. **What is a getter? Show a code example declaring a getter and then calling it.**
```java
public class Box {
	int size;
	
	public Box(int size) {
		this.size = size; 
	}
	
	public int getSize() {
		return this.size; // This method will let you GET the size of the box
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); 
		System.out.println("myBox's size: " + myBox.getSize());
	}
}
```

16. **What is a setter? Show a code example declaring a setter and then calling it.**
```java
public class Box {
	int size;
	
	public Box(int size) {
		this.size = size; 
	}
	
	public int getSize() {
		return this.size;
	}
	
	public void setSize() {
		this.size; = size; // This method will let you SET the size of the box
	}
	
	public static void Main(String[] args) {
		Box myBox = new Box(10); 
		System.out.println("myBox's first size: " + myBox.getSize()); // Says 10
		// CHANGE the size with the setter
		myBox.setSize(1000);
		System.out.println("myBox's new size: " + mybox.getSize()); // Says 1000
	}
}
```

17. **What is the difference between private and public attributes/methods? Show code**
**examples.**
18. **What are the other two access modifiers of Java besides public and private?**
19. **Why is it recommended to declare all attributes of a class private?**
20. **What is the purpose of the toString() method? What is its signature (return type and**
**inputs)?**
21. **Show a Java example of a Class having a custom toString() method.**
22. **When is the toString() method called?**
23. **What is the Java convention for naming a Class? Show examples of class names**
**following the convention and others that do not.**
24. **What is the Java convention for naming variables? Show examples of variable names**
**following the convention and others that do not.**
25. **What is the requirement that Java makes regarding the name of the file and the name of**
**a class contained in it? Explain with an example.**
26. **What is a static function? Write Java code showing how to call a static function.**
27. **What is a non-static function? Write Java code showing how to call a non-static function.**
28. **What does it mean to instantiate an object? Write down code showing how to instantiate**
**an object.**
29. **What is the heap?**
30. **What does the heap store? Write down code showing something stored in the heap.**
31. **What is the call stack?**
32. **What is the purpose of the call stack?**
33. **What is a stack frame? Show an example.**
34. **Does each function get a frack frame? True or false? Explain.**
35. **What does the call stack store? Write down code showing something stored in the stack.**
36. **Trace the evolution of the call stack during the execution of the Fibonacci function when**
**called as fib(3), as seen in class.**
37. **Explain step by step what happens when you run the Java statement:**
**Mechanic m = new Mechanic(“Leal”);**
**Assuming that Mechanic is a class with a name attribute and that the above statement is**
**correctly placed inside a main function in a class.**
38. **Write code that creates a single-dimensional array of int in Java and initializes it with the**
**{2,3,8} list.**
39. **Write code that creates a single-dimensional array of int in Java and initializes it with a**
**for loop.**
40. **Write code that creates a single-dimensional array of Mechanic in Java and initializes**
**each entry in that array. The class Mechanic should have name and rank attributes.**
41. **Explain with a concrete Java example the Single Responsibility Principle (SRP). Show a**
**class that does not follow it, explain why it doesn’t follow it, and explain how to modify it**
**to respect SRP.**
42. **What is a debugger? What can you do with it?**
43. **What is Git? Explain with a concrete example some of the features it offers.**
44. **Explain step-by-step the basic workflow for using Git.**
45. **What is a commit in Git?**
46. **What is a Git repository?**
47. **Why is it important to learn to use Git?**
48. **What is the purpose of Javadoc? Show an example class that uses Javadoc.**