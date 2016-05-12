This method reverses the value of the StringBuffer object that invoked the method.

Let n be the length of the old character sequence, the one contained in the StringBuffer just prior to the execution
of the reverse method. Then, the character at index k in the new character sequence is equal to the character at index
n-k-1 in the old character sequence.

                     public StringBuffer reverse()
                     
EXAMPLE

                     public class Test {
                      public static void main(String args[]) {
                       StringBuffer buffer = new StringBuffer("Game Plan");
                       buffer.reverse();
                       System.out.println(buffer);
                        }
                     }
                     
RESULT

                     nalP emaG
