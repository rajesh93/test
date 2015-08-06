# test
1. Reflection:
It’s a process of modifying the run time behavior of a class.
2. What is the super class all the exception and error classes?
Throwable is the super class for all types of exception.
3. Name few subclasses of Exception and Error?
Runtime Exception, Arithmetic exception, array index out of bound exception, filenotfound exception.

4. example having try, multiple catch, finally block:
public class hello {
	int c;
	String a;
	public void hello1()
	{
		try
		{
		
		a=null;
		System.out.println(a.length());
		c=1/0;
	}
		catch(ArithmeticException e)
		{
			System.out.println("Arith exception");
		}
		catch(NullPointerException e)
		{
			System.out.println("Null pointer");
		}
		finally
		{
			System.out.println("code to be executed irrespective of exception occurs or not");
		}
	}
public static void main(String args[])
{
hello obj=new hello();
	obj.hello1();
}
}
5. Can a try can be associated without catch block
	Yes, it is possible to use try block without catch block by combining try with finally block
6.Final:
        Final is a keyword and used to provide restriction on class,variable and method to be inherited.
Finally:
       Finally is a block and it is executed whether exception occurs or not.
Finalize:
       It is a method and it is used to clean memory just before the object is getting into garbage collector.
7. Checked Exception:
It is checked in compile time. Ex: IO and SQL Exeception
		
Unchecked Exception:
            It is checked in run time Ex: array bound out of index and null pointer exception.

8. What are all ways you can handle the checked exceptions?
	Checked exception handled by try-catch-throw and throws keyword.
9. What happens if exception occurs and if you don’t have catch block for that exception?
	Suppose if exception occurs at line 7 means, code will not be executed after line7.It will show error message.
10. Throws:
	Doesn’t handle exception it will show some message to the user like exceptions occurs and it’s used in method signature.
Throw:
	It is used in custom exceptions i.e the user defines some exception.it is used within the method.

11.User defined Exception:
If user defines their own exception then it is called as user defined exception
12.What is the difference between throwing an exception by JVM and when you use throw keyword?
	Throw is used to define user defined exception and JVM shows compile time and runtime exception.
13. How can you change the exception's message which will print while printing the stack trace?
	
14.Finally working scenarios:
	*Try,catch,finally
	*Try,finally
	*Method,finally
Finally not working scenarios:
	In case of fatal error and any method contain System.exit() 
15. What are all the types of I/O supported by java and list down all the interfaces and implementation classes under each category of I/O?
I/O:
        Supported I/O:
              *Character based I/O
              *Byte based I/O
       Interfaces:
                *Reader
                *Writer
                *InputStream
                *OutputStream

       Implementation classes:
                *FileReader
                *BufferReader 
                *FileWriter
                *BufferdWriter
                *FileInputStream
                *BufferedInputStream
               *ObjectInputStream
               *FileOutputStream
               *BufferedOutputStream
               *ObjectOutputStream
               
16. What is meant by marker interface? Give me few examples of marker interfaces?
	Marker interface is used as a tag to inform a message to the java compiler so that it can add special behavior to the class implementing it.
Ex:Serializiable,Clonnable.
17. What is meant by serialization? what are all the interfaces that you can use to achieve serialization?
            It is a mechanism which contains both object’s data as well as information. Serializable is an interface.                                                                                                
18. How can you make some state variables to not include in serialization?
	By using transient we can make some state variables not  to be included in serialization process.
19. What is meant by OutofMemory Error and How will you be able to fix it?
	OutofMemory error means allocated memory in the heap will be full. Using vm arguments we can increase the memory area.

20. What is difference between Serializable and Externalizable interface?
	Serializable                                                                  Externalizable
        It is marker interface.                                                  It is not marker interface.
        Marker interface does not have                                   It have methods.                                                        
        any methods.        

