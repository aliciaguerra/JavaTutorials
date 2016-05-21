A variable provides us with named storage that our programs can manipulate. Each variable in Java has a specific type,
which determines the size and layout of the variable's memory, the range of values that can be stored within that memory,
and the set of operations which can be applied on that variable.

You must declare all variables before they can be used. The basic form of a variable declaration can be shown here:

                  data type variable [= value][, variable][, variable [= value]...];
                  
Here data type is one of Java's datatypes and variable is the name of the variable. To declare more than one variable
of the specified type, you can use a comma-separated list.

Following are valid examples of variable declaration and initialization in Java:

                   int a, b, c; //Declares three ints, a, b, and c
                   int a=10, b=10; //Example of initialization
                   byte B=22; //initializes a byte type variable B
                   double pi = 3.14159; //declares and assigns a value of PI
                   char a = 'a'; //the char variable a is initialized with the value 'a'
                   
This chapter will explain various variable types available in Java language. There are three kinds of variables in
Java:

- Local variables
- Instance variables
- Class/static variables

<h2>Local Variables</h2>
- Local variables are declared in methods, constructors, and blocks.
- Local variables are created when the method, constructor, or block is entered and the variable will be destroyed
  once it exits the method, constructor, or block
- Access modifiers cannot be used for local variables
- Local variables are visible only within the declared method, constructor, or block
- Local variables are implemented at stack level internally
- There is no default value for the local variables so local variables should be declared and an initial value should be assigned before first use.

<h2>Example:</h2>
Here, age is a local variable. This is defined inside pupAge() method and its cope is limited to this method only.

                        public class Test {
                         public void pupAge() {
                         int age = 0;
                         age = age+7;
                         System.out.println("Puppy age is:" + age);
                         }
                         
                         public static void main(String args[]) {
                         
                   
                   
