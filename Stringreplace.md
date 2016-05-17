This method returns a new String resulting from replacing all occurrences of oldChar with newChar.

                          public String replace(char oldChar, char newChar)
                          
EXAMPLE

                         import java.io.*;
                         public class Test {
                          public static void main(String args[]) {
                          String Str = new String("Welcome to Tutorialspoint.com");
                          System.out.println("Return Value");
                          System.out.println(Str.replace('o','T');
                          System.out.println("Return Value");
                          System.out.println(Str.replace('l', 'D'));
                              }
                          }

RESULT

                        Return Value :WelcTme tT TutTrialspTint.cTm
                        Return Value :WeDcome to TutoriaDspoint.com
