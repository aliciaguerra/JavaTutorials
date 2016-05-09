This method gives the absolute value of the argument. The argument can be int, float, long, double, short, byte.

                           double abs(double d)
                           float abs(float f)
                           int abs(int i)
                           long abs(long lg)
                           
The parameter is any primitive data type.

                          public class Test {
                            public static void main(String args[]){
                            Integer a =-8;
                            double d=-100;
                            float f=-90;
                            System.out.println(Math.abs(a));
                            System.out.println(Math.abs(d));
                            System.out.println(Math.abs(f));
                             }
                            }
                            
                            //RESULT
                            //8
                            //100.0
                            //90.0
