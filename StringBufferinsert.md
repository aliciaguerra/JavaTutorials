                      public StringBuffer insert(int offset, boolean b)
                      public StringBuffer insert(int offset, char c)
                      public insert(int offset, char[] str, int offset, int len)
                      public StringBuffer insert(int offset, float f)
                      public StringBuffer insert(int offset, int i)
                      public StringBuffer insert(int offset, long l)
                      public StringBuffer insert(int offset, Object o)
                      public StringBuffer insert(int offset, String str)
                      
EXAMPLE

                      public class Test {
                        public static void main(String args[]) {
                         StringBuffer sb = new StringBuffer("abcdefghijk");
                         sb.insert(3, "123");
                         System.out.println(sb);
                         }
                      }
                      
RESULT

                      abc123defghijk
