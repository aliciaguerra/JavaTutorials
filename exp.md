The method returns the base of the natural logarithms, e, to the power of the argument.

                      double exp(double d)
                      
Example

                     public class Test {
                       public static void main(String args[]) {
                       double x = 11.653;
                       double y = 2.76;
                       
                       System.out.printf("The value of e is %.4f%n", Math.E);
                       System.out.printf("exp(%.3f) is %.3f%n", x, Math.exp(x));
                            }
                      }
                      
RESULT

                       The value of e is 2.7183.
                       exp(11.365) is 112983.831
