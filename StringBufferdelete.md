This method removes the characters in a substring of this StringBuffer. The substring begins at the specified start 
and extends to the character at the index end -1 or to the end of the StringBuffer if no such character exists.

If start is equal to end, no changes are made.

                   public StringBuffer delete(int start, int end)
                   
EXAMPLE

                    public class Test {
                      public static void main(String args[]) {
                       StringBuffer sb = new StringBuffer("abcdefghijk");
                       sb.delete(3,7);
                       System.out.println(sb);
                         }
                      }
                      
RESULT

                     abchijk
