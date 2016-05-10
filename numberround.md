This method round returns the closest long or int, as given by the method's return type.
   
                              long round(double d)
                              int round(float f)
                              
takes in a double or float, returns the closest long or int

                                 public class Test {
                                   public static void main(String args[]) {
                                    double d = 100.675;
                                    double e = 100.500;
                                    float f = 100;
                                    float g = 90f;
                                    
                                    System.out.println(Math.round(d));
                                    System.out.println(Math.round(e));
                                    System.out.println(Math.round(f));
                                    System.out.println(Math.round(g));
                                      }
                                    }
                                    
RESULT

                               101
                               101
                               100
                               90
