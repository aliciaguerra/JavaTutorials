This method returns a hashcode for this String. The hash code for  String object is computed as:
s[0]*31^(n-1) + s[1]*31^(n-2) + ... + s[n-1]

Using int arithmetic , where s[i] is the ith character of the String, n is the length of the String, and ^ indicates 
exponentiation. (the hash value of the empty string is zero)

                          public int hashCode()
                          
EXAMPLE

                          import java.io.*;
                          public class Test {
                           public static void main(String args[]) {
                           String Str = new String("Welcome to TutorialsPoint.com");
                           System.out.println();
                           System.out.println("Hashcode for Str:" + Str.hashCode());
                                 }
                          }
                          
RESULT

                          Hashcode for Str :1186874997
