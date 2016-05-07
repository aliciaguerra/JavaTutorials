Normally, when we work with characters, we use primitive data types char. 

                             char c='a';
                             //Unicode for uppercase Greek omega character
                             char uniChar='\u039A';
                             //an array of characters
                             char[] charArray = {'a', 'b', 'c', 'd', 'e'};
                             
However, in development, we come across situations where we need to use objects instead of primitive data types.
In order to achieve this, Java provides a wrapper class Character for the primtiive data type char. 

The Character class offers a number of useful class (i.e. static) methods for maniuplating characters. You create a
Character object with the Character constructor:

                              Character ch = new Character('a');
                              
The Java compiler will also create a Character object for you under some circumstances. For example, if you pass a primitive
char into a method that expects an object, the compiler automatically converts the char into a Character for you. This feature is called autoboxing or unboxing, if the conversion goes the other way.

                             //Here following primitive char 'a'
                             //is boxed into the Character object ch
                             Character ch = 'a';
                             //Here primitive 'x' is boxed for method test,
                             //return is unboxed to char c
