The singleton's purpose is to promote object creation, limiting the number of objects to one only. Since there is only
one singleton instance, any instance fields of a singleton will occur only once per class, just like static fields. Singletons
often control access to resources such as database connections or sockets.

For example, if you have a license for only one connection for your database or your JDBC driver has trouble with multithreading,
the Singleton makes sure that only one connection is made or that only one thread can access the connection at the time.

<h1>Implementing Singletons</h1>
<h2>Example 1</h2>
The easiest implementation consists of a private constructor and a field to hold its result, and a static accessor method
with a name like getInstance().

The private field can be assigned from within a static initializer block or more simply, using an initializer.
The getInstance() method (which must be public) then simply returns this instance.

                         public class Singleton {
                          private static Singleton singleton = new Singleton();
                          
                          /*
                          A private constructor prevents any other class from instantiating
                          */
                          private Singleton(){}
                          
                          /* Static instance method */
                          public static Singleton getInstance(){
                          }
                          
                          /*Other methods protected by singleton-ness*/
                          protected static void demoMethod(){
                          System.out.println("demoMethod for singleton");
                           }
                          }
                          
  Here is the main program file where we will create the singleton object:
  
                        public class SingletonDemo{
                         public static void main(String args[]){
                         Singleton tmp = Singleton.getInstance();
                         tmp.demoMethod();
                          }
                         }
                         
<h2>Example 2</h2>   
Following implementation shows a classic singleton design pattern:

                           public class ClassicSingleton {
                            private static ClassicSingleton(){
                            //exists only to defeat instantiation
                            }
                            public static ClassicSingleton getInstance(){
                            if(instance==null){
                            instance=new Classic Singleton();
                            }
                            return instance;
                             }
                            }
                            
The ClassicSingleton class maintains a static reference to the lone singleton instance and returns that reference from
the static getInstance().

Here, ClassicSingleton class employs a technique known as lazy instantiation to create the singleton; as a result, 
the Singleton instance is not created until the getInstance() method is called the first time. This instance ensures
that singleton instances are created only when needed.
