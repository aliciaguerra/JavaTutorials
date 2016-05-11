The method returns the tangent of the specified double value.

                        double tan(double d)
                        
EXAMPLE

                      public class Test {
                       public static void main(String args[]) {
                        double degrees = 45.0;
                        double radians = Math.toRadians(degrees);
                        System.out.format("The value of pi is %.4f%n", Math.PI);
                        System.out.format("The tangent of %.1f degrees is %.4f%n", degrees, Math.tan(radians));
                            }
                      }
                      
RESULT

                      The value of pi is 3.1416.
                      The tangent of 45.0 degrees is 1.000.
