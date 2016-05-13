The method has different forms:

- public static String copyValueOf(char[] data) 
  Returns a String that represents the character sequence in the array specified.

- public static String copyValueOf(char[] data, int offset, int count)
  Returns a String that represents the character sequence in the array specified.
  
                             public static String copyValueOf(char[] data)
                             
                             or
                             
                             public static String copyValueOf(char[] data, int offset, int count)
                             
EXAMPLE

                            public class Test{
                             public static void main(String args[]){
                             char[] Str1 = {'h', 'e', 'l', 'l', 'o', ' ', 'w', 'o', 'r', 'l', 'd'};
                             String str2 = Str2.copyValueOf(Str1);
                             Str2 = Str2.copyValueOf(Str1, 2, 6);
                             System.out.println("Returned String" + Str2);
                                }
                            }
                            
RESULT

                             Returned String: hello world
                             Returned String: llo wo
