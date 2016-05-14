This method compares this String to then specified object. The result is true if and only if the argument is not null
and is a String object that represents the same sequence of characters as this object.

                        public boolean equals(Object anObject)
                        
EXAMPLE

                         public class Test {
                          public static void main(String args[]) {
                          String Str1 = new String("This is really not immutable!");
                          String Str2 = Str1;
                          String Str3 = new String("This is really not immutable!");
                          boolean retVal;
                          
                          retVal = Str1.equals(Str2);
                          System.out.println("Returned Value =" + retVal);
                          
                          retVal = Str1.equals(Str3);
                          System.out.println("Returned Value =" + retVal);
                                  }
                          }
                          
RESULT

                        Returned Value = true
                        Returned Value = true
                          
                          
                          
