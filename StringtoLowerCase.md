This method has two variants. First variant converts all of the characters in the Stringto lower case using the rules
of the given Locale. This is the equivalent to calling toLowerCase(Locale.getDefault()).

Second variant takes the locale as an argument to be used while converting to lowercase.

                       public String toLowerCase()
                       or
                       public String toLowerCase(Locale locale)
                       
EXAMPLE
  
                        import java.io.*;
                        public class Test {
                         public static void main(String args[]){
                         String Str = new String("Welcome to Tutorialspoint.com");
                         System.out.println("Return Value:");
                         System.out.println(Str.toLowerCase());
                             }
                        }
                        
RESULT

                         Return Value :welcome to tutorialspoint.com
