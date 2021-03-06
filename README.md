# Coding With C

*This is a tutorial I made for my final project in my Computer Programming with GIS course (Fall 2020)*

This tutorial will show you a very brief introduction the programming language C and approaches to using it in GIS work. Throughout our class we have mostly used Python and Java, which have many similarities, however C operates slightly differently. You may have heard of C++, and C#, which are both derived from C, however they are different languages and work differently. In order to understand how C works, we first need to understand the difference between object oriented programming (OOP) and procedural oriented programming (POP). These are two different approaches to writing code and therefore exist in different programming languages. 

Here are some key facts about each one:

### Object Oriented Programming (OOP) ### 
* Easy to add new classes without changing functions that already exist
* Data is hidden behind functions that operate on them
* Structures a program by grouping behaviours into classes and objects in order to solve problems
* Each class often has its own function
* Some key features of OOP are:
  * Encapsulation: Reduces complexity. Able to reuse that part of it. 
  * Abstraction - data into concepts and modular units.
  * Inheritance - Eliminates redundant code.
  * Polymorphic - the code can change but the algorithm stays the same. 

### Procedural Oriented Programming (POP) ###
* Data is exposed and can be easily modified, not abstracted
* Uses classes and objects, however not in the same way that OOP does
* Easy to add new functions without changing the data structure
* Classes don’t always have their own functions

Many coding languages such as Python, Java, Ruby and C++ use OOP as they are very user friendly. With Python, the code is written, run in the interpreter and an output is given using an IDE so that machines can understand it. Python is a high-level language and is very person oriented, meaning that it’s easy for humans to intuitively understand and interpret. C is what’s called a low-level language and more machine oriented, so it’s easier for a machine to read but harder for a human to understand. It is put through a compiler and then an executor and the output does not have to go through an IDE. 


### Uses in GIS ###
C is not used in GIS the same way we use Python, as C is more commonly used to code hardware devices and heavyweight development. It is not often used for scripting, data processing, analysis & modeling, web mapping, as we do with Python. This means that C is used to code processing system and geospatial libraries such as the Geospatial Data Abstraction Library (GDAL), or the German database for spatial data Einheitliche Datenbankschnittstelle (EDBS). There are some open source GIS projects written in C (also uses C++ and Python) such as the  that reads raster and vector data, for example GRASS GIS (Geographic Resources Analysis Support System).


### Let's Code! ###
Now that we have some background knowledge on C, let's code in Python and also C! We will be using a lab that is taken from IDCE 302: Python Programming. We will be creating a code that shows temperature suitability mapping for chameleons. 
When coding in C, you are able to use Python, Google Colab, Jupyter Notebooks or anything that can read Python. In order to write in C, I used CLion, which is an IDE for writing code in C, however you may use something else such as Visual Studio or Eclipse.

We will write code that looks at temperature in different areas. This will be helpful when assessing the climate when a temperature is input to the code.  To begin, let's create our class and our object (used in OOP).

```
class Temperature: 
  def globalTemp(x):
```
Our class is temperature and our object is global Temp. Next we will set our parameters for the temperature.

```
#This function classifies which numerical temperature will go into which category.
class Temperature: 
  def globalTemp(x):
    if x >= 100:
      print("It is hot")
    elif x >= 70 and x < 100:
      print("It is warm")
    elif x >= 32 and x < 70:
      print("It is cool")
    elif x < 32:
      print("It is cold")

#I added "int" to the beginning so that the program knows it is an integer as opposed to a string. 
  feelTemp(x = int(input('Enter temperature: ')))
```

Now to let's create the same code using C:

```
#include<stdio.h>
int main()
{
  int x;
  printf("Enter x:");
  scanf("%d", x);
  if(x=<100)	
  {		
   printf(“It is hot");	
  }	
  if(x>=70 && x<100)
  {		
   printf(“It is warm");	
  }	
  if (x>=32 && x <70);
  {
   printf(“x “It is cool.);
  }
   if(x<32)	
  {		
   printf(“x “It is cold.);	
  }	
  getch();
}

```
Can you spot similarities and differences between the Python code and C? What are they? What does each line of code do?

Happy coding!
