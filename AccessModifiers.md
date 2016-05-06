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
  
  Here, the format variable of the Logger class is private, so there's no way for other classes to retrieve or set its value
  directly.
  
  So to make this variable available to the outside world, we defined two public methods: getFormat(), which returns 
  the value of the format, and setFormat(String), which sets its value.
  
  <h2>Public Access Modifier - Public</h2>
  A class, method, constructor, interface declared public can be accessed from any other class. Therefore, fields, 
  methods, blocks declared inside a public class can be accessed from any other class. Therefore, fields, methods, blocks,
  declared inside a public class can be accessed from any class belonging to a Java universe.
  
  However, if the public class we are trying to access is in a different package, then the public class still needs
  to be imported.
  
  Because of class inheritance, all public methods and variables of a class are inherited by subclasses. 
  
  <h2>Example:</h2>
  The following function uses public access control:
  
                               public static void main(String args[]){
                               }

The main method of an application has to be public. Otherwise, it could not be called by a Java interpreter (such as Java)
to run the class.

<h2>Protected Access Modifier - Protected</h2>
Variables, methods, and constructors which are declared protected in a superclass in other package or any class within the package of protected members' class.

The protected access modifier cannot be applied to class and interfaces. Methods, fields can be declared protected,
however methods and fields in an interface cannot be declared protected.

Protected access gives the subclass a chance to use the helper method or variable, while preventing a nonrelated 
class from trying to use it.

<h2>Example</h2>
The following parent class uses protected access control to allow its child class override openSpeaker() method.

                                 class AudioPlayer {
                                  protected boolean openSpeaker(Speaker sp) {
                                  //implementation details
                                       }
                                     }
                                 class StreamingAudioPlayer {
                                    booleanOpenSpeaker(Speaker sp){
                                        }
                                }
                                
Here, if we define openMethod() speaker as private, then it would not be accessible from any other class other
than AudioPlayer. If we define it as public, then it would become accessible to the outside world. But our intention
is to expose this method to its subclass only, that's why we used the protected modifier.

<h2>Access Control and Inheritance</h2>
The following rules for inherited methods are enforced:
           
- Methods declared public in a superclass also must be public in all subclasses.
- Methods declared protected in a superclass must either be protected or public in subclasses; they cannot be private.
- Methods declared private should not be inherited at all, so there is no rule for them.
                                 
