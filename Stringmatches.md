This method tells whether or not this String matches the given regular expression. An invocation of this method
of the form str.matches(regex) yields exactly the same result as the expression Pattern.matches(regex, str).

                         public boolean matches(String regex)
 
 EXAMPLE
 
                       import java.io.*;
                       public class Test {
                        public static void main(String args[]) {
                        String Str = new String("Welcome to Tutorialspoint.com");
                        
                        System.out.print("Return Value:");
                        System.out.println(Str.matches("(.*)Tutorials(.*)"));
                        
                        System.out.println("Return Value:");
                        System.out.println(Str.matches("Tutorials"));
                        
                        System.out.print("Return Value:");
                        System.out.println(Str.matches("Welcome(.*)"));
                              }
                        }
                        
                        
                         
