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

Private attributes/methods can ONLY be accessed by the object that owns it.
Public attributes/methods can be accessed anywhere from anything.

**Public example:**
```java
public class Box {
	public int size;
}

public class Main {
	public static void Main(String[] args) {
		Box myBox = new Box(); 
		myBox.size = 10; // I can change it from anywhere because it's public
	}
}
```
**Private example:**
```java
public class Box {
	private int size;
}

public class Main {
	public static void Main(String[] args) {
		Box myBox = new Box(); 
		myBox.size = 10; // This DOES NOT WORK anymore!!! 
	}
}
```
17. **What are the other two access modifiers of Java besides public and private?**
	`Static` and `protected`. 

18. **Why is it recommended to declare all attributes of a class private?**
	This ensures that other parts of the program don't just change stuff willy nilly and your data is always being protected through setters which might have some logic to ensure that the values make sense for your object. 
	
	An example is a rectangle object with a width setter. You can't have a negative width, so the setter method would make sure that the width isn't negative or it won't actually change the value. If it was public there's nothing protecting the sanity of your object's attributes.

18. **What is the purpose of the toString() method? What is its signature (return type and inputs)?**
	The `toString()` method is special because if an object has it defined it will return that when you implicitly cast the object to a string.

19. **Show a Java example of a Class having a custom toString() method.**
```java
public class Box {
	private int height;
	private int width;
	
	public Box(int height, int width) {
		this.height = height;
		this.width = width;
	}
	
	public String toString() {
	// Uses string concatenation (Adding Strings with the + symbol) to make one big String.
	return "Height: " + this.height "\n" + // \n means new line!
			"Width: " + this.width;
	}
}
```

19. **When is the toString() method called?**
	When you implicitly cast the object to a String.
Example: 
```java
// the above box object is also here
public static main(String[] args) {
	Box myBox = new Box(10, 20); // Make a new box
	System.out.println(myBox); // Print the box!
	
	//Outputs the height and width of the box
}
```

19. **What is the Java convention for naming a Class? Show examples of class names**
**following the convention and others that do not.**
PascalCase. The first letter is capitalized, as well as the first letter of every word in the object.

**Good examples:**
- Cat
- DogThatBarks
- EvilCelery

**Bad Examples:**
- cat
- dogthat_barks
- evil-Celery

20. **What is the Java convention for naming variables? Show examples of variable names following the convention and others that do not.**
camelCase: The same as PascalCase except the first letter isn't capitalized.

**Good Examples:**
- myCat
- georgeTheMechanic
- example

**Bad Examples:**
- my_cat
- Georgethemechanic
- EXAMPLE

21. **What is the requirement that Java makes regarding the name of the file and the name of a class contained in it? Explain with an example.**
They must be the same

Example:
```java
// Car.java file name
public Car {
//...
}
```

22. **What is a static function? Write Java code showing how to call a static function.**


23. **What is a non-static function? Write Java code showing how to call a non-static function.**
24. **What does it mean to instantiate an object? Write down code showing how to instantiate**
**an object.**
25. **What is the heap?**
26. **What does the heap store? Write down code showing something stored in the heap.**
27. **What is the call stack?**
28. **What is the purpose of the call stack?**
29. **What is a stack frame? Show an example.**
30. **Does each function get a frack frame? True or false? Explain.**
31. **What does the call stack store? Write down code showing something stored in the stack.**
32. **Trace the evolution of the call stack during the execution of the Fibonacci function when**
**called as fib(3), as seen in class.**
33. **Explain step by step what happens when you run the Java statement:**
**Mechanic m = new Mechanic(“Leal”);**
**Assuming that Mechanic is a class with a name attribute and that the above statement is**
**correctly placed inside a main function in a class.**
34. **Write code that creates a single-dimensional array of int in Java and initializes it with the**
**{2,3,8} list.**
35. **Write code that creates a single-dimensional array of int in Java and initializes it with a**
**for loop.**
36. **Write code that creates a single-dimensional array of Mechanic in Java and initializes**
**each entry in that array. The class Mechanic should have name and rank attributes.**
37. **Explain with a concrete Java example the Single Responsibility Principle (SRP). Show a**
**class that does not follow it, explain why it doesn’t follow it, and explain how to modify it**
**to respect SRP.**
38. **What is a debugger? What can you do with it?**
39. **What is Git? Explain with a concrete example some of the features it offers.**
40. **Explain step-by-step the basic workflow for using Git.**
41. **What is a commit in Git?**
42. **What is a Git repository?**
43. **Why is it important to learn to use Git?**
44. **What is the purpose of Javadoc? Show an example class that uses Javadoc.**