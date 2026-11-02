# COS-201


<!-- COVER PAGE -->
<div class="cover">
  <h1>COS 201 – Computer Programming I</h1>
  <p style="font-size:14pt; font-weight:bold; color:#0b3d6b;">Practical Assignments (Weeks 1–3)</p>
  <br>
  <p><strong>Student Name:</strong> Adeotan Daniel Oluwaferanmi</p>
  <p><strong>Matriculation Number:</strong> 25/18061</p>
  <p><strong>Programme:</strong> Computer Science (CSC)</p>
  <p><strong>Course:</strong> COS 201 – Computer Programming I</p>
</div>

<!-- WEEK 1 -->
<h2>Week 1 Practical: My First Java Program</h2>

<h3>Algorithm (IPO)</h3>
<ul>
  <li><strong>Input:</strong> None (static output)</li>
  <li><strong>Process:</strong> Print course code/title, programme, three reasons programming is important to Computer Science, and one personal learning goal.</li>
  <li><strong>Output:</strong> Displayed lines of text in the terminal.</li>
</ul>

<h3>Pseudocode</h3>
<pre>START
OUTPUT "Course: COS 201 - Computer Programming I"
OUTPUT "Programme: Computer Science"
OUTPUT "Reason 1: Programming helps solve computational problems."
OUTPUT "Reason 2: Programming supports automation of tasks."
OUTPUT "Reason 3: Programming enables software development."
OUTPUT "My goal: I want to develop simple working applications."
STOP</pre>

<h3>Flowchart</h3>
<pre>        [Start]
           |
   [Display course info]
           |
   [Display programme]
           |
   [Display 3 reasons]
           |
   [Display goal]
           |
         [Stop]</pre>

<h3>Java Source: week01/FirstProgram.java</h3>
<pre>/*
 * COS 201 - Computer Programming I
 * Week 1 Practical: First Java Program
 * Student: Adeotan Daniel Oluwaferanmi
 * Matric: 25/18061
 * Programme: Computer Science
 */
public class FirstProgram {
    public static void main(String[] args) {
        System.out.println("Course: COS 201 - Computer Programming I");
        System.out.println("Programme: Computer Science");
        System.out.println("Reason 1: Programming helps solve computational problems.");
        System.out.println("Reason 2: Programming supports automation of tasks.");
        System.out.println("Reason 3: Programming enables software development.");
        System.out.println("My goal: I want to develop simple working applications.");
    }
}</pre>

<h3>Compilation &amp; Execution</h3>
<pre>&gt; javac FirstProgram.java
&gt; java FirstProgram

Course: COS 201 - Computer Programming I
Programme: Computer Science
Reason 1: Programming helps solve computational problems.
Reason 2: Programming supports automation of tasks.
Reason 3: Programming enables software development.
My goal: I want to develop simple working applications.</pre>

<h3>GitHub README.md (Week 1)</h3>
<pre># COS 201 – Computer Programming I

## Student Details
- Name: Adeotan Daniel Oluwaferanmi
- Matriculation Number: 25/18061
- Programme: Computer Science
- Course Code: COS 201

## Week 1: Introduction to Programming and Problem-Solving

### Practical Exercise
Created and executed my first Java programme.

### File
- week01/FirstProgram.java

### Skills Practised
- Java class and main method
- Output statements
- Compilation and execution
- GitHub version control</pre>

<!-- WEEK 2 -->
<div class="page-break"></div>
<h2>Week 2 Practical: Development Environment and First Java Program</h2>

<h3>Java Source: week02/HelloWorld.java</h3>
<pre>/*
 * COS 201 - Computer Programming I
 * Week 2 Practical: Development Environment and First Java Program
 * Student: Adeotan Daniel Oluwaferanmi
 * Matric: 25/18061
 * Programme: Computer Science
 */
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
        System.out.println("Welcome to COS 201.");
        System.out.println("I am learning Java programming.");

        System.out.println();
        System.out.println("COURSE: COS 201");
        System.out.println("COURSE TITLE: Computer Programming I");
        System.out.println("PROGRAMME: Computer Science");
        System.out.println("WEEK: 2");
        System.out.println("TOPIC: Development Environment and Java");
        System.out.println("GOAL: To learn how to write Java programs.");
    }
}</pre>

<h3>Compilation &amp; Execution</h3>
<pre>&gt; javac HelloWorld.java
&gt; java HelloWorld

Hello, World!
Welcome to COS 201.
I am learning Java programming.

COURSE: COS 201
COURSE TITLE: Computer Programming I
PROGRAMME: Computer Science
WEEK: 2
TOPIC: Development Environment and Java
GOAL: To learn how to write Java programs.</pre>

<h3>GitHub README.md (Week 2 section)</h3>
<pre>## Week 2: Development Environment and First Java Program

### Objectives
- Configure the Java development environment.
- Write, compile and run a Java program.
- Submit source code through GitHub.

### Tools Used
- Java Development Kit (JDK)
- Visual Studio Code
- Git &amp; GitHub Desktop
- GitHub

### Files
- week02/HelloWorld.java

### How to Run
1. Open a terminal in the `week02` directory.
2. Compile: `javac HelloWorld.java`
3. Run: `java HelloWorld`

### Learning Outcome
Practised creating, compiling and running a Java program and submitting source code through GitHub.</pre>

<!-- WEEK 3 -->
<div class="page-break"></div>
<h2>Week 3 Practical: Variables, Data Types, Expressions and Input/Output</h2>

<h3>Program 1 — Simple Calculator</h3>
<pre>/*
 * COS 201 - Computer Programming I
 * Week 3 Practical 1: Simple Calculator
 * Student: Adeotan Daniel Oluwaferanmi
 * Matric: 25/18061
 * Programme: Computer Science
 */
import java.util.Scanner;

public class SimpleCalculator {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter the first number: ");
        double firstNumber = input.nextDouble();

        System.out.print("Enter the second number: ");
        double secondNumber = input.nextDouble();

        double sum        = firstNumber + secondNumber;
        double difference = firstNumber - secondNumber;
        double product    = firstNumber * secondNumber;

        System.out.println("\n--- CALCULATOR RESULTS ---");
        System.out.printf("Sum: %.2f%n", sum);
        System.out.printf("Difference: %.2f%n", difference);
        System.out.printf("Product: %.2f%n", product);

        if (secondNumber != 0) {
            double quotient = firstNumber / secondNumber;
            System.out.printf("Quotient: %.2f%n", quotient);
        } else {
            System.out.println("Division is undefined for a zero divisor.");
        }

        input.close();
    }
}</pre>

<h3>Sample Run</h3>
<pre>Enter the first number: 20
Enter the second number: 4

--- CALCULATOR RESULTS ---
Sum: 24.00
Difference: 16.00
Product: 80.00
Quotient: 5.00</pre>

<h3>Test Case (Zero Divisor)</h3>
<pre>Enter the first number: 10
Enter the second number: 0

--- CALCULATOR RESULTS ---
Sum: 10.00
Difference: 10.00
Product: 0.00
Division is undefined for a zero divisor.</pre>

<h3>Program 2 — Student Average Calculator</h3>
<pre>/*
 * COS 201 - Computer Programming I
 * Week 3 Practical 2: Student Average Calculator
 * Student: Adeotan Daniel Oluwaferanmi
 * Matric: 25/18061
 * Programme: Computer Science
 */
import java.util.Scanner;

public class AverageCalculator {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter student name: ");
        String name = input.nextLine();

        System.out.print("Enter score for Course 1: ");
        double score1 = input.nextDouble();

        System.out.print("Enter score for Course 2: ");
        double score2 = input.nextDouble();

        System.out.print("Enter score for Course 3: ");
        double score3 = input.nextDouble();

        // Validation (extension exercise)
        if (score1 &lt; 0 || score1 &gt; 100 ||
            score2 &lt; 0 || score2 &gt; 100 ||
            score3 &lt; 0 || score3 &gt; 100) {
            System.out.println("Error: All scores must be between 0 and 100.");
            input.close();
            return;
        }

        double total   = score1 + score2 + score3;
        double average = total / 3.0;

        System.out.println("\n--- STUDENT RESULT ---");
        System.out.println("Student: " + name);
        System.out.printf("Total: %.2f%n", total);
        System.out.printf("Average: %.2f%n", average);

        input.close();
    }
}</pre>

<h3>Sample Run</h3>
<pre>Enter student name: Adeotan Daniel
Enter score for Course 1: 70
Enter score for Course 2: 80
Enter score for Course 3: 90

--- STUDENT RESULT ---
Student: Adeotan Daniel
Total: 240.00
Average: 80.00</pre>

<h3>Test Case (Invalid Score)</h3>
<pre>Enter student name: Test Student
Enter score for Course 1: 110
Enter score for Course 2: 80
Enter score for Course 3: 90
Error: All scores must be between 0 and 100.</pre>

<h3>Program 3 — Item Cost Calculator</h3>
<pre>/*
 * COS 201 - Computer Programming I
 * Week 3 Practical 3: Item Cost Calculator
 * Student: Adeotan Daniel Oluwaferanmi
 * Matric: 25/18061
 * Programme: Computer Science
 */
import java.util.Scanner;

public class ItemCost {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter item name: ");
        String itemName = input.nextLine();

        System.out.print("Enter quantity: ");
        int quantity = input.nextInt();

        System.out.print("Enter unit price: ");
        double unitPrice = input.nextDouble();

        double totalCost = quantity * unitPrice;

        System.out.println("\n--- PURCHASE SUMMARY ---");
        System.out.println("Item: " + itemName);
        System.out.println("Quantity: " + quantity);
        System.out.printf("Unit price: %.2f%n", unitPrice);
        System.out.printf("Total cost: %.2f%n", totalCost);

        input.close();
    }
}</pre>

<h3>Sample Run</h3>
<pre>Enter item name: Exercise Book
Enter quantity: 3
Enter unit price: 1500

--- PURCHASE SUMMARY ---
Item: Exercise Book
Quantity: 3
Unit price: 1500.00
Total cost: 4500.00</pre>

<!-- REPO STRUCTURE + SUBMISSION -->
<div class="page-break"></div>
<h2>Final Repository Structure</h2>
<pre>COS201-Programming-I/
├── README.md
├── week01/
│   └── FirstProgram.java
├── week02/
│   └── HelloWorld.java
└── week03/
    ├── SimpleCalculator.java
    ├── AverageCalculator.java
    └── ItemCost.java</pre>

<h2>Submission Message</h2>
<div class="note">
<strong>COS 201 – Practical Submission (Weeks 1–3)</strong>
</div>
<p>Dear Lecturer,</p>
<p>I am submitting my practical assignments for COS 201 – Computer Programming I.</p>
<table>
  <tr><th>Field</th><th>Details</th></tr>
  <tr><td>Student Name</td><td>Adeotan Daniel Oluwaferanmi</td></tr>
  <tr><td>Matriculation Number</td><td>25/18061</td></tr>
  <tr><td>Programme</td><td>Computer Science</td></tr>
  <tr><td>Assignments Covered</td><td>Week 1 (First Java Program), Week 2 (Development Environment &amp; First Java Program), Week 3 (Variables, Data Types, Expressions and I/O)</td></tr>
  <tr><td>GitHub Repository URL</td><td>[https://github.com/ADECABANA/COS-201]</td></tr>
</table>
<p>The repository contains the source files <code>week01/FirstProgram.java</code>, <code>week02/HelloWorld.java</code>, <code>week03/SimpleCalculator.java</code>, <code>week03/AverageCalculator.java</code> and <code>week03/ItemCost.java</code>, along with a README documenting the objectives, instructions for compiling/running, and skills practised. All programs have been compiled and tested successfully.</p>
<p>Thank you.</p>

<footer>
  COS 201 – Computer Programming I &nbsp;|&nbsp; Adeotan Daniel Oluwaferanmi &nbsp;|&nbsp; 25/18061
</footer>

</body>
</html>
