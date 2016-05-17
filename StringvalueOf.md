This method has the following variants, which depend on the passed parameters. This method returns the String representation
of the passed argument.

- valueOf(boolean b) Returns the String representation of the boolean argument)
- valueOf(char c) Returns the String representation of the char argument.
- valueOf(char[] data) Returns the String representation of the char arrsay argument.
- valueOf(char[] data, int offset, int count) Returns the string representation of a specific subarray of the char array
  argument
- valueOf(double d)  Returns the String representation of the double argument
- valueOf(float f) Returns the String representation of the float argument
- valueOf(int i) Returns the String representation of the int argument
- valueOf(long l) Returns the String representation of the long argument
- valueOf(Object o) Returns the String representation of the Object argument

EXAMPLE

                           import java.io.*;

                          public class Test{
                           public static void main(String args[]){
                            double d = 102939939.939;
                             boolean b = true;
                             long l = 1232874;
                           char[] arr = {'a', 'b', 'c', 'd', 'e', 'f','g' };
 
                           System.out.println("Return Value : " + String.valueOf(d) );
                            System.out.println("Return Value : " + String.valueOf(b) );
                           System.out.println("Return Value : " + String.valueOf(l) );
                           System.out.println("Return Value : " + String.valueOf(arr) );
                                 }
                           }
                           
RESULT

                        Return Value : 1.02939939939E8
                        Return Value : true
                        Return Value : 1232874
                        Return Value : abcdefg
