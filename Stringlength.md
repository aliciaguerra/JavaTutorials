This method returns the length of this string. The length is equal to the number of 16-bit Unicode characters in
the String.

                            public int length()
                            
EXAMPLE

                          import java.io.*;
                          public class Test {
                           public static void main(String args[]) {
                           String Str1 = new String("Welcome to Tutorialspoint.com");
                           String Str2 = new String("Tutorials");
                           
                           System.out.print("String Length:");
                           System.out.println(Str1.length());
                           
                           System.out.print("String Length:");
                           System.out.println(Str2.length());
                              }
                          }
                          
RESULT

                         String Length: 29
                         String Length: 9
