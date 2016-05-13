This method returns true if and only if this String represents the same sequence of characters as specified in
the StringBuffer.

                           public boolean contentEquals(StringBuffer sb)
                           
EXAMPLE

                          public class Test {
                           public static void main(String args[]) {
                            String str1 = "Not immutable";
                            String str2 = "Strings are immutable";
                            StringBuffer str3 = new StringBuffer("Not immutable");
                            
                            boolean result = str2.contentEquals(str3);
                            System.out.println(result);
                            
                            result = str2.contentEquals(str3);
                            System.out.println(result);
                               }
                          }
                          
RESULT
                          
                          true
                          false
