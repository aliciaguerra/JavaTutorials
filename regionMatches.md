This method has two variants which can be used to test if two string regions are equal.

                      public boolean regionMatches(int offset, String other, int oofset, int len)
                      or
                      public boolean regionMatches(boolean ignoreCase, int toffset, String other, int ooffset, int len)
                      
EXAMPLE

                    import java.io.*;
                    public class Test {
                     public static void main(String args[]){
                      String Str1 = new String("Welcome to Tutorialspoint.com");
                      String Str2 = new String("Tutorials");
                      String Str3 = new String("TUTORIALS");
                      
                      System.out.println("Return Value:");
                      System.out.println(Str1.regionMatches(11, Str2, 0, 9));
                      
                      System.out.println("Return Value:");
