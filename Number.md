Normally, when we work with numbers we use primitive data types such as byte, long, int, double, etc.

Example:

                              int i = 5000;
                              float gpa = 13.65;
                              byte mask = 0xaf;
                              
However, in development, we come across situations where we need to use objects instead of primitive data types. 
In order to achieve this, Java provides wrapper classes.

All the wrapper classes (Integer, Long, Byte, Double, Float, Short) are subclasse of the abstract Number.

The object of the wrapper class contains or wraps its repsective primitive data type. Converting primitive data types
into objects is called boxing, and this is taken care of by the compiler. Therefore, while using the wrapper class,
you just need to pass the value of the primitive data type to the constructor of the Wrapper class.

And the wrapper object will be converted back to a primitive data type, and this process is called unboxing.The
Number class is part of the java.lang package.

Here is an example of boxing and unboxing:

                             public class Test {
                              public static void main(String args[]){
                              Integer x=5; //boxes int to an Integer object
                              x=x+10; //unboxes the integer to an int
                              System.out.println(x);
                               }
                              }
                              
                              //RESULT:
                              //15
                              
When x is assigned integer value, the compiler boxes the integer because x is the integer object. Later, x is unboxed
so that they can be added as integer.

<h2>Number Methods</h2>

- xxxValue() Converts the value of this number object to the xxx data type and returned it
- compareTo() compare this Number object to the argument
- equals() Determines whether this number object is equal to the argument
- valueOf() returns an Integer object holding the value of the specified primitive
- toString() returns a String object representing the value of the specified int or Integer
- parseInt() this method is used to get the primtiive data type of a certain String
- abs() returns the absolute value of the argument
- ceil() returns the smallest integer that is greater than or equal to the argument. Returned as double.
- floor() Returns the largest integer that is less than or equal to the argument. 
- rint() Returns the integer that is closest in value to the argument. Returned as double.
- round() Returns the closest long or int, as indicated by the method's return type, to the argument.
- min() returns the smallest of the two arguments
- max() returns the largest of two arguments
- exp() returns the base of the natural logarithms, e, to the power of argument
- log() returns the natural logarithm of the argument
- pow() returns the value of the first argument raised to the power of the second argument
- sqrt() returns the square root of the argument
- sin() returns the sine of the specified double value
- cos() returns the cosine of the specified double value
- tan() returns the tangent of the specified double value
- asin() returns the arcsine of the specified double value
- acos() returns the arcosine of the specified double value
- atan() returns the arctangent of the specified double value
- atan2() converts rectangular coordinates (x,y) to polar coordinate (r, theta) and returns theta
- toDegrees() converts the arguments to degrees
- toRadians() converts the argument to radians
- random() returns a random number

