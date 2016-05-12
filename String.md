String, which are widely used in Java programming, are a String of Characters. In the Java programming language,
Strings are objects.

The Java platform provides the String class to create and manipulate strings.

<h2>Creating Strings</h2>
The most direct way to create a String is to write:

                  String greeting "Hello World!";
                  
Whenever it encounters a String literal in your code, the compiler creates a String object with a value in this case 
"Hello World!".

As with any other object, you can create String objects by using the new keyword and a constructor. The String class has
eleven constructors that allow you to provide the initial value of the String using different sources, such as an array of
characters.

                   public class StringDemo {
                     public static void main(String args[]) {
                      char[] helloArray = { 'h', 'e', 'l', 'l', 'o', '.'};
                      String helloString = new String(helloString);
                      System.out.println(helloString);
                      }
                  }
                  
Note: The String class is immutable, so that once it is created, a String object cannot be changed. If there is a 
necessity to make a lot of modifications to Strings of characters, then you should use the StringBuffer and
StringBuilder classes.

<h2>String Length</h2>
Methods used to obtain information about an object are known as accessor methods. One accessor method that you can
use with Strings is the length() method, which returns the number of characters contained in the String object.

Below given program is an example of length(), method String class. 

                    public class StringDemo {
                     public static void main(String args[]) {
                      String palindrome = "Dot saw I was Tod";
                      int len = palindrome.length();
                      System.out.println("String Length is:" +len);
                        }
                    }
                    
<h2>Concatenating Strings</h2>
The string class includes a method for concatenating two strings:

                      string1.concat(string2);
                      
This returns a new String that is string1 with string2 added to it at the end. You can use the concat() method with
String literals, as in:

                      "My name is ".concat("Zara");
                      
Strings are more commonly concatenated with the + operator, as in:

                      "Hello, " + "world" + "!"
                      
Let us look at the following example:

                       public class StringDemo {
                         public static void main(String args[]) {
                          String string1 = "saw I was";
                          System.out.println("Dot" + String1 + "Tod");
                            }
                       }
                       
<h2>Creating Format Strings</h2>
You have printf() and format() methods to print output with formatted numbers. The String class has an equivalent class method, format(), that returns a String object rather than a PrintStream object.

Using String's static format() method allows you to create a formatted string that you can reuse, as opposed to a one-time print statement. For example, instead of:

                   System.out.printf("The value of the float variable is" + "%f, while the value of the integer")
                   + "variable is %d, and the string" + "is %s", floatVar, intVar, stringVar);
                   
you can write:

                   String fs;
                   fs = String.format("The float variable is" + 
                   "%f, while the value of the integer" +
                   "variable is %d, and the String" +
                   "is %s", floatVar, intVar, stringVar);
                   System.out.println(fs);
                   
<h2>String Methods</h2>
- char charAt(index i) Returns the character at the specified index
- int compareTo(Object o) Compares this String to another object
- int compareTo(String anotherString) Compares two string lexicographically
- int compareToIgnoreCase(String str) Compares two strings lexicographically, ignoring case differences
- String concat(String str) Concatenates the specified string to the end of this String
- boolean ContentEquals(StringBuffer sb) Returns true if and only if String represents the same sequence of characters
  as the specified StringBuffer.
- static String copyValueOf(char[] data) Returns a String represents the character sequence in the array specified.
- static String copyValueOf(char[] data, int offset, int count) Returns a String that represents the character sequence in
  the array specified.
- boolean endsWith(String suffix) Test if this string ends with the specified suffix.
- boolean equals(Object anObject) Compares this String to the specified object.
- boolean equalsIgnoreCase(String anotherString) Compares this string to another string, ignoring case considerations
- byte getBytes() Encodes this String into a sequence of bytes using the platform's default charset, storing the result
  into a new byte array.
- byte[] getBytes(String charsetName) Encodes this String into a sequence of bytes using the named charset, storing the 
  result in a new byte array
- void getChars(int srcBegin, int srcEnd, char[] dst, int dstBegin) Copies characters from the String into the destination
  character array.
- int hashCode() Returns a hashCode for this String
- int indexOf(int ch) Returns the index within the String of the first outcome of the specified character
- int indexOf(int ch, int fromIndex) Returns the index within the String of the first occurence of the specified character,
  starting the search at the specified index
- int indexOf(String str) Returns the index within this String of the first occurence of the specified substring
- int indexOf(String str, int fromIndex) Returns the index within this String of the first occurrence of the specified
  substring, starting at the specified index
- String intern() Returns a canonical representation of the string object
- int lastIndexOf(int ch) Returns the index within this String of the last occurrence of the specified character.
- int lastIndexOf(int ch, int fromIndex) Returns the index within this String of the last occurrence of the specified
  character, searching backwards starting at the specified index
- int lastIndexOf(String str) Returns the index of the String of the rightmost occurrence of the specified substring.
- int lastIndexOf(String str, int fromIndex) Returns the index within this string of the last occurrence of the specified
  substring, searching backwards starting at the specified index.
- int length() Returns the length of the specified string
- boolean matches(String regex) Tells whether or not this string matches the given regular expression
- boolean regionMatches(boolean ignoreCase, int toffset, String other, int ooffset, int len) Tests if two String regions are
  equal
- boolean regionMatches(int toffset, String other, int ooffset, int len) Tests if two String regions are equal
- String replace(char oldChar, char newChar) Returns a new String resulting from replacing all occurrences of oldChar in
  this String with newChar.
- String replaceAll(String regex, String replacement) Replaces each substring of this String that matches the given regular
  expression with the given replacement.
- String replaceFirst(String regex, String replacement) Replaces the first substring of this string that matches the given
  regular expression with the given replacement.
- String[] split(String regex) Splits the string around matches of the given regular expression
- String[] split(String regex, int limit) Splits the string around matches of the given regular expression
- boolean startsWith(String prefix) Test if this String starts with the specified prefix
- boolean startsWith(String prefix, int toffset) Tests if this string starts with the specified prefix beginning a specified   index
- CharSequence subSequence(int beginIndex, int endIndex) Returns a new character sequence that is a subsequence of this 
  sequence.
- String substring(int beginIndex) returns a new string that is a substring of this string
- String substring(int beginIndex, int endIndex) Returns a new String that is a substring of this string
- char[] tocharArray() Converts this String to a new charArray
- String toLowerCase() Converts all of the characters in this String to lower case using the rules of the default locale
- String toLowerCase(Locale locale) Converts all characters in this String to lower case using the rules of the given locale
- String toString() The object (which is already a string) is itself returned
- String toUpperCase() Converts all of the characters in this String to upper case using all the rules of the default 
  locale.
- String toUpperCase(Locale locale) Converts all the characters in this String to upper case using the rules of the given
  locale.
- String trim() Returns a copy of the string, with leading and trailing whitespace ommitted.
- static String valueOf(primitive data type x) Returns the String representation of the passed data type argument.
                   

