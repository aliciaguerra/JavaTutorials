This method returns a copy of the string, with leading and trailing whitespace omitted. 

                                  public String trim()
                                  
EXAMPLE

                                 import java.io.*;
                                 public class Test {
                                  public static void main(String args[]) {
                                   String Str = new String("Welcome to tutorialspoint.com      ");
                                   System.out.print("Return Value:");
                                   System.out.println(Str.trim());
                                     }
                                 }
                                 
RESULT

                                    Return Value :Welcome to Tutorialspoint.com
