This method copies characters from this String into the destination character array.

                     public void getChars(int srcBegin, int srcEnd, char[] dst, int dstBegin);
                     
EXAMPLE

                 import java.io.*;
                 public class Test {
                  public static void main(String args[]) {
                   String Str1 = new String("Welcome to TutorialsPoint.com");
                   char[] Str2 = new char[7];
                   
                   try {
                     Str1.getChars(2, 9, Str2, 0);
                     System.out.println("Copied Value=");
                     System.out.println(Str2);
                     
                     } catch(Exception e) {
                      System.out.println("Raised exception");
                          }
                     }
                     
RESULT

                     Copied Value = lcome t
