This method is used to get the primitive data type of a certain string. parsexxx() is a static method that can have
one argument or two.

                              static int parseInt(String s)
                              static int parseInt(String s, int radix)
                              
<h2>Parameters</h2>
Here, is the detail of the parameters

- s -- the string representation of the decimal
- radix--this would be used to convert String s to integer

<h2>Return Value</h2>
- parseInt(String s) - this returns an integer (decimal only)
- parseInt(int i) - this returns an integer, given a string representation of decimal, binary, octal, or hexidecimal
  (radix equals 10, 2, 8 or 16 respectively) numbers as input
  
                               public class Test {
                                 public static void main(String args[]){
                                 int x = Integer.parseInt("9");
                                 double c = Double.parseDouble("5");
                                 int b = Integer.parseInt("444", 16);
                                 
                                 System.out.println(x);
                                 System.out.println(c);
                                 System.out.println(b);
                                   }
                                }
                                
This produces the following result:

                                  9
                                  5.0
                                  1092
