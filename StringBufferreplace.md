This method replaces the characters in a substring of this StringBuffer with characters in the specified String.

The substring begins at the specified start and extends to the character at index end -1 or to the end of the StringBuffer
if no such character exists. First the characters in the substring are removed and then the specified String is inserted
at start.

                   public StringBuffer replace(int start, int end, String str)
                   
EXAMPLE

                   public class Test {
                    public static void main(String args[]) {
                    StringBuffer sb = new StringBuffer("abcdefghijk");
                    sb.replace(3, 8, "ZARA");
                    System.out.println(sb);
                     }
                   }
                   
RESULT
   
                  abcZARAijk
                  
            
