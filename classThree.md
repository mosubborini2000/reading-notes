The difference between an "int" and an "Integer" in Java:

"int" is a primitive data type that represents a 32-bit signed integer.
"Integer" is a class in the Java standard library that wraps an "int" value into an object. This is known as boxing.
Default value for ints and Integers:

The default value for an "int" is 0.
The default value for an "Integer" is null since it's an object.
Autoboxing and Unboxing:

Autoboxing is the automatic conversion that the Java compiler makes between primitive types and their corresponding object wrapper classes. For example, converting an "int" to an "Integer" automatically.
Unboxing is the reverse process, where the Java compiler automatically converts an object of a wrapper class to its corresponding primitive type.
Exceptions in Java:

Three basic categories of exceptions:

Checked Exceptions: These are exceptions that are checked at compile-time. They are subclasses of Exception but not of RuntimeException. Examples include IOException and SQLException.
Unchecked Exceptions (Runtime Exceptions): These exceptions do not need to be explicitly caught or declared in the method. They are subclasses of RuntimeException. Examples include NullPointerException and ArrayIndexOutOfBoundsException.
Errors: These are exceptional conditions that are external to the application, and the application usually cannot anticipate or recover from them. Examples include OutOfMemoryError and StackOverflowError.
Statement to handle an exception:

To handle an exception, you use a try-catch block. The try block contains the code that might throw an exception, and the catch block contains the code to handle that exception if it's thrown.
Using Scanner to read in a file in Java:

Situation where Scanner would be useful:

Scanner can be useful when you want to read and process text data from various sources, such as reading data from a user input, reading data from a file, or parsing text from a web page.
Input from a Scanner is broken down into:

Input from a Scanner is broken down into tokens. Tokens are individual units of input, such as words or numbers, separated by delimiters like spaces, commas, or newlines. You can use methods like next(), nextInt(), nextLine() to retrieve these tokens from the input.
and here is example about it :


        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = scanner.nextLine(); 
        System.out.print("Enter your age: ");
        int age = scanner.nextInt(); 
        System.out.println("Hello, " + name + "! You are " + age + " years old.");

        but I'm as prefer to use :

 String input = JOptionPane.showInputDialog("Enter a number:");

 ## Things I want to know more about
actually I want to learn more about inteliJ and jdk and how to connect with Gradle
