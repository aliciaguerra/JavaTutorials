The valueOf method returns the relevant Number object holding the value of the argument passed. The argument can be a 
primitive data type, string, etc. The argument can be a primitive data type, String, etc.

This method is a static method. The method can take two arguments, where one is a String and the other is a radix.

                            static Integer valueOf(int i)
                            static Integer valueOf(String s)
                            static Integer valueOf(String s, int radix)
                            
<h2>Parameters</h2>
- i- An int for which Integer representation would be returned
- s- A string for which Integer representation would be returned
- radix-This would be used to decide the value of returned Integer based on passed String

<h2>Return Value</h2>
- valueOf(int i)-This returns an Integer object holding the value of a specified primitive.
- valueOf(String s)-This returns an Integer object holding the value of the specified String representation.
- valueOf(String s, int radix)- This returns an Integer object holding the integer value of the specified string 
  representation, parsed with the value of the radix
  
                              public class Test{
                               public static void main(String args[]) {
                                Integer x = Integer.valueOf(9);
                                Double c = Double.valueOf(5);
                                Float a = Float.valueOf("80");
                                
                                Integer b = Integer.valueOf("444",16);
                                
                                System.out.println(x);
                                System.out.println(c);
                                System.out.println(a);
                                System.out.println(b);
                                    }
                              }
                              
This produces the following result:

                              9
                              5.0
                              80.0
                              1092
                              

