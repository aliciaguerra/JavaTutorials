A Java method is a collection of statements that are grouped together to perform an operation. 
When you call the System.out.println method, for example, the system actually executes several statements in order to 
display a message on the console. Now you will learn how to create your own methods with or without return values, invoke
a method with or without parameters, and apply method abstraction in the program design.

<h2>Creating Method</h2>
Considering the following example to explain the syntax of the method

                           public static int methodName(int a, int b) {
                           //body
                           }
                           
Here,

- public static: modifier
- int: return type
- methodName: name of method
- a, b: formal parameters
- int a, int b: list of parameters

Method definition consists of a method header and a method body. The same is shown below:

                         modifier returnType nameOfMethod(Parameter list) {
                         //method body
                         }
                         
<h2>Example</h2>     
Here is the source code of the above defined method called max(). This method takes two parameters num1 and num2 and
returns the maximum between the two. 

                        /*the snippet returns the minimum between two numbers*/
                        public static int minFunction(int n1, int n2) {
                        int min;
                        if(n1>n2)
                        min=n2;
                        else
                        min=n1;
                        return min;
                        }
                        
<h2>Method Calling</h2>      
For using a method, it should be called. There are two ways in which a method is called i.e. method returns a value or returning nothing (no return value). 

The process of method calling is simple. When a program invokes a method, the program control gets transferred
to the called method. This called method then returns control to the caller in two conditions, when:

- return statement is executed
- reaches the method ending close brace

The methods returning void is considered to call to a statement. Let's consider an example.

                  System.out.println("This is a tutorialspoint.com");
                  
The method value can be overturned by the following example:

                    int result = sum(6,9);
                    
<h2>EXAMPLE</h2>           
Following is the example to demonstrate how to define a method and how to call it:

                    public class ExampleMinNumber {
                     public static void main(String args[]) {
                     int a = 11;
                     int b = 6;
                     int c = minFunction(a,b);
                     System.out.println("Minimum Value=" + c);
                     
                     /*Returns the minimum of two numbers*/
                     public static int minFunction(int n1, int n2) {
                     int min;
                     if(n1>n2)
                     min=n2;
                     else
                     min=n1;
                     return min;
                      }
                     }
                     
<h2>The void Keyword</h2>  
The void keyword allows us to create methods which do not return a value. Here, in the following example we're considering,
a void method methodRankPoints. This method is a void method which does not return any value. Call to a void method must be
a statement i.e. methodRankPoints(255.7). This method is a void method which does not return any value. 

EXAMPLE

                     public class Examplevoid {
                      public static void main(String args[]) {
                      methodRankPoints(255.7);
                      }
                      
                     public static void methodRankPoints(double points){
                     if(points>=202.5) {
                     System.out.println("Rank: A1");
                     }
                     else if(points>=122.4)
                     System.out.println("Rank: A2");
                     }
                     else {
                     System.out.println("Rank: A3");
                           }
                          }
                        }
                        
<h2>Passing Parameters by Value</h2> 
While working under calling process, arguments is to be passed. These should be in the same order as their respective 
parameters in the method specification. Parameters can be passed by value or by reference.

Passing parameters by value means calling a method with a parameter. Through this the argument value is passed to
the parameter.

<h2>EXAMPLE</h2>
The following program shows an example of passing parameters by value. The values of the arguments remain the same even
after method invocation.

                          public class swappingExample {
                           public static void main(String args[]) {
                           int a = 30;
                           int b = 45;
                           
                           System.out.println("Before swapping, a=" + a + "and b=" + b);
                           
                           //Invoke a swap method
                           swapFunction(a,b);
                           System.out.println("\n***Now, Before and After swapping values will be the same here**:");
                           System.out.println("After swapping, a=" + a + " and b is" + b);
                           }
                           
                           public static void swapFunction(int a, int b){
                           System.out.println("Before swapping(inside), a=" + a + "b=" + b);
                           
                           //swap n1 with n2
                           int c = a;
                           a=b;
                           b=c;
                           
                           System.out.println("After swapping(Inside), a=" + a + "b=" + b);
                                }
                           }
                           
<h2>Method Overloading</h2>  
When a class has two or more methods by the same name but different parameters, it is known as method overloading. 
It is different from overriding. In overriding a method has same method name, type, numbe rof parameters, etc.

Let's consider the example shown before for finding minimum numbers of integer type. If, let's say we want to find 
minimum number of double type. Then the concept of Overloading will be introduced to create two or more methods
with the same name but different parameters.

                         public class ExampleOverloading {
                          public static void main(String args[]) {
                          int a = 11;
                          int b = 6;
                          double c = 7.3;
                          double d = 9.4;
                          int result1 = minFunction(a,b);
                          //same function name with different parameters
                          double result2 = minFunction(c,d);
                          System.out.println("Minimum Value=" + result1);
                          System.out.println("Minimum Value=" + result2);
                          }
                          
                          //for integer
                          public static int minFunction(int n1, int n2) {
                          int min;
                          if(n1>n2)
                          min=n2;
                          else
                          min=n1;
                          return min;
                             }
                          }
                          
Overloading methods makes programs readable. Here, two methods are given same name but with different parameters. The
minimum number from integer and double types is the result.

<h2>Using command line arguments</h2>
Sometimes you will want to pass information into a program when you run it. This is accomplished by passing 
command arguments into main. 

A command-line argument is the information that directly follows the program's name on the command line when it is
executed. To access the command line arguments inside a Java program is quite easy. They are stored as string in the 
String array passed to main().

<h2>Example</h2>
The following displays all the command-line arguments that is called with:

                          public class CommandLine {
                           public static void main(String args[]) {
                           for(int i=0; i<args.length; i++) {
                           System.out.println("args[" + i + "]:" + args[i]);
                                  }
                               }
                           }
  
  This would produce the following result
  
                          $java CommandLine this is a command line 200 -100
                          
                          args[0]: this
                          args[1]: is
                          args[2]: a
                          args[3]: command
                          args[4]: line
                          args[5]: 200
                          args[6]: -100
                          
<h2>The Constructors</h2>   
A constructor initializes an object when it is created. It has the same name as its class and is syntatically similar
to a method. However, constructors have no explicit return type. 

Typically, you will use a constructor to give initial values to the instance variables defined by the class, or to perform
any other startup procedures required to create a fully formed object.

All classes have constructors, whether you define one or not, because Java automatically provides a default constructor
that initializes all member variables to zero. However, once you define your own constructor, the default constructor
is no longer used.

EXAMPLE

Here is a simple example that uses a constructor without parameters:

                     //A simple constructor
                     class MyClass{
                     int x;
                     //Following is the constructor
                     MyClass(){
                     x=10;
                     }
                     }
                     
You would call the constructor to initialize objects as follows:

                     public class ConsDemo {
                      public static void main(String args[]) {
                       MyClass t1 = new MyClass();
                       MyClass t2 = new MyClass();
                       System.out.println(t1.x + " " + t2.x);
                           }
                      }
                      
 <h2>parameterized constructor</h2>   
 Most often, you will need a constructor that accepts one or more parameters. Parameters are added to a constructor
 in the same way they are added to a method, just declare them inside the parentheses after the constructor's name.
 
 <h2>Example</h2>
 Here is a simple example that uses a constructor parameter:
 
                    //A simple constructor
                    class MyClass {
                    int x;
                    
                    //Following the constructor
                    MyClass(int i) {
                    x=i;
                     }
                    }

You would call a constructor to initialize objects as follows:

                   public class ConsDemo {
                    public static void main(String args[]) {
                    MyClass t1 = new MyClass(10);
                    MyClass t2 = new MyClass(20);
                    System.out.println(t1.x + " " + t2.x);
                         }
                    }
                    
<h2>the this keyword</h2>                    

                           
