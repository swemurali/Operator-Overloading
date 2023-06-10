# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:
 
 ## step 1:
 Create a class for operator overloading.

 ## step2:
 Get inputs for length,breadth from the user in overloading function

 ## step 3:
 Compare the inputs such as length and breadth.

 ## step 4:
 Using equal to(==) and not equal to(!=) operator we can compare the inputs
 
 
 ## Program:
 ```
 using System;

namespace ConsoleApp8
{
   class example
   {
       public int length;
       public example()
       {
           length = 10;
       }
       public example(int i)
       {
           length = i;
       }
       public static bool operator == (example obj1, example obj2)
       {

           return obj1.Equals(obj2);
       }
       public static bool operator != (example obj1, example obj2)
       {
          return !obj1.Equals(obj2);
       }
       public static void Main()
       {
           example e1 = new example();
           example e2 = new example(20);
           example e3 = new example();
           example e4 = e3;
           if (e1 == e2)
           {
               Console.WriteLine("Equal");
           }
           else if (e1 != e2)
           {
               Console.WriteLine("Not equal");
           }
       }
   }
}
 ```
 
 ## Output:
 
 ![198813608-8dca83b3-d28e-4adf-a571-d5cd92895cd6](https://github.com/swemurali/Operator-Overloading/assets/94165336/b2dfd860-775a-48dd-b6d9-900759661518)

 
 ## Result:
Experiment has been successfully executed
