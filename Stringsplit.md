This method has two variants and splits this string around matches of the given regular expression.
limit is the threshold of Strings that can be returned.

                  public String[] split(String regex, int limit)
                  or
                  public String[] split(String regex)
                  
EXAMPLE

                  import java.io.*;
                  public class Test {
                   public static void main(String args[]) {
                   String Str = new String("Welcome-to-tutorials.com");
                   
                   System.out.println("Return Value:");
                   for(String retval: Str.split("-",2));
                   System.out.println(retVal);
                   }
                   System.out.println("");
                   System.out.println("Return Value:");
                   System.out.println("-", 3)) {
                   System.out.println(retVal);
                   }
                   System.out.println("");
                   System.out.println("Return Value:");
                   for(String retVal: Str.split("-",0)) {
                   System.out.println(retVal);
                   }
                   System.out.println("");
                   System.out.println("Return Value:");
                   for(String retVal: Str.split("-")){
                   System.out.println(retVal);
                        }
                     }
                  }
                  
RESULT

                  Return Value :
                  Welcome
                  to-Tutorialspoint.com

                  Return Value :
                  Welcome
                  to
                  Tutorialspoint.com

                  Return Value:
                  Welcome
                  to
                  Tutorialspoint.com

                  Return Value :
                  Welcome
                  to
                  Tutorialspoint.com
