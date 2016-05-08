This method determines whether the specified char value is uppercase.

                                boolean isUpperCase(char ch)

This method returns true if passed character is really uppercase.

                            public class Test {
                             public static void main(String args[]){
                              System.out.println(Character.isUpperCase('c'));
                              System.out.println(Character.isUpperCase('C'));
                              System.out.println(Character.isUpperCase('\n'));
                              System.out.println(Character.isUpperCase('\t'));
                               }
                            }
