This method has two variants and tests if a string starts with the specified prefix beginning a specified prefix or 
by default at the beginning.

                         public boolean startsWith(String prefix)
                         or
                         public boolean startsWith(String prefix)
                         
<h2>Parameters</h2>   
- prefix-the prefix to be matched
- toffset-where to begin looking in the string

EXAMPLE
 
                         import java.io.*;
                         public class Test {
                         public static void main(String args[]){
                         String str=new String("Welcome to Tutorialspoint.com");
                         System.out.print("Return Value");
                         System.out.println(Str.startsWith("Welcome"));
                         System.out.print("Return Value:");
                         System.our.println(Str.startsWith("Tutorials"));
                         System.out.print("Return Value:");
                         System.out.println(Str.startsWith("Tutorials", 11));
                            }
                         }
                         
RESULT

                        Return Value :true
                        Return Value :false
                        Return Value :true
