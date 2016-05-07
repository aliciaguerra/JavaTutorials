Normally, when we work with characters, we use primitive data types char. 

                             char c='a';
                             //Unicode for uppercase Greek omega character
                             char uniChar='\u039A';
                             //an array of characters
                             char[] charArray = {'a', 'b', 'c', 'd', 'e'};
                             
However, in development, we come across situations where we need to use objects instead of primitive data types.
In order to achieve this, Java provides a wrapper class Character for the primtiive data type char. 

The Character class offers a number of useful class (i.e. static) methods for maniuplating characters. You create a
Character object with the Character constructor:

                              Character ch = new Character('a');
                              
The Java compiler will also create a Character object for you under some circumstances. For example, if you pass a primitive
char into a method that expects an object, the compiler automatically converts the char into a Character for you. This feature is called autoboxing or unboxing, if the conversion goes the other way.

                             //Here following primitive char 'a'
                             //is boxed into the Character object ch
                             Character ch = 'a';
                             //Here primitive 'x' is boxed for method test,
                             //return is unboxed to char c
                             char c = test('c');
                             
Escape Sequences
A character represented by a backslash (\) is an escape character that has special meaning to the compiler.

The newline character (\n) has been used frequently in this tutorial in System.out.println() statements to advance to the next line after the string is processed.

- \t inserts a tab in the text at this point
- \b inserts a backspace into this text at this point
- \n inserts a newline in the text at this point
- \r inserts a carriage return at this point
- \f inserts a form feed in the text at this particular point
- \' inserts a single quote character in the text at this point
- \" inserts a double quote character in the text a this point
- \\ inserts a backslash character in the text at this point

When an escape sequence is encountered in a print statement, the compiler interprets it accordingly.

<h2>Example</h2>
If you want to put quotes within quotes, you must use the escape sequence, \" on the interior quotes:

                                public class Test {
                                  public static void main(String args[]){
                                   System.out.println("She said \"Hello!\" to me.");
                                     }
                                }
                                
  <h2>Character Methods</h2>
  Here is the list of important instance methods that all the subclasses of the Character class implement:
  
