The method is used to get a String object representing the value of the Number object.

If the method takes a primitive data type as an argument, then the String object representing the primtive data 
type value is returned.

If the method takes two arguments, then a String representation of the first argument in the radix specified 
by the second argument will be returned.

                         String toString()
                         static String toString(int i)
                         
<h2>Parameters</h2>
- i - an int for which string representation would be returned
 
                         public class Test {
                             public static void main(String args[]){
                             Integer x=5;
                             System.out.println(x.toString());
                             System.out.println(Integer.toString(12));
                               }
                          }
 
<h2>RESULT</h2>
5

12
