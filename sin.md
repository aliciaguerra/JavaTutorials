The method returns the sine of the specified souble value.

                       double sin(double d)
                       
EXAMPLE

           public class Test {
            public static void main(String args[]) {
             double degrees = 45.0;
             double radians = Math.toRadians(degrees);
             System.out.format("The value of pi is %.4f%n", Math.PI);
             System.out.format("The sine of %.1f degrees is %.4f%n", degrees, Math.sin(radians));
              }
            }
            
RESULT

            The value of pi is 3.1416.
            The sine of 45.0 degrees is 0.7071
