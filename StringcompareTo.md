There are two variants of this method. First method compares this String to another object and the second method compares
two strings lexicographically.

                        int compareTo(Object o)
                        int compareTo(String anotherString)
                        
<h2>Return Value</h2>
The value 0 if the argument is a string lexicographically equal to this string; a value less than zero if the argument
is a string lexicographically greater than this string; and a value greater than zero if the argument is a String 
lexicographically less than this String


                            public class Test {
                              public static void main(String args[]) {
                              String str1 = "Strings are immutable";
                              String str2 = "Strings are immutable";
                              String str3 = "Integers are immutable";
                              
                              int result = str1.compareTo(str2);
                              System.out.println(result);
                              
                              result = str2.compareTo(str3);
                              System.out.println(result);
                              
                              result = str3.compareTo(str1);
                              System.out.println(result);
                                }
                             }
                             
<h2>Result</h2>
                             0
                             10
                             -10
                              
                              
