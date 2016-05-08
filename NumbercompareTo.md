This method compares the Number object that invoked the method to the argument. It is possible to cpmare Byte, Long,
Integer, etc.

However, two different types cannot be compared, both the argument and the Number object invokign the method should be the
same type.

                           public int compareTo(NumberSubClass referenceName)
                           
<h2>Parameters</h2>
referenceType - This could be a Byte, Double, Integer, Float, Long, or short.

<h2>Return Value</h2>

- If the integer is equal to the argument then 0 is returned.
- If the integer is less than the argument then -1 is returned.
- If the integer is greater than the argument then 1 is returned.

                            public class Test {
                             public static void main(String args[]) {
                              Integer x = 5;
                              System.out.println(x.compareTo(3));
                              System.out.println(x.compareTo(5));
                              System.out.println(x.compareTo(8));
                                }
                              }
                              
                            //RESULT:
                            //1
                            //0
                            //-1
