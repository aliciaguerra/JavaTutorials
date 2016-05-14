This method compares this String to another string, ignoring case considerations. Two strings are considered equal ignoring 
case if they are of the same length, and corresponding characters in the two Strings are equal ignoring case.

                   public boolean equalsIgnoreCase(String anotherString)
                   
EXAMPLE

                   public class Test {
                     public static void main(STring args[]) {
                      String Str1 = new String("This is really not immutable!!");
                      String Str2 = Str1;
                      String Str3 = new String("This is really not immutable!!");
                      String Str4 = new String("THIS IS REALLY NOT IMMUTABLE!");
                      boolean retVal;
                      
                      retVal = Str1.equals(Str2);
                      System.out.println("Returned Value =" + retVal);
                      
                      retVal = Str2.equals(Str3);
                      System.out.println("Returned Value =" + retVal);
                      
                      retVal = Str1.equalsIgnoreCase(Str4);
                      System.out.println("Returned Value =" + retVal);
                        }
                    }
                    
RESULT

                      Returned Value = true
                      Returned Value = true
                      Returned Value = true
