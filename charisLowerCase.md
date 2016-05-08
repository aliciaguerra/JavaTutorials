The method determines whether the specified char value is lowercase.

                          boolean isLowerCase(char ch)
                          
This method returns true if the passed character is really lower case.

                          public class Test {
                           public static void main(String args[]){
                           System.out.println(Character.isLowerCase('c'));
                           System.out.println(Character.isLowerCase('C'));
                           System.out.println(Character.isLowerCase('\n'));
                           System.out.println(Character.isLowerCase('\t'));
                              }
                          }
