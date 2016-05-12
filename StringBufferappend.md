This method updates the value of the object that invoked the method. The method takes boolean, char, int, long, Strings, etc.

                        public StringBuffer append(boolean b)
                        public StringBuffer append(char c)
                        public StringBuffer append(char[] str)
                        public StringBuffer append(char[] str, int offset, int len)
                        public StringBuffer append(double d)
                        public StringBuffer append(float f)
                        public StringBuffer append(int i)
                        public StringBuffer append(long l)
                        public StringBuffer append(object o)
                        public StringBuffer append(StringBuffer sb)
                        public StringBuffer append(String str)
                        
EXAMPLE

                 public class Test {
                  public static void main(String args[]) {
                   StringBuffer sb = new StringBuffer("Test");
                   sb.append("StringBuffer");
                   System.out.println(sb);
                    }
                 }
                
RESULT

                  Test String Buffer
