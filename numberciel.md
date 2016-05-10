The method ceil gives the smallest integer that is greater than or equal to the argument.

                               double ceil(double d)
                               double ceil(float f)
                               
The parameter is a float or double primitive data type.

                            public class Test {
                             public static void main(String args[]){
                             double d = -100.675;
                             float f = -90;
                             
                             System.out.println(Math.ceil(d));
                             System.out.println(Math.ceil(f));
                             System.out.println(Math.ceil(d));
                             System.out.println(Math.ceil(f));
                               }
                            }
                             
RESULT

                             -100.0
                             -90.0
                             -101.0
                             -90.0
                             
