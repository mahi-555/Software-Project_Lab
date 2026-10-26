# Software-Project_Lab

# Java Lab Practice: Stack, Heap, and Inner Classes

This repository contains two Java lab practice programs demonstrating object identity, instance variables, local variables, heap objects, and method execution frames.
# Requirements 
- Java JDK 25 (or a compatible JDK)
- Command Prompt / Terminal
- A text editor such as Notepad

# Problem 1: Student — Stack and Heap Memory
File: Main.java

# The program:
- Creates a Student class with the instance variable age.
- Declares the local variable marks inside display().
- Creates a Student object in main().
- Prints the object's identity hash code using System.identityHashCode().
# Example output (the hash code may differ):
Student Object Created
Object Identity Hash Code: 12345678
Instance Variable (age): 20
Local Variable (marks): 85
# Run Problem 1
1. Save the first program as Main.java in a folder.
2. Open Command Prompt in that folder.
3. Run:
javac Main.java
java Main
# Problem 2: Employee — Stack Frames, Heap Objects, and Inner Classes
File: Main.java

# The program:
- Creates an Employee object with an instance variable salary.
- Accepts salary and bonus from the user.
- Declares bonus as a parameter of display().
- Defines a local inner class named Report inside display().
- Creates a Report object and calls its show() method.
- Prints identity hash codes for the Employee and Report objects.
- 
# Example input:
Enter salary: 30000
Enter bonus: 5000
Example output (hash codes will vary):
Enter salary: 30000
Enter bonus: 5000

Employee Object Created
Employee Identity Hash Code: 12345678

Inside display() Method:
Salary (Instance Variable): 30000
Bonus (Local Variable): 5000

Report Object Created
Report Identity Hash Code: 87654321
Report: Employee salary is 30000

# Memory Concept:
Employee object -> Heap
Report object -> Heap
salary -> Instance field
bonus -> Local variable in display()
show() -> Executes in its own method frame

# Run Problem 2
The two programs both use the public class name Main, so run them separately. Replace the contents of Main.java with the second program, save it, then run:
javac Main.java
java Main
Key Concepts
Concept	Meaning
Stack frame	Execution context created for a method call.
Heap	Memory area where Java objects are generally allocated.
Instance variable	A field belonging to an object, such as age or salary.
Local variable	A variable declared within a method, such as marks.
Local inner class	A class declared inside a method or block.
System.identityHashCode()	Returns an identity-based hash code; it is not the object's actual memory address.


# Important Notes
- Identity hash codes are illustrative and may differ between runs.
- The stack and heap descriptions are simplified explanations of Java memory behavior.
- Save and compile one Main.java program at a time because both examples define public class Main.
  
