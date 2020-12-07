# Coding With C

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



### Proceduarl Oriented Programming (POP) ###
* Data is exposed and can be easily modified, not abstracted
* Uses classes and objects, however not in the same way that OOP does
* Easy to add new functions without changing the data structure
* Classes don’t always have their own functions

Many coding languages such as Python, Java, Ruby and C++ use OOP as they are very user friendly. With Python, the code is written, run in the interpreter and an output is given using an IDE so that machines can understand it. Python is a high-level language and is very person oriented, meaning that it’s easy for humans to intuitively understand and interpret. C is what’s called a low-level language and more machine oriented, so it’s easier for a machine to read but harder for a human to understand. It is put through a compiler and then an executor and the output does not have to go through an IDE. 


Use modular units that are blocks of code that can easily be changed or added without disrupting the operation


C is not used in GIS the same way we use Python, as C is more commonly used to code hardware devices and heavyweight development. This means that it is used to code processing system and geospatial libraries such as the Geospatial Data Abstraction Library (GDAL), 

There’s not really a consensus on the best programming languages for GIS

but python is used for more scripting and data processing, analysis & modeling, web mapping. 

Java, C, C++ are statically typed and show you errors during compilation time, and Python, JavaScript show errors when you run it, they are dynamic typing languages. As we saw with ArcGIS and Python, we often didn’t know the error until after running but with C, it’s not like that 

However there a lot of open source GIS projects written in C (also uses C++ and Python) such as the  that reads raster and vector data. A lot of GIS software uses GDAL such as ArcGIS, ENVI which is a remote sensing software, Google Earth, GRASS GIS (Geographic Resources Analysis Support System), QGIS, R 

Knowing C is important as it is the base of many other coding languages, however tools that are used more commonly by GIS specialists include Java, JavaScript, C++, C#, R, HTML, SQL.

Now that we have some background knowledge on C, let's code in Python and also C! We will be using a lab that is taken from IDCE 302: Python Programming. 



