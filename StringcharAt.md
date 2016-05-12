This method returns the character located at the String's specified index. The String indexes start from zero.

                      public char charAt(int index)
                      
EXAMPLE

                       public class Test {
                        public static void main(String args[]) {
                         String s = "Strings are immutable";
                         char result = s.charAt(8);
                         System.out.println(result);
                          }
                       }
                       
RESULT

                       a
