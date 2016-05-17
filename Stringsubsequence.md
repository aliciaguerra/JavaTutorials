This method has two variants and returns a new String that is the substring of this string. The substring begins with the
character at the specified index and extends to the end of this String or up to endIndex-1 if second argument is given.

                 public String substring(int beginIndex)
                 or
                 public String substring(int beginIndex, int endIndex)
                 
<h2>EXAMPLE</h2>                 

                 import java.io.*;
                 public class Test {
                 public static void main(String args[]){
                 String Str=new String("Welcome to Tutorialspoint.com");
                 System.out.print("Return Value:");
                 System.out.println(Str.substring(10));
                 System.out.print("Return Value:");
                 System.out.println(Str.substring(10,15));
                     }
                 }
                 
RESULT

                Return Value : Tutorialspoint.com
                Return Value : Tuto
