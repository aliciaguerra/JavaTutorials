This method converts the value of the Number Object that invokes the method to the primitive data type that is returned
from the method.

Here is a separate emthod for each primitive data type:

                                       byte byteValue()
                                       short shortValue()
                                       int intValue()
                                       long longValue()
                                       float floatValue()
                                       double doubleValue()
                                       
All of these are default methods and accepts no parameter.

                                     public class Test {
                                      public static void main(String args[]){
                                      Integer x = 5;
                                      //Returns byte primtiive data type
                                      System.out.println(x.byteValue());
                                      //Returns double primitive data type
                                      System.out.println(x.doubleValue());
                                      //Return long primitive data type
                                      System.out.println(x.longValue());
                                          }
                                      }
                                      
                                      //RESULT
                                      //5
                                      //5.0
                                      //5
