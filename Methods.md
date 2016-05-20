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
