Download Link: https://assignmentchef.com/product/solved-ch-230-a-assignment-10-classes-objects-and-methods
<br>
<h1><strong>Problem 10.1 </strong>Error messages produced by the compiler</h1>

<h1>Comment out the using namespace std; and then take your time, read and interpret the error messages.</h1>

<ol>

 <li>Also remove the Critter:: prefix in one of the methods in Critter.cpp, read and interpret the error message.</li>

</ol>

Then create a file called explanations.txt. This file should be uploaded together with the other files and should contain your descriptions and interpretations of the errors as well as your comments on potential alternative solutions. <em>You can assume that the input will be valid.</em>

<table width="457">

 <tbody>

  <tr>

   <td width="457"><strong>Problem 10.2 </strong><em>The Critter class</em></td>

  </tr>

  <tr>

   <td width="457"> </td>

  </tr>

 </tbody>

</table>

Use the previously given files: Critter.h, Critter.cpp and testcritter.cpp. Expand Critter.h by two additional properties of your choice, and corresponding setter and getter methods, then adjust Critter.cpp and testcritter.cpp accordingly.

Also adapt the print() method such that the new properties are printed on the screen as well. <em>You can assume that the input will be valid.</em>

<table width="457">

 <tbody>

  <tr>

   <td width="457"><strong>Problem 10.3 </strong><em>A City class</em></td>

  </tr>

 </tbody>

</table>

<h2>Language: C++</h2>

Create a class named City. Assume that a city has a name, a number of inhabitants, a mayor and an area (in <em>km</em><sup>2</sup>).

Then create three instances of this class: <em>Bremen</em>, <em>Paris </em>and <em>London</em>. Provide suitable setter and getter methods for each of these properties. The class declaration has to be placed into City.h, the class definition has to be placed into City.cpp and the test program where the instances are created has to be in testcity.cpp.

You can set the needed data from the main() function by initialization or read it from the keyboard.

<h1><strong>Problem 10.4 </strong>Constructors for Critter</h1>

Add three constructors to the class Critter. Each constructor should also print a simple informational message on the screen such that one can see when and which constructor has been called.

You should be able to create an instance of the Critter class

<ul>

 <li>without supplying any properties (which should set the name to ”default_critter”, the height to 5 and the rest to 0),</li>

 <li>by only supplying a name as parameter (which should set the height to 5 and the rest to 0), and also</li>

 <li>by supplying <em>name</em>, <em>hunger</em>, <em>boredom </em>and <em>height </em>all as parameters. You should also be able to create an instance of the Critter class without specifying the <em>height</em>. If the <em>height </em>is not supplied, the critter has the default height of 10.</li>

</ul>

Write a test program which creates four instances of the Critter by using these three different constructors (the last one in two ways). Set their <em>hunger </em>levels to 2 by using appropriate method and/or constructor calls. The critters’ properties should then be printed on the screen. Name the files Critter.h, Critter.cpp and testcritter.cpp.

<h1><strong>Problem 10.5 </strong>Information hiding I</h1>

A game developer crew has decided to rather use a percentage scale (double value between 0<em>.</em>0 and 1<em>.</em>0) to represent the <em>hunger </em>level of a critter. Change the internal structure of the class to reflect this. However, your <strong>existing test program should run without any modifications </strong>(therefore the public class interface stays the same) and you will need to find a way to convert the current <em>hunger </em>levels from integer values (which are from 0 to 10) to doubles and then from doubles back to integers. Use separate methods for doing this.

Use a simple mapping scheme like 10 is 1<em>.</em>0, 9 is 0<em>.</em>9, 8 is 0<em>.</em>8 …1 is 0<em>.</em>1, and 0 is 0<em>.</em>0.

Name the files Critter.h, Critter.cpp and testcritter.cpp (<strong>must remain unchanged</strong>). The implementation for the conversions needs to be put into Critter.cpp and should not be part of the public interface.

The client program testcritter.cpp from the previous problem <strong>must remain unchanged</strong>.

The <em>hunger </em>levels of the critters should be “internally” at 0<em>.</em>2 (meaning 20%). <em>You can assume that the setting values are always valid.</em>

<h1><strong>Problem 10.6 </strong>Information hiding II</h1>

Next a <em>thirst </em>level (as double value) should be added to the properties of a critter. Add a new constructor that takes five parameters for setting all properties of a critter.

Make also sure that the existing constructors will still work. For the existing constructors, the <em>thirst </em>level should be set to the same level as the <em>hunger </em>level. Your existing testcritter.cpp must still be able to run <strong>in its unchanged form</strong>. So the already existing constructors need to support the change. Name the files Critter.h, Critter.cpp and testcritter.cpp.

Finally, you should adapt the print method for printing on the screen also the value of the thirst level as a double. The client program testcritter.cpp may contain one additional line, where the constructor taking five parameters is being called.

<em>You can assume that the setting values are always valid.</em>

<table width="457">

 <tbody>

  <tr>

   <td width="457"><strong>Problem 10.7 </strong><em>Copy constructor</em></td>

  </tr>

 </tbody>

</table>

Based on the source code of copyconstructor.cpp implement the method funcByref(). Change all constructors (including the copy constructor) such that <strong>you can clearly see when and which of them is invoked </strong>by adding a message which is printed on the screen.

Then in your main() function create at least two objects using the different constructors, call funcByVal(), funcByRef(), and print the results on the screen. Then make sure that the memory occupied by the objects will be released by the end of the program. <em>You can assume that the setting values are always valid.</em>

<h1><strong>Problem 10.8 </strong>A Complex class</h1>

Create a class named Complex for storing and managing complex numbers. A complex number has an real part and an imaginary part. The class has to provide a default constructor initializing the properties by 0, another constructor for setting the properties with specific values, a copy constructor and an empty destructor. Provide suitable setter and getter methods for each property and a method for printing the complex number on the screen in its mathematical form (e.g., 1+2<em>i</em>, 3 − 5<em>i</em>). Also provide methods for the conjugation of a complex number, and for adding, subtracting and multiplying two complex numbers. The class declaration has to be placed into Complex.h, the class definition has to be placed into Complex.cpp and the test program where the instances are created has to be in testcomplex.cpp. The test program should create at least two instances of the Complex class, the data for the properties should be read from the keyboard. Then:

<ol>

 <li>the conjugate of the first instance should be determined and printed on the screen;</li>

 <li>the sum of the two instances should be determined and printed on the screen;</li>

 <li>the difference between the second and first instance should be determined and printed onthe screen;</li>

 <li>the multiplication of the two instances should be determined and printed on the screen.</li>

</ol>

The prototypes of the methods for adding, subtracting and multiplying must have the following form:

Complex Complex::add(Complex); Then the usage will be the following:

Complex c1, c2, c3; … c3 = c1.add(c2);

Note: If <em>z </em>= <em>a </em>+ <em>bi </em>then <em>z </em>= <em>a </em>− <em>bi</em>. If <em>z</em><sub>1 </sub>= <em>a </em>+ <em>bi </em>and <em>z</em><sub>2 </sub>= <em>c </em>+ <em>di </em>then <em>z</em><sub>1</sub>+ <em>z</em><sub>2 </sub>= (<em>a </em>+ <em>c</em>)+(<em>b </em>+ <em>d</em>)<em>i</em>, <em>z</em><sub>1 </sub>− <em>z</em><sub>2 </sub>= (<em>a </em>− <em>c</em>)+(<em>b </em>− <em>d</em>)<em>i </em>and <em>z</em><sub>1 </sub>· <em>z</em><sub>2 </sub>= (<em>a </em>· <em>c </em>− <em>b </em>· <em>d</em>)+(<em>b </em>· <em>c </em>+ <em>a </em>· <em>d</em>)<em>i</em>.

<em>You can assume that the input will be valid.</em>