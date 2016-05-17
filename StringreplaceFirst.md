This method replaces the first substring of this string that matches the given regular expression with the given replacement.

                public String replaceFirst(String regex, String replacement)
                
EXAMPLE

                 import java.io.*;
                 public class Test {
                 public static void main(String args[]) {
                 String Str = new String("Welcome to Tutorialspoint.com");
                 System.out.println("Return Value:");
                 System.out.println(Str.replaceFirst(Str.replaceFirst("(.*)Tutorials(.*)", "AMROOD"));
                 System.out.println("Return Value:");
                 System.out.println(Str.replaceFirst("Tutorials", "AMROOD"));
                 
  RESULT
  
                Return Value :AMROOD
                Return Value :Welcome to AMROODpoint.com
