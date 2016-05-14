This method returns a canonical representation for the String object. It follows that for any two strings s and t, 
s.intern() == t.intern() is true if and only if s.equals(t) is true.

                        public String intern()
                        
EXAMPLE

                    import java.io.*;
                    public class Test {
                    public static void main(String args[]) {
                    String Str1 = new String("Welcome to TutorialsPoint.com");
                    String Str2 = new String("WELCOME TO SUTORIALSPOINT.COM");
                    
                    System.out.println("Canonical Representation:");
                    System.out.println(Str1.intern());
                    
                    System.out.println("Canonical Representation:");
                    System.out.println(Str2.intern());
                                   }
                    }
                    
EXAMPLE:

                     Canonical representation: Welcome to Tutorialspoint.com
                     Canonical representation: WELCOME TO SUTORIALSPOINT.COM
