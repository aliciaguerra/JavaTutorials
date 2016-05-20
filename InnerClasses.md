<h2>Inner Classes</h2>
In Java, just like methods, variables of a class can have another class as its member. Writing a class within another
is allowed in Java. The class written within is called the nested class, and the class that holds the inner class is the outer
class. 

<h2>Syntax</h2>
The syntax to write  anested class is given below. Here Outer_Demo is the outer class and Inner_Demo is the nested inner
class.

                 class OuterDemo(){
                    class Inner_Demo(){
                              }
                 }
                 
Nested classes are divided into two types:

- Non-static nested classes: These are the non-static methods of the class.
- Static nested classes: These are the static methods of the class.

<h2>Inner Classes (Non-Static Nested Classes)</h2>
Inner classes are a security mechanism in Java. We know a class cannot be associated with the class modifier private,
but if we have the class as a memmber of the other class, then the inner class can be made private. And this is also
used to access the private modifiers of a class.

Inner classes are three types depending on how and where you define them. They are:

- inner class
- method-local inner classes
- annonymous inner class

<h2>Inner Class</h2>
Creating an inner class is quite simple. You just need to write a class within a class. Unlike a class, an inner
class can be private and once you declare an inner class private, it cannot be accessed from an object outside the 
class.

Given below is the program to create an inner class and access it. In the given example, we make the inner class
private and access the class through a method.

                        class Outer_Demo {
                         int num;
                         //inner class
                         private class Inner_Demo {
                         public void print() {
                         System.out.println("This is an inner class");
                            }
                         }
                         //Accessing the inner class from the method within
                         void display Inner() {
                         Inner_Demo inner = = new Inner_Demo();
                         inner.print();
                             }
                         }
                         public class My_class {
                          public static void main(String args[]) {
                          //Instantiating the outer class
                          Outer_Demo outer = new Outer_Demo();
                          //Accessing the display_Inner() method
                          outer.display_Inner();
                            }
                          }
                          
 Here you can observe that Outer_Demo is the outer class, Inner_Demo is the inner class, display_Inner() is the method
 in which we are instantiating the inner class, and this method is invoked from the main method.
 
 <h2>Accessing the Private Members</h2>
 As mentioned earlier, inner classes are also used to access the private memebers of the class. Suppose a class is having
 private members to access them. Write an inner class in it, return the private members from a method within the inner
 class, say, getValue(), and finally another class (from which you want to access the private members) call the
 getValue() method of the inner class.
 
 To instantiate the inner class, initially you have to instantiate the outer class.Thereafter, using the object of the
 outer class, you can instantiate the inner class as shown.
 
                     Outer_Demo outer = new Outer_Demo();
                     Outer_Demo.Inner_Demo inner = outer.new Inner_Demo();
                     
The following program shows how to access the private members of a class using inner class

                     class Outer_Demo {
                      //private variable of the outer class
                      private int num=175;
                      //inner class
                      public class Inner_Demo {
                      public int getNum();
                      System.out.println("This is the getnum method of the inner class");
                      return num;
                          }
                        }
                      }
                      
                      public class My_class2 {
                      public static void main(String args[]) {
                      //Instantiating the outer class
                      Outer_Demo outer = new Outer_Demo();
                      //Instantiating the inner class
                      Outer_Demo.Inner_Demo inner = outer.new Inner_Demo();
                      System.out.println(inner.getNum());
                           }
                      }
                      
<h2>Method-Local Inner Class</h2>
In Java, we can write a class within the method and this will be a local type. Like local variables, the scope of the
inner class is restricted within the method.

A method-local inner class can be instantiated only within the method where the inner class is defined.

                     public class Outerclass {
                      //instance method of the outer class
                      void my_Method() {
                      int num = 23;
                      
                      //method-local inner class
                      class MethodInner_Demo {
                      public void print() {
                      System.out.println("This is the method inner class" + num);
                        }
                      }//end of inner class
                      
                      //Accessing the inner class
                      MethodInner_Demo inner = new MethodInner_Demo();
                      inner.print();
                      }
                      
                      public static void main(String args[]) {
                      OuterClass outer = new OuterClass();
                      outer.my_Method();
                            }
                      }
                      
<h2>Anonymous Inner Class</h2>    
An inner class declared without a class name is known as an anonymous inner class. In case of anonymous inner classes,
we declare and instantiate them at the same time. Generally, they are used whenever you need to override the method
of a class or an interface. The syntax of an anonymous inner class is as follows:

                    AnonymousInner an_inner = new AnonymousInner(){
                    public void my_method(){
                     }
                    }
                    
The following program shows how to override the method of a class using anonymous inner class.     

                  abstract class AnonymousInner {
                  public abstract void my_method();
                  }
                  
                  public class Outer_class {
                  public static void main(String args[]) {
                  AnonymousInner inner = new AnonymousInner();
                  public void mymethod(){
                  System.out.println("This is an example of anonymous inner class");
                   }
                  };
                  inner.my_method();
                   }
                  }
                  
In the same way, you can override the methods of the concrete class as well as the interface using an anonymous inner class.

<h2>Anoymous Inner Class as Argument</h2>
Generally if a method accepts an object of an interface, an abstract class, or a concrete class, than we can implement
the interface, extend the abstract class, and pass the object to the method. If it is a class, then we can directly pass
it to the method.

But in all three cases, you can pass an anonymous inner class to the method. Here is the syntax of passing an anonymous 
inner class as a method argument.

                   obj.my_method(new My_Class() {
                   public void Do{
                   }
                   });
                   
The following program shows how to pass an anonymous inner class as a method argument:

                  //interface
                  interface Message(){
                  String greet();
                  }
                  
                  public class My_class {
                  //method which accepts the object of interface Message
                  public void displayMessage(Message m){
                  System.out.println();
                  }
