This method returns the specified double value.

                         double cos(double d)
                         
EXAMPLE

                       public class Test {
                        public static void main(String args[]) {
                         double degrees = 45.0;
                         double radians = Math.toRadians(degrees);
                         System.out.format("The value of pi is %.4f%n", Math.PI);
                         System.out.format("The cosine of %.1f degrees is %.4f%n", degrees, Math.cos(radians));
                           }
                       }
                       
RESULT

                      The value of pi is 3.1416.
                      The cosine of pi is 0.07071.
