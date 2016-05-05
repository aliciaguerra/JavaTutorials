Java provides a number of access modifiers to set access levels for classes, variables, methods, and constructors.
The four access levels are:
    - visible to the package. the default.no modifiers are needed.
    - visible to the class only (private).
    - visible to the world (public).
    - visible to the package and all subclasses (protected).
    
<h2>Default Access Modifiers - No Keyword</h2>
Default access modifier means we do not explicitly declare an access modifier for a class, field, method, etc.

A variable or method declared without any access control modifier is available to any other class in the same package.
The fields in an interface are implicitly public static final and the methods in the interface are by default public.

<h2>Example:</h2>
Variables and methods can be declared without any modifiers, as in the following examples:

                      String version="1.5.1";
                      boolean processOrder(){
                      return true;
                      }
                      
  <h2>Private Access Modifier - private:</h2>
  Methods, varibles, and constructors that are declared private can only be accessed within the declared class itself.
  Private accesss modifier is the most restrictive class level. Classes and interfaces cannot be private.
  
  Variables that are declared private can be accessed outside the class if public getter methods are present in the class.
  
  Using the private modifier is the main way that an object encapsulates itself and hide data from the outside world.
  
  <h2>Example</h2>
  The following class uses private access control:
  
                           public class Logger{
                           private String format;
                           public String getFormat(){
                            return this.format;
                            }
                           public void setFormat(String format){
                           this.format=format;
                           }
  
  Here, the format variable of the Logger class is private
                           }
