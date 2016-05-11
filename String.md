String, which are widely used in Java programming, are a String of Characters. In the Java programming language,
Strings are objects.

The Java platform provides the String class to create and manipulate strings.

<h2>Creating Strings</h2>
The most direct way to create a String is to write:

                  String greeting "Hello World!";
                  
Whenever it encounters a String literal in your code, the compiler creates a String object with a value in this case 
"Hello World!".

As with any other object, you can create String objects by using the new keyword and a constructor. The String class has
eleven constructors that allow you to provide the initial value of the String using different sources, such as an array of
characters.

                   public class StringDemo {
                     public static void main(String args[])
