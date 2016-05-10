The method returns the value of the first argument raised to the power of the second argument.

                      double pow(double base, double exponent)
                      
EXAMPLE

                    public class Example {
                     public static void main(String args[]) {
                      double x = 11.635;
                      double y = 2.76;
                      
                      System.out.printf("The value of e is %.4f%n", Math.E);
                      System.out.printf("pow(%.3f, %.3f) is %.3f%n", x, y, Math.pow(x,y));
                         }
                    }
                    
RESULT

                    The value of e is 2.7183.
                    pow(11.365, 2.760) is 874.008
