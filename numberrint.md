The method rint returns the integer that is closest in value to the argument.

                         double rint(double d)
                         
The parameter d is a double as a parameter.

                        public class Test{
                         public static void main(String args[]) {
                         double d = 100.675;
                         double e = 100.500;
                         double f = 100.200;
                         
                         System.out.println(Math.rint(d));
                         System.out.println(Math.rint(e));
                         System.out.println(Math.rint(f));
                            }
                         }
                         
RESULT

                        101.0
                        100.0
                        100.0
