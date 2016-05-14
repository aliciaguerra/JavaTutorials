- public int indexOf(int ch)
  Returns the index within this String of the first occurrence of the specified character or -1 if the character does not
  occur
- public int indexOf(int ch, int fromIndex) 
  Returns the index within this String of the first occurrence of the specified character, starting the search at the 
  specified character, starting the search at the specified index or -1 if the character does not occur
- int indexOf(String str)
  Returns the index within this string of the first occurrence of the specified substring. If it does not occur as a 
  substring,-1 is returned.
- int indexOf(String str, int fromIndex)
  Returns the index within this String of the first occurence of the specified substring, starting at the specified index. 
  If it does not occur, -1 is returned.
  
                         public int indexOf(int ch)
                         
                         or
                         
                         public int indexOf (int ch, int fromIndex)
                         
                         or 
                         
                         int indexOf(String str)
                         
                         or
                         
                         int indexOf(String str, int fromIndex)
                         
EXAMPLE

                  import jav.io.*;
                  public class Test {
                   public static void main(String args[]) {
                    String Str = new String("Welcome to tutorialspoint.com");
                    String SubStr1 = new String("Tutorials");
                    String SubStr2 = new String("Sutorials");
                    
                    System.out.println("Found Index : ");
                    System.out.println(Str.indexOf('o'));
                    System.out.println("Found Index:");
                    System.out.println(Str.indexOf('o', 5));
                    System.out.println("Found Index:");
                    System.out.println(Str.indexOf(SubStr1));
                    System.out.println("Found Index:");
                    System.out.println(Str.indexOf(SubStr1, 15));
                    System.out.println("Found Index:");
                    System.out.println(Str.indexOf(SubStr2));
                             }
                    }
                    
RESULT      

                   Found Index: 4
                   Found Index: 9
                   Found Index: 11
                   Found Index: -1
                   Found Index: -1
                         
