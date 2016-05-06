Object - Objects have states and behaviors. Example: a dog has states - color, name, breed, as well as behaviors -
wagging, barking, eating. An object is an instance of a class.

Class - A class can be defined as template/blue print that describes the behaviors/states that objects of its type
support.

<h2>Objects in Java</h2>
Let us now look in deep to what are objects. If we consider the real world, we can find many objects around us, Cars,
Dogs, Humans, etc. All these objects have a state and behavior.

If we consider a dog, then its state is - name, breed, color, and the behavior is barking, wagging, running.

If you compare a software object with a real world object, they have very similar characteristics.

Software objects also have a state and behavior. A software object's state is stored in fields and behavior is shown
via methods.

So, in software development, methods operate on the internal state of an object and the object-to-object communication
is done via methods.

<h2>Classes in Java</h2>
A class is a blueprint from which individual objects are created.

                              public class Dog {
                               String breed;
                               int ageC;
                               String color;
                               void barking(){
                               }
                               void hungry(){
                               }
                               void sleeping(){
                                 }
                              }
                               
  A class can contain any of the following variable types:
  
  - Local Variables: Variables defined inside methods, constructors, or blocks are caled local variables.
    The variable will be declared and initialized within the method and the variable will be destroyed when
    the method has completed.
  - Instance variables: Instance variables are variables within a class but outside any method. These variables
    are initialized when the class is instantiated. Instance variables can be accessed from inside any method,
    constructor, or blocks of that particular class.
  - Class variables: Class variables are variables within a class, outside any method, with the static keyword.
  
A class can have any number of methods to access the value of various kinds of methods. In the above example, barking(),
hungry(), and sleeping() are methods.

Below mentioned are some of the important topics that need to be discussed when looking into classes of the Java language.

<h2>Constructors</h2>
When discussing about classes, one of the most important subclasses would be constructors. Every class has a constructor.
If we do not explicitly write a constructor for a class the Java compiler builds a default constructor for that class.

Each time a new object is created, at least one constructor will be invoked. The main rule of constructors is that they
should have the same name as the class. A class can have more than one constructor.

                                 public class Puppy(){
                                  public Puppy() {}
                                  public Puppy(String name){}
                                  }
                                  
  Java also supports Singleton classes where you would only be able to create only one instance of a class.
  
  Note: We have two different types of constructors, we are going to discuss constructors in detail inn the upcoming
  chapters.
  
  <h2>Creating an Object</h2>
  As mentioned previously, a class provides the blueprints for objects. So, basically an object is created from a class.
  In Java, the new keyword is used to create new objects.
  
  There are three steps when creating an object from a class:
  
  - Declaration: A variable declaration with a variable name with an object type.
  - Instantiation: The "new" keyword is used to create the object.
  - Initialization: The "new" keyword is followed by a call to a constructor. The call initializes a new object.
  
Example of creating an object is below:

                              public class Puppy{
                               public Puppy(String name){
                               //the constructor has one parameter, name
                               System.out.println("Passed Name is:" + name);
                               }
                               public static void main(String args[]){
                               //Following statement would create an object, my puppy
                               Puppy myPuppy = new Puppy("tommy");
                                  }
                               }
                               
<h2>Accessing Instance Variables and Methods</h2>
Instance variables and methods are accessed via created objects. To access an instance variable, the fully qualified path
should be as follows:

                          /*First create the object*/
                          ObjectReference = new Constructor();
                          /*Now call a variable as follows*/
                          ObjectReference.variableName;
                          /*Now you can call a class method as follows*/
                          ObjectReference.methodName();
                          
  <h2>Example:</h2>
The example explains how to access instance variables and methods of a class:

                           public class Puppy{
                           int puppyAge;
                           
                           public PuppyAge(String name){
                           //The constructor has one parameter, name
                           System.out.println("Name chosen is" + name);
                           }
                           
                           public void setAge(int age){
                           puppyAge = age;
                           }
                           
                           public int getAge(){
                           System.out.println("Puppy's age is" + puppyAge);
                           return puppyAge;
                           }
                           
                           public static void main(String args[]){
                           //Object creation
                           Puppy myPuppy = new Puppy("tommy");
                           //Call class method to set puppy's age
                           myPuppy.setAge(2);
                           //Call class method to get puppy's age
                           myPuppy.getAge();
                           //You can access instance variables as follows as well
                           System.out.println("Variable value" + myPuppy.puppyAge);
                                }
                              }
                              
  <h2>Source File Declaration Rules</h2>
  As the last part of this section, let's now look into the source file declaration rules. These rules are essential
  when declaring classes, import statements and package statements in a source file.
  
  - There can only be one public class per source file.
  - A source file can have multiple non public classes.
  - The public class name should be the name of the source file as well which should be appended by .java
    at the end. For example: the class name is public class Employee{} then the source file should be Employee.java.
  - If the class is defined inside a package, then the package statement should be the first statement in the source file.
  - If import statements are present then they must be written between the package statement and the class declaration.
    If there are no package statements then the import statement should be the first line in the source file.
  - Import and package statements will imply to all the classes present in the source file. It is not possible to
    declare different import and/or package statements to different classes in the source file.

Classes have different access levels and there are different types of classes; abstract classes, final classes, etc. we will
be explaining about all these in the access modidier chapter.

Apart from the above mentioned types of classes, Java also has special classes called inner classes and annonymous classes.

<h2>Java Package</h2>
In simple, it was a way of categorizing the classes and interfaces. When developing applications in Java,
hundreds of classes and interfaces will be written, therefore categorizing these classes will make life much easier.

<h2>Import Statements</h2>
In Java if a fully qualified name, which includes the package and the class name, is given then the compiler can easily
locate the source code or classes. Import statement is the way of giving the proper location for the compiler to find
that particular class.

For example, the following line would ask the compiler to load all the classes available in the directory java_installation/
java/io:

                         import java.io.*;
                         
<h2>A Simple Case Study</h2>
For our case study, we will be creating two classes. They are Employee and EmployeeTest.

First open NotePad and add the following code. Rememeber this is the Employee class and the class is a public class.
Now, save this source file with the name Employee.java.

The Employee class has four instance variables name, age, designation, and salary. The class has one explicitly defined
constructor which accepts a parameter.

                           import java.io.*;
                           public class Employee { 
                           String name;
                           String age;
                           String designation;
                           double salary;
                           
                           //This is the constructor of the class Employee
                           public Employee(String name){
                           this.name = name;
                           }
                           
                           //Assign the age of the employee to the variable age
                           public void empAge(){
                           age=empAge;
                           }
                           
                           //Assign the designation to the variable designation
                           public void empDesignation(String empDesig){
                           designtion=empDesig;
                           }
                           
                           //Assign the salary to the variable salary.
                           public void empSalary(double empSalary){
                           salary=empSalary;
                           }
                           
                           //Print the employee details
                           public void printEmployee(){
                           System.out.println("Name" + name);
                           System.out.println("Age" + age);
                           System.out.println("Designation" + designation);
                           System.out.println("Salary" + salary);
                                   }
                           }
                           
  As mentioned previously in this tutorial, processing starts from the main method. Therefore, in order for us to 
  run this Employee class there should be a main method and objects should be created. We will be creating a separate 
  class for these tasks.
  
  Given below is the EmployeeTest class, which creates two instances of the class Employee and invokes the method for 
  each object to assign values for each variable.
  
                            import java.io.*;
                            public class EmployeeTest{
                             public static void main(String args[]) {
                             //Create two objects using constructor
                             Employee empOne = new Employee("James Smith");
                             Employee empTwo = new Employee("Mary Anne");
                             
                             //Invoking methods for each object created
                             empOne.empAge(26);
                             empOne.empDesignation("Senior Software Engineer");
                             empOne.empSalary(1000);
                             empOne.printEmployee();
                             
                             empTwo.empAge(21);
                             empTwo.empDesignation("Software Engineer");
                             empTwo.empSalary(500);
                             empTwo.printEmployee();
                                 }
                              }
                              
  
                           

                               
