- int lastIndexOf(int ch)
  Returns the index within this String of the last occurrence of the specified character or -1 if the character does
  not occur
- public int lastIndexOf(int ch, int fromIndex)
  Returns the index of the last occurrence of the character in the character sequence represented by this object
  that is less than or equal to fromIndex, or -1 if the character does not occur before that point
- public int lastIndexOf(String str)
  If the string argument occurs one or more times as a substring within this object, then it returns the index as a
  first character of the last such substring is returned. If it does not occcur as a substring, -1 is returned.
- public int lastIndexOf(String str, int fromIndex)
  Returns the index within this String of the last occurrence of the specified substring, searching backwards starting
  at the specified index.
  
                    int lastIndexOf(int ch)
                    public int lastIndexOf(int ch, int fromIndex)
                    public int lastIndexOf(String str)
                    public int lastIndexOf(String str, int fromIndex)
                    
EXAMPLE

                    import java.io.*;
                    public class Test {
                     public static void main(String args[]) {
                     String Str = new String("Welcome to Tutorialspoint.com");
                     String SubStr1 = new String("Tutorials");
                     String SubStr2 = new String("Sutorials");
                     
                     System.out.print("Found Last Index:");
                     System.out.println(Str.lastIndexOf('o'));
                     System.out.print("Found Last Index:");
                     System.out.println(Str.lastIndex('o', 5));
                     System.out.print("Found Last Index:");
                     System.out.println(Str.lastIndexOf(SubStr1));
                     System.out.print("Found Last Index");
                     System.out.println(Str.lastIndexOf(SubStr1, 15));
                     System.out.print("Found Last Index:");
                     System.out.println(Str.lastIndexOf(SubStr2));
                                }
                    }
                    
RESULT

                        Found Last Index :27
                        Found Last Index :4
                        Found Last Index :11
                        Found Last Index :11
                        Found Last Index :-1
