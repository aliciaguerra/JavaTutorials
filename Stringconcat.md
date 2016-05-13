This method returns one string at the end of another. The method returns a String with the value of the String 
passed into the method appeneded to the end of the String used to this method.

                       public String concat(String s)
                       
EXAMPLE

                        public class Test {
                          public static void main(String args[]) {
                           String s = "Strings are immutable";
                           s = s.concat(" all the time.");
                           System.out.println(s);
                            }
                        }
                        
RESULT

                         Strings are immutable all the time.
