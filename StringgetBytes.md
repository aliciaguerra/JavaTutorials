getBytes(String charsetName): Encodes this String into a sequence of bytes using the name charset, storing the result
into a new byte array.

getBytes(): Encodes this String into a sequence of bytes using the platform's default charset, storing the result 
into a new byte array.

                    public byte[] getBytes(String charsetName) throws UnsupportedEncodingException
                    or 
                    public byte[] getBytes()
                    
EXAMPLE
   
                   import java.io.*;
                   public class Test {
                    public static void main(String args[]) {
                    String Str1 = new String("Welcome to tutorialspoint.com");
                    
                    try {
                    byte[] Str2 = Str1.getBytes();
                    System.out.println("Returned Value" + Str2);
                    
                    Str2 = Str1.getBytes("UTF-8");
                    System.out.println("Returned Value" + Str2);
                    
                    Str2 = Str1.getBytes("ISO-8859-1");
                    System.out.println("Returned Value" + Str2);
                    
                    } catch(UnsupportedEncodingException e) {
                    System.out.println("Unsupported chracter set");
                              }
                          }
                    }
                    
RESULT

                     Returned  Value [B@192d342
                     Returned  Value [B@15ff48b
                     Returned  Value [B@1b90b39
                    
