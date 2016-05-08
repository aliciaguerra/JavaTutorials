This determines whether the specified char value is white space, which include space, tab, and new line.

                              boolean isWhiteSpace(char ch)
                              
This method returns true if passed character is really a white space.

                               public class Test {
                                public static void main(String args[]){
                                System.out.println(Character.isWhiteSpace('c');
                                System.out.println(Character.isWhiteSpace(' '));
                                System.out.println(Character.isWhiteSpace('\n'));
                                System.out.println(Character.isWhiteSpace('\t');
                                 }
                                }
  
