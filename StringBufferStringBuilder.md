The StringBuffer and StringBuilder classes are used when there is a necessity to make a lot of modifications to Strings 
of characters. 

Unlike Strings, objects of type StringBuffer and StringBuilder can be modified over and over again without leaving behind a 
lot of new unused objects. 

The StringBuilder class was introduced as of Java 5 and the main difference between the StringBuffer andf StringBuilder is 
that StringBuilder methods are not thread safe (not synchronized).

It is recommended to use StringBuilder whenever possible because it is faster than StringBuffer. However, if thread safety
is necessary, the best option is StringBuffer objects.

                       public class Test {
                        public static void main(String args[]) {
                         StringBuffer sBuffer = new StringBuffer("test");
                         sBuffer.append("String buffer");
                         System.out.println(sBuffer);
                          }
                       }
                       
<h2>StringBuffer Methods</h2>
- public StringBuffer append(String s) Updates the value of the object that invoked the method. This method takes
  boolean, Strings, char, int, long, etc.
- public StringBuffer reverse() This method reverses the value of the StringBuffer object that invoked the method.
- public delete(int start, int end) Deletes the String starting from the start index until the end index.
- public insert(int offset, int i) This method inserts a String s at the position mentioned by offset.
- replace(int start, int end, String str) This method replaces the characters in the substring of this StringBuffer with
  characters in this specified String.
  
Here is the list of other methods (Except set methods) which are very similar to the String class:

- int capacity() Returns the current capacity of the String buffer.
- char charAt(int index) The specified character of the sequence currently represented by the String buffer, as indicated
  by the index argument, is returned.
- void ensureCapacity(int minimumCapacity) Ensures that the capacity of the buffer is at least equal to the specified 
  minimum.
- void getChars(int srcBegin, int srcEnd, char[] dst, int dstBegin) Characters are copied from this StringBuffer into the
  destination character array dst
- int indexOf(String str) Returns the index within this String of the first occurence of the specified String.
