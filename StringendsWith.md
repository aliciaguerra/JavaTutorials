This method tests if the String ends from the specified suffix.

                       public boolean endsWith(String suffix)
                       
EXAMPLE

                      public class Test {
                       public static void main(String args[]) {
                       String Str = new String("This is not really immutable!");
                       boolean retVal;
                       
                       retVal = Str.endsWith("immutable!");
                       System.out.println("Returned Value = " + retVal);
                       
                       retVal = Str.endsWith("immu");
                       System.out.println("Returned Value = " + retVal);
                        }
                      }
                      
RESULT

                       Returned Value = true
                       Returned Value = false
