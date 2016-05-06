The singleton's purpose is to promote object creation, limiting the number of objects to one only. Since there is only
one singleton instance, any instance fields of a singleton will occur only once per class, just like static fields. Singletons
often control access to resources such as database connections or sockets.

For example, if you have a license for only one connection for your database or your JDBC driver has trouble with multithreading,
the Singleton makes sure that only one connection is made or that only one thread can access the connection at the time.

<h1>Implementing Singletons</h1>
<h2>Example 1</h2>
The easiest implementation consists of a private constructor and a field to hold its result, and a static accessor method
with a name like getInstance();
