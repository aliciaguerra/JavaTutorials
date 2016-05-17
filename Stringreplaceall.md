This method replaces each substring of this string that matches the given regular expression with the given replacement.

                      public String replaceAll(String regex, String replacement)
                      
EXAMPLE
    
                    import java.io.*;
                    public class Test {
                     public static void main(String args[]) {
                     String Str = new String("Welcome to Tutorialspoint.com");
                     System.out.println("Return value");
                     System.out.println(Str.replaceAll(Str.replaceAll("(.*)Tutorials(*)", "AMROOD")));
                         }
                    }
                    
RESULT

                 Return Value :AMROOD
