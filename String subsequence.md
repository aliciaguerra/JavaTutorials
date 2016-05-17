This method returns a new character sequence that is a subsequence of this sequence.

                  public CharSequence subSequence(int beginIndex, int endIndex)
 
 <h2>Parameters</h2>  
 beginIndex - the begin index, inclusive
 endIndex - the end index, exclusive
 
                  import java.io.*;
                  public class Test{
                  public static void main(String args[]){
                  String Str = new String("Welcome to Tutorialspoint.com");
                  System.out.print("Return Value:");
                  System.out.println(Str.subSequence(0,10));
                  System.out.print("Return Value");
                  System.out.println(Str.subSequence(10,15));
                      }
                  }

RESULT

                 Return Value :Welcome to
                 Return Value : Tuto
