This method compares two strings lexicographically, ignoring case differences. 

                    int compareToIgnoreCase(String str)
                    
<h2>Example</h2>

                   public class Test {
                     public static void main(String args[]) {
                      String str1 = "Strings are immutable";
                      String str2 = "Strings are immutable";
                      String str3 = "Integers are not immutable";
                      
                      int result = str1.compareToIgnoreCase(str2);
                      System.out.println(result);
                      
                      result = str2.compareToIgnoreCase(str3);
                      System.out.println(result);
                      
                      result = str3.compareToIgnoreCase(str1);
                      System.out.println(result);
                        }
                    }
                    
RESULT

                    0
                    10
                    -10
