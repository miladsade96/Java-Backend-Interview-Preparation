# Technical Interview Questions - Java

1. **What is java programming language?**  
   Java is a high-level, object-oriented programming language designed with "write once, run anywhere" portability. It
   compiles source code into bytecode that runs on the Java Virtual Machine (JVM), making it platform-independent. Java
   features automatic memory management through garbage collection and strong type safety. It's widely used for
   enterprise applications, Android development, web services, and large-scale systems due to its robustness, security,
   and extensive ecosystem.
2. **What are JDK, JRE, and JVM?**
    - JDK (Java Development Kit): A software development kit that includes tools for developing, debugging, and
      monitoring Java applications. It contains the JRE and development tools like the Java compiler (javac).
    - JRE (Java Runtime Environment): A package that provides the libraries, Java Virtual Machine (JVM), and other
      components necessary to run Java applications. It does not include development tools.
    - JVM (Java Virtual Machine): An abstract computing machine that enables a computer to run Java bytecode. It
      interprets compiled Java code and provides platform independence by allowing Java programs to run on any device
      with a compatible JVM.
3. **How a java program compiled and executed?**  
   A Java program is compiled and executed in the following steps:
    1. Writing the Code: The developer writes the Java source code in a file with a .java extension using a text editor
       or an Integrated Development Environment (IDE).
    2. Compilation: The Java source code is compiled using the Java Compiler (javac). This process converts the source
       code into bytecode, which is stored in a file with a .class extension.
       ```
       javac MyProgram.java
       ```
    3. Execution: The compiled bytecode is executed by the Java Virtual Machine (JVM) using the java command. The JVM
       interprets the bytecode and translates it into machine code that can be executed by the host operating system.
       ```
       java MyProgram
       ```
4. **What is compile-time and run-time in java?**
    - Compile-time: This is the phase when the Java source code is translated into bytecode by the Java compiler (
      javac).
      During this phase, the compiler checks for syntax errors and ensures that the code adheres to Java's language
      rules.
      If any errors are found, they must be corrected before the code can be successfully compiled.
    - Run-time: This is the phase when the compiled bytecode is executed by the Java Virtual Machine (JVM). During
      run-time, the JVM interprets the bytecode and performs tasks such as memory allocation, garbage collection, and
      executing the program's logic. Errors that occur during this phase, such as exceptions, are known as run-time
      errors.
5. **What are the main features and advantages of Java?**
    - Platform Independence: Java's "write once, run anywhere" capability allows code to run on any device with a
      compatible JVM.
    - Object-Oriented: Java supports object-oriented programming principles, promoting code reusability and modularity.
    - Robustness: Java has strong memory management, exception handling, and type-checking features that enhance
      reliability.
    - Security: Java provides a secure execution environment through its sandbox model, bytecode verification, and
      built-in security features.
    - Multithreading: Java supports multithreading, allowing concurrent execution of multiple threads for improved
      performance.
    - Rich Standard Library: Java offers an extensive standard library with pre-built classes and methods for various
      functionalities, reducing development time.
    - Automatic Memory Management: Java's garbage collection automatically manages memory allocation and deallocation,
      reducing memory leaks and improving performance.
    - Community Support: Java has a large and active community, providing extensive resources, libraries, frameworks,
      and tools for developers.
6. **How java is platform independent? Why convert java code to bytecode?**  
   Java is platform-independent because it uses the Java Virtual Machine (JVM) as an intermediary between the compiled
   Java code and the underlying operating system. When a Java program is compiled, it is converted into an intermediate
   form called bytecode, which is stored in .class files. This bytecode is not specific to any particular hardware or
   operating system.

   The JVM interprets the bytecode and translates it into machine code that can be executed by the host operating
   system.
   Since JVMs are available for various platforms (Windows, macOS, Linux, etc.), the same Java bytecode can run on any
   device with a compatible JVM without modification. This "write once, run anywhere" capability is what makes Java
   platform-independent.

   Converting Java code to bytecode allows for this level of abstraction and portability, enabling developers to create
   applications that can run seamlessly across different environments.
7. **What is main method in java? What is the role of public, static, void, and String[] args in main method?**  
   The main method in Java is the entry point of any Java application. It is where the program starts executing. The
   signature of the main method is:
   ```java
   public static void main(String[] args)
   ```
    - `public`: This is an access modifier that allows the main method to be accessible from anywhere, including outside
      the class. This is necessary because the Java Virtual Machine (JVM) needs to call this method to start the
      program.
    - `static`: This keyword indicates that the main method belongs to the class itself rather than an instance of the
      class. This means that the JVM can invoke the main method without creating an object of the class.
    - `void`: This indicates that the main method does not return any value. It simply performs its task and exits.
    - `String[] args`: This parameter is an array of Strings that allows command-line arguments to be passed to the
      program when it is executed. Each element in the array represents a separate argument provided by the user.
8. **What is java bytecode?**  
   Java bytecode is an intermediate representation of a Java program that is generated by the Java compiler (javac)
   after compiling the source code. It is a low-level, platform-independent code that is designed to be executed by the
   Java Virtual Machine (JVM).

   Bytecode is stored in .class files and consists of a set of instructions that the JVM can interpret and execute. The
   use of bytecode allows Java to achieve its "write once, run anywhere" capability, as the same bytecode can run on
   any device with a compatible JVM, regardless of the underlying hardware or operating system.

   Bytecode is more efficient than source code for execution, as it is optimized for performance by the JVM. The JVM
   translates bytecode into machine code at runtime, allowing for dynamic optimization and improved performance.
9. **What are variables and data types? What are the types of data types?**  
   Variables in Java are named storage locations that hold data values. Each variable has a specific data type that
   defines the kind of data it can store and the operations that can be performed on it.

   Data types in Java can be broadly categorized into two types:
    1. Primitive Data Types: These are the basic data types that store simple values. Java has eight primitive data
       types:
        - `byte`: 8-bit signed integer
        - `short`: 16-bit signed integer
        - `int`: 32-bit signed integer
        - `long`: 64-bit signed integer
        - `float`: 32-bit floating-point number
        - `double`: 64-bit floating-point number
        - `char`: 16-bit Unicode character
        - `boolean`: Represents true or false values
    2. Reference Data Types: These data types store references (memory addresses) to objects rather than the actual
       data values. Reference data types include:
        - Classes: User-defined data types that can contain fields (variables) and methods (functions).
        - Arrays: Collections of elements of the same type, stored in contiguous memory locations.
        - Interfaces: Abstract data types that define a contract for classes to implement.
        - Enums: Special data types that define a set of named constants.
          -Strings: A special class in Java that represents a sequence of characters.

   Understanding variables and data types is essential for effective programming in Java, as they determine how data is
   stored, manipulated, and accessed within a program.
10. **What are the differences between primitive and reference data types in java?**
    - Primitive Data Types:
        - Store simple values directly in memory.
        - Have a fixed size and predefined range of values.
        - Examples include int, float, char, and boolean.
        - Operations on primitive types are performed directly on the values.
        - Primitive types are stored on the stack memory.
    - Reference Data Types:
        - Store references (memory addresses) to objects rather than the actual data values.
        - Can represent complex data structures and user-defined types.
        - Examples include classes, arrays, interfaces, and enums.
        - Operations on reference types involve manipulating the objects they refer to.
        - Reference types are stored on the heap memory, while the reference itself is stored on the stack.
11. **What are operators in java? What are the types of operators?**  
    Operators in Java are special symbols or keywords that perform specific operations on one or more operands (
    variables,
    values, or expressions) to produce a result. Java provides a variety of operators that can be categorized into
    several
    types:
    1. Arithmetic Operators: Used for performing basic mathematical operations.
        - `+` (Addition)
        - `-` (Subtraction)
        - `*` (Multiplication)
        - `/` (Division)
        - `%` (Modulus)
    2. Relational Operators: Used for comparing two values and returning a boolean result.
        - `==` (Equal to)
        - `!=` (Not equal to)
        - `>` (Greater than)
        - `<` (Less than)
        - `>=` (Greater than or equal to)
        - `<=` (Less than or equal to)
    3. Logical Operators: Used for combining multiple boolean expressions.
        - `&&` (Logical AND)
        - `||` (Logical OR)
        - `!` (Logical NOT)
    4. Assignment Operators: Used for assigning values to variables.
        - `=` (Simple assignment)
        - `+=` (Add and assign)
        - `-=` (Subtract and assign)
        - `*=` (Multiply and assign)
        - `/=` (Divide and assign)
        - `%=` (Modulus and assign)
    5. Unary Operators: Operate on a single operand to perform various operations.
        - `++` (Increment)
        - `--` (Decrement)
        - `+` (Unary plus)
        - `-` (Unary minus)
    6. Bitwise Operators: Perform operations on individual bits of integer types.
        - `&` (Bitwise AND)
        - `|` (Bitwise OR)
        - `^` (Bitwise XOR)
        - `~` (Bitwise NOT)
        - `<<` (Left shift)
        - `>>` (Right shift)
        - `>>>` (Unsigned right shift)
    7. Ternary Operator: A shorthand for an if-else statement that takes three operands.
        - `? :` (Conditional operator)
12. **What is instanceOf operator in java?**  
    The `instanceof` operator in Java is a binary operator used to test whether an object is an instance of a specific
    class or implements a particular interface. It returns a boolean value: `true` if the object is an instance of the
    specified type, and `false` otherwise.

    The syntax for using the `instanceof` operator is as follows:
    ```java
    object instanceof Type
    ```
    - `object`: The reference variable that you want to check.
    - `Type`: The class or interface you want to compare against.

    Example:
    ```java
    class Animal {}
    class Dog extends Animal {}

    public class Main {
        public static void main(String[] args) {
            Animal myAnimal = new Dog();

            if (myAnimal instanceof Dog) {
                System.out.println("myAnimal is an instance of Dog");
            } else {
                System.out.println("myAnimal is not an instance of Dog");
            }
        }
    }
    ```
    In this example, the output will be "myAnimal is an instance of Dog" because `myAnimal` refers to an object of
    type `Dog`.
13. **What are control statements in java? What are the types of control statements?**  
    Control statements in Java are used to control the flow of execution of the program based on certain conditions or
    loops. They allow developers to make decisions, repeat actions, and manage the sequence of operations in a program.

    The types of control statements in Java include:
    1. Decision-Making Statements: These statements allow the program to make decisions based on conditions.
        - `if` statement: Executes a block of code if a specified condition is true.
        - `if-else` statement: Executes one block of code if a condition is true and another block if it is false.
        - `switch` statement: Allows selection among multiple options based on the value of a variable.
        - `ternary` operator: A shorthand for an if-else statement that returns a value based on a condition.
    2. Looping Statements: These statements enable the repetition of a block of code multiple times.
        - `for` loop: Repeats a block of code a specific number of times.
        - `while` loop: Repeats a block of code as long as a specified condition is true.
        - `do-while` loop: Similar to the while loop, but guarantees that the block of code is executed at least once
          before checking the condition.
    3. Jump Statements: These statements are used to transfer control to another part of the program.
        - `break` statement: Exits from a loop or switch statement prematurely.
        - `continue` statement: Skips the current iteration of a loop and proceeds to the next iteration.
        - `return` statement: Exits from a method and optionally returns a value to the caller.

    These control statements are essential for creating dynamic and flexible programs that can respond to different
    conditions and perform repetitive tasks efficiently.
14. **What are the differences between while loop, do-while loop, and for loop in java?**
    - `while` Loop:
        - The `while` loop checks the condition before executing the loop body.
        - If the condition is false initially, the loop body may not execute at all.
        - Syntax:
          ```java
          while (condition) {
              // loop body
          }
          ```
    - `do-while` Loop:
        - The `do-while` loop executes the loop body first and then checks the condition.
        - This guarantees that the loop body is executed at least once, regardless of the condition.
        - Syntax:
          ```java
          do {
              // loop body
          } while (condition);
          ```
    - `for` Loop:
        - The `for` loop is typically used when the number of iterations is known beforehand.
        - It consists of three parts: initialization, condition, and increment/decrement, all in one line.
        - Syntax:
          ```java
          for (initialization; condition; increment/decrement) {
              // loop body
          }
          ```

    In summary, use a `while` loop when the number of iterations is unknown and may not execute at all, a `do-while`
    loop when you want to ensure at least one execution of the loop body, and a `for` loop when you know the exact
    number
    of iterations in advance.
15. **What are the differences between break and continue statements in java?**
    - `break` Statement:
        - The `break` statement is used to exit from a loop or switch statement prematurely.
        - When encountered, it immediately terminates the loop or switch and transfers control to the statement
          following
          the loop or switch.
        - It is commonly used to stop the execution of a loop when a certain condition is met.
        - Example:
          ```java
          for (int i = 0; i < 10; i++) {
              if (i == 5) {
                  break; // Exit the loop when i is 5
              }
              System.out.println(i);
          }
          ```
    - `continue` Statement:
        - The `continue` statement is used to skip the current iteration of a loop and proceed to the next iteration.
        - When encountered, it skips the remaining code in the loop body for that iteration and goes back to the loop's
          condition check.
        - It is commonly used to skip specific iterations based on certain conditions without terminating the entire
          loop.
        - Example:
          ```java
          for (int i = 0; i < 10; i++) {
              if (i % 2 == 0) {
                  continue; // Skip even numbers
              }
              System.out.println(i);
          }
          ```

    In summary, use `break` to exit a loop or switch entirely, and use `continue` to skip the current iteration and move
    to the next one.
16. **What are the differences between for loop and for-each loop in java?**
    - `for` Loop:
        - The `for` loop is a general-purpose loop that allows you to iterate over a range of values or perform a
          specific
          number of iterations.
        - It consists of three parts: initialization, condition, and increment/decrement, all in one line.
        - You have full control over the loop variable and can modify it as needed within the loop body.
        - Syntax:
          ```java
          for (initialization; condition; increment/decrement) {
              // loop body
          }
          ```
        - Example:
          ```java
          for (int i = 0; i < 10; i++) {
              System.out.println(i);
          }
          ```
    - `for-each` Loop:
        - The `for-each` loop (also known as the enhanced for loop) is specifically designed for iterating over arrays
          and
          collections.
        - It simplifies the syntax by eliminating the need for an explicit loop variable and condition.
        - The loop variable automatically takes on each value from the array or collection in each iteration.
        - Syntax:
          ```java
          for (Type element : collection) {
              // loop body
          }
          ```
        - Example:
          ```java
          int[] numbers = {1, 2, 3, 4, 5};
          for (int number : numbers) {
              System.out.println(number);
          }
          ```

    In summary, use a `for` loop when you need more control over the iteration process, and use a `for-each` loop when
    iterating over arrays or collections for cleaner and more readable code.
17. **What is switch statement in java? How it works?**  
    The `switch` statement in Java is a control flow statement that allows you to execute one block of code among
    multiple
    options based on the value of a variable or expression. It is often used as an alternative to multiple `if-else`
    statements when you have a fixed set of possible values to compare against.

    The syntax of the `switch` statement is as follows:
    ```java
    switch (expression) {
        case value1:
            // code block for value1
            break;
        case value2:
            // code block for value2
            break;
        // more cases...
        default:
            // code block if no cases match
    }
    ```

    How it works:
    1. The `expression` inside the `switch` statement is evaluated once.
    2. The value of the expression is compared against the values specified in each `case`.
    3. If a match is found, the corresponding code block for that `case` is executed.
    4. The `break` statement is used to exit the `switch` statement after executing a case. If `break` is omitted, the
       execution will continue to the next case (this is known as "fall-through").
    5. If no cases match the expression's value, the code block under the `default` case (if provided) is executed.

    Example:
    ```java
    int day = 3;
    String dayName;

    switch (day) {
        case 1:
            dayName = "Monday";
            break;
        case 2:
            dayName = "Tuesday";
            break;
        case 3:
            dayName = "Wednesday";
            break;
        case 4:
            dayName = "Thursday";
            break;
        case 5:
            dayName = "Friday";
            break;
        case 6:
            dayName = "Saturday";
            break;
        case 7:
            dayName = "Sunday";
            break;
        default:
            dayName = "Invalid day";
    }

    System.out.println("Day: " + dayName);
    ```
    In this example, since `day` is 3, the output will be "Day: Wednesday".

18. **When to use which types of conditional statements in java? (if-else, switch, ternary operator)**

    - Use `if-else` statements when:
        - You have complex conditions that require multiple logical checks.
        - The conditions are not based on a single variable or expression.
        - You need to handle ranges of values or more intricate decision-making processes.
        - Example:
          ```java
          if (age < 13) {
              System.out.println("Child");
          } else if (age < 20) {
              System.out.println("Teenager");
          } else {
              System.out.println("Adult");
          }
          ```
    - Use `switch` statements when:
        - You have a single variable or expression that can take on a limited set of discrete values.
        - You want to improve code readability when dealing with multiple specific cases.
        - The cases are mutually exclusive and do not require complex conditions.
        - Example:
          ```java
          switch (day) {
              case 1:
                  System.out.println("Monday");
                  break;
              case 2:
                  System.out.println("Tuesday");
                  break;
              // more cases...
              default:
                  System.out.println("Invalid day");
          }
          ```
    - Use the `ternary operator` when:
        - You need a concise way to assign a value based on a simple condition.
        - The condition is straightforward and can be expressed in a single line.
        - You want to improve code brevity without sacrificing readability.
        - Example:
          ```java
          String result = (score >= 50) ? "Pass" : "Fail";
          System.out.println(result);
          ```

      In summary, choose `if-else` for complex conditions, `switch` for discrete values of a single variable, and the
      `ternary operator` for simple conditional assignments.

19. **What is StringBuilder in java?**  
    `StringBuilder` in Java is a mutable sequence of characters that is used to create and manipulate strings more
    efficiently than the standard `String` class. Unlike `String`, which is immutable (meaning once created, its value
    cannot be changed), `StringBuilder` allows for dynamic modification of the character sequence without creating new
    objects.

    Key features of `StringBuilder`:
    - Mutable: You can modify the contents of a `StringBuilder` object without creating new instances.
    - Efficient: It is more efficient for operations that involve frequent modifications, such as appending, inserting,
      or deleting characters.
    - Not synchronized: `StringBuilder` is not thread-safe, making it faster than `StringBuffer`, which is synchronized
      and thread-safe.

    Common methods of `StringBuilder`:
    - `append(String str)`: Adds the specified string to the end of the current sequence.
    - `insert(int offset, String str)`: Inserts the specified string at the specified position.
    - `delete(int start, int end)`: Removes characters from the specified start index to the end index.
    - `replace(int start, int end, String str)`: Replaces characters in the specified range with the given string.
    - `toString()`: Converts the `StringBuilder` object to a `String`.

    Example:
    ```java
    StringBuilder sb = new StringBuilder("Hello");
    sb.append(" World");
    sb.insert(5, ",");
    System.out.println(sb.toString()); // Output: Hello, World
    ```

    In this example, we create a `StringBuilder` object, append a string to it, insert a comma, and then convert it to
    a `String` for output.
20. **What is StringBuffer in java?**  
    `StringBuffer` in Java is a mutable sequence of characters that is used to create and manipulate strings in a
    thread-safe manner. Similar to `StringBuilder`, `StringBuffer` allows for dynamic modification of the character
    sequence without creating new objects. However, unlike `StringBuilder`, `StringBuffer` is synchronized, making it
    safe for use in multi-threaded environments.

    Key features of `StringBuffer`:
    - Mutable: You can modify the contents of a `StringBuffer` object without creating new instances.
    - Thread-safe: It is synchronized, meaning that multiple threads can safely access and modify a `StringBuffer`
      object
      without causing data corruption.
    - Slightly slower: Due to its synchronization overhead, `StringBuffer` is generally slower than `StringBuilder`
      for
      single-threaded operations.

    Common methods of `StringBuffer`:
    - `append(String str)`: Adds the specified string to the end of the current sequence.
    - `insert(int offset, String str)`: Inserts the specified string at the specified position.
    - `delete(int start, int end)`: Removes characters from the specified start index to the end index.
    - `replace(int start, int end, String str)`: Replaces characters in the specified range with the given string.
    - `toString()`: Converts the `StringBuffer` object to a `String`.

    Example:
    ```java
    StringBuffer sb = new StringBuffer("Hello");
    sb.append(" World");
    sb.insert(5, ",");
    System.out.println(sb.toString()); // Output: Hello, World
    ```

    In this example, we create a `StringBuffer` object, append a string to it, insert a comma, and then convert it to
    a `String` for output.
21. **What are the differences between String, StringBuilder, and StringBuffer in java?**
    - `String`:
        - Immutable: Once created, the value of a `String` object cannot be changed. Any modification results in the
          creation of a new `String` object.
        - Thread-safe: Since `String` objects are immutable, they are inherently thread-safe.
        - Slower for modifications: Frequent modifications (like concatenation) can lead to performance issues due to
          the creation of multiple objects.
    - `StringBuilder`:
        - Mutable: Allows for dynamic modification of the character sequence without creating new objects.
        - Not synchronized: It is not thread-safe, making it faster than `StringBuffer` for single-threaded
          operations.
        - Efficient for modifications: Ideal for scenarios where frequent modifications are needed, such as in loops.
    - `StringBuffer`:
        - Mutable: Similar to `StringBuilder`, it allows for dynamic modification of the character sequence.
        - Synchronized: It is thread-safe, making it suitable for multi-threaded environments where multiple threads
          may access and modify the same object.
        - Slightly slower: Due to synchronization overhead, it is generally slower than `StringBuilder` for
          single-threaded operations.

    In summary, use `String` for fixed text that doesn't change, `StringBuilder` for efficient string manipulation in
    single-threaded scenarios, and `StringBuffer` when thread safety is required in multi-threaded environments.
22. **What is the concept of string pooling in java?**  
    String pooling in Java is a memory optimization technique that involves storing a single copy of each distinct
    string
    literal in a special area of memory called the "string pool" or "string intern pool." This pool is maintained by
    the
    Java Virtual Machine (JVM) to improve memory efficiency and performance when dealing with strings.

    When a string literal is created in Java, the JVM checks the string pool to see if an identical string already
    exists.
    If it does, the reference to the existing string is returned instead of creating a new string object. If the
    string
    does not exist in the pool, a new string object is created and added to the pool.

    Example:
    ```java
    String str1 = "Hello";
    String str2 = "Hello";

    System.out.println(str1 == str2); // Output: true
    ```
    In this example, both `str1` and `str2` refer to the same string object in the string pool, so the comparison
    using
    `==` returns `true`.

    The benefits of string pooling include:
    - Memory Efficiency: Reduces memory consumption by avoiding duplicate string objects.
    - Performance Improvement: Enhances performance by reusing existing string objects instead of creating new ones.

    Note that strings created using the `new` keyword are not stored in the string pool by default. However, you can
    explicitly add them to the pool using the `intern()` method.
    ```java
    String str3 = new String("Hello").intern();
    System.out.println(str1 == str3); // Output: true
    ```
    In this example, `str3` is created using the `new` keyword but is interned, so it refers to the same string
    object in the string pool as `str1`.
23. **What is the difference between == and equals() method for comparing strings?**
    - `==` Operator:
        - The `==` operator compares the references (memory addresses) of two string objects to determine if they point
          to
          the same object in memory.
        - It does not compare the actual content of the strings.
        - Example:
          ```java
          String str1 = new String("Hello");
          String str2 = new String("Hello");
          System.out.println(str1 == str2); // Output: false
          ```
          In this example, `str1` and `str2` are two different objects in memory, so the comparison using `==` returns
          `false`.
    - `equals()` Method:
        - The `equals()` method compares the actual content of two string objects to determine if they are equal in
          terms
          of their character sequences.
        - It returns `true` if the contents are the same, regardless of whether they are different objects in memory.
        - Example:
          ```java
          String str1 = new String("Hello");
          String str2 = new String("Hello");
          System.out.println(str1.equals(str2)); // Output: true
          ```
          In this example, although `str1` and `str2` are different objects, their contents are identical, so the
          comparison using `equals()` returns `true`.

    In summary, use the `==` operator to check if two string references point to the same object, and use the
    `equals()`
    method to compare the actual content of the strings for equality.
24. **What are the important methods of String class?**  
    The `String` class in Java provides a variety of important methods for manipulating and working with strings. Some
    of the most commonly used methods include:

    1. `length()`: Returns the length of the string (number of characters).
       ```java
       String str = "Hello";
       int len = str.length(); // len = 5
       ```
    2. `charAt(int index)`: Returns the character at the specified index.
       ```java
       char ch = str.charAt(1); // ch = 'e'
       ```
    3. `substring(int beginIndex, int endIndex)`: Returns a new string that is a substring of the original string.
       ```java
       String subStr = str.substring(1, 4); // subStr = "ell"
       ```
    4. `toLowerCase()`: Converts all characters in the string to lowercase.
       ```java
       String lowerStr = str.toLowerCase(); // lowerStr = "hello"
       ```
    5. `toUpperCase()`: Converts all characters in the string to uppercase.
       ```java
       String upperStr = str.toUpperCase(); // upperStr = "HELLO"
       ```
    6. `trim()`: Removes leading and trailing whitespace from the string.
       ```java
       String trimmedStr = "  Hello  ".trim(); // trimmedStr = "Hello"
       ```
    7. `replace(char oldChar, char newChar)`: Replaces all occurrences of a specified character with a new character.
       ```java
       String replacedStr = str.replace('l', 'x'); // replacedStr = "Hexxo"
       ```
    8. `indexOf(String str)`: Returns the index of the first occurrence of the specified substring.
       ```java
       int index = str.indexOf("ll"); // index = 2
       ```
    9. `equals(Object anObject)`: Compares the content of two strings for equality.
       ```java
       boolean isEqual = str.equals("Hello"); // isEqual = true
       ```
    10. `split(String regex)`: Splits the string into an array of substrings based on the specified delimiter.
        ```java
        String[] parts = "a,b,c".split(","); // parts = ["a", "b", "c"]
        ```
25. **What is an Array? Why we need arrays in real applications?**  
    An array in Java is a data structure that allows you to store multiple values of the same type in a single,
    contiguous
    block of memory. Each value in the array is called an element, and each element can be accessed using its index,
    which
    represents its position in the array (starting from 0).

    Arrays are useful in real applications for several reasons:
    - Efficient Data Storage: Arrays provide a way to store large amounts of data in a structured manner, allowing for
      efficient access and manipulation of the data.
    - Fixed Size: Once an array is created, its size is fixed, which can help manage memory usage and prevent
      unexpected
      growth of data structures.
    - Easy Access: Elements in an array can be accessed directly using their index, making it easy to retrieve or modify
      specific values.
    - Iteration: Arrays can be easily traversed using loops, allowing for efficient processing of all elements in the
      array.
    - Grouping Related Data: Arrays allow you to group related data together, making it easier to manage and work with
      collections of similar items.

    Example:
    ```java
    int[] numbers = new int[5]; // Declare an array of integers with a size of 5
    numbers[0] = 10; // Assign values to the array elements
    numbers[1] = 20;
    numbers[2] = 30;
    numbers[3] = 40;
    numbers[4] = 50;

    for (int i = 0; i < numbers.length; i++) {
        System.out.println(numbers[i]); // Output each element in the array
    }
    ```

    In this example, we create an array of integers, assign values to its elements, and then iterate through the array
    to
    print each value.
26. **How to declare and initialize an array in java?**  
    In Java, you can declare and initialize an array in several ways. Here are the common methods:

    1. Declaration and Initialization in Separate Steps:
       ```java
       int[] numbers; // Declare an array of integers
       numbers = new int[5]; // Initialize the array with a size of 5
       ```
    2. Declaration and Initialization in a Single Step:
       ```java
       int[] numbers = new int[5]; // Declare and initialize an array of integers with a size of 5
       ```
    3. Declaration and Initialization with Values:
       ```java
       int[] numbers = {10, 20, 30, 40, 50}; // Declare and initialize an array with specific values
       ```
    4. Using the `new` Keyword with Values:
       ```java
       int[] numbers = new int[]{10, 20, 30, 40, 50}; // Declare and initialize an array using the new keyword
       ```

    Example:
    ```java
    // Method 1: Separate declaration and initialization
    String[] fruits;
    fruits = new String[3];
    fruits[0] = "Apple";
    fruits[1] = "Banana";
    fruits[2] = "Cherry";

    // Method 2: Single step declaration and initialization
    String[] vegetables = new String[3];
    vegetables[0] = "Carrot";
    vegetables[1] = "Broccoli";
    vegetables[2] = "Spinach";

    // Method 3: Declaration and initialization with values
    String[] colors = {"Red", "Green", "Blue"};

    // Method 4: Using new keyword with values
    String[] animals = new String[]{"Dog", "Cat", "Bird"};
    ```

    In these examples, we demonstrate different ways to declare and initialize arrays of various types in Java.
27. **How to iterate over an array in java?**  
    In Java, you can iterate over an array using several methods. Here are some common ways to do so:

    1. Using a `for` loop:
       ```java
       int[] numbers = {10, 20, 30, 40, 50};
       for (int i = 0; i < numbers.length; i++) {
           System.out.println(numbers[i]); // Output each element in the array
       }
       ```
    2. Using an enhanced `for` loop (for-each loop):
       ```java
       int[] numbers = {10, 20, 30, 40, 50};
       for (int number : numbers) {
           System.out.println(number); // Output each element in the array
       }
       ```
    3. Using `Arrays.stream()` (Java 8 and later):
       ```java
       import java.util.Arrays;

       int[] numbers = {10, 20, 30, 40, 50};
       Arrays.stream(numbers).forEach(System.out::println); // Output each element in the array
       ```
    4. Using `while` loop:
       ```java
       int[] numbers = {10, 20, 30, 40, 50};
       int i = 0;
       while (i < numbers.length) {
           System.out.println(numbers[i]); // Output each element in the array
           i++;
       }
       ```
