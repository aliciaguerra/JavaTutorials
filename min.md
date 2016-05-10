The method gives the smaller of the two arguments. The argument can be int, float, long, double.

                           double min(double arg1, double arg2)
                           double min(float arg1, float arg2)
                           double min(int arg1, int arg2)
                           long min(long arg1, long arg2)
                           
EXAMPLE

                        public class Test {
                          public static void main(String args[]){
                          System.out.println(Math.min(12.123, 12.456));
                          System.out.println(Math.min(23.12, 23.0));
                          }
                        }
                        
RESULT
          
                          12.123
                          23.0
