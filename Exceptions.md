An exception (or exceptional event) is a problem that arises during the execution of a program. When an exception occurs, the
normal flow of the program is disrupted and the program/application terminates abnormally, which is not recommended, therefore
these exceptions are to be handled. An exception can be for many different reasons, below given are some scenarios where
exception occurs.
- A user enters invalid data
- A file that needs to be opened cannot be found
- A network connection has been lost in the middle of communications or the JVM ran out of memory

Some of the exceptions are caused by user error, others by programmer error, and others by physical resources that have 
failed in some manner. 

Based on these we have three categories of Exceptions you need to understand them to know how exception handling works in
Java. 

- Checked Exceptions
  A checked exception is also an exception that occurs at compile time, these are also called as compile time exceptions.
  These exceptions cannot simply be ignored at the time of compilation, the programmer should take care of (handle)
  these exceptions.
  For example, if you use FileReader class in your program to read data from a file, if the file specified in its
  constructor doesn't exist, then a FileNotFoundException occurs, and compiler prompts the programmer to handle the
  exception. 
  
                   import java.io.File;
                   import java.io.FileReader;
                   public class FilenotFound_Demo {
                    public static void main(String args[]) {
                     File file = new File("E://file.txt");
                     FileReader fr = new FileReader(file);
                       }
                   }
                   
Since the methods read() and close() of FileReader class throws IOException, you can observe that compiler notifies to
handle IOException along with FileNotFoundException.

- Unchecked Exceptions: An unchecked exception is an exception that occurs at the time of the execution, these are also 
  called Runtime Exception, these include programming bugs, such as logic errors or improper use of an APIs. Runtime
  exceptions are ignored at the time of compilation. 
  
  For example, if you have declared an array of size 5 in your program, and trying to call the 6th element of an array,
  then an ArrayOutOfBoundsException occurs.
  
                  public class Unchecked_Demo {
                    public static void main(String args[]) {
                     int num[] = {1,2,3,4};
                     System.out.println(num[5]);
                       }
                  }
                  
  Error: These are not exceptions at all, but problems that arise beyond the control of the user or programmer. 
  Errors are typically ignored in your code because you can rarely do anything about an error. For example, if a
  if a stack overflow occurs, an error will arise. They are also ignored at the time of compilation.
  
  #Exception Hierarchy
  All exception classes are subtypes of java.lang.Exception class. The exception class is a subclass of the Throwable class.
  Other than the exception class, there is another class called error which is devised from the throwable class.
  
  Errors are abnormal conditions that happen in case of severe failures, that are not handled by the Java programs.
  Errors are generated to indicate errors generated by the runtime environment. Example: JVM is out of memory.
  Normally programs
  
  
