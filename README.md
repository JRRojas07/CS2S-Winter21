# LAB 2

2.1 READ ME
# Working with the cout Statement

In the previous week's lab we saw how the `cout` statement can be used to display text output. To get started, copy your code from Lab 1.1 into the editor panel.  

# Exercise 1

Fill in code so that the program will do the following:


- Write your first and last name on one line.
- Write your sign of the zodiac on the next line.
- Write your favorite color on the next line. 
- Write your favorite animal on the next line. 

Remember that to output a string literal, such as `"Hello"`, you must use quotes. 


Run the program. 


Example Output: 

**Hector Smith
Taurus
Blue
Rabbits**


# Exercise 2

Change the program so that a blank line separates your zodiac sign from your favorite color.

**Hector Smith
Taurus**

**Blue
Rabbits**

# Exercise 3

Change the program so that the following (but with your name and info) is printed, including asterisks. Try to get the spacing for the right column to align similar to the the example. 

**\*\*\*\*\*\*\*\*\*\*\*\*
Programmer: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Hector Smith
Zodiac Sign: &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Taurus**

**Favorite Color: &nbsp;&nbsp;&nbsp;Blue
Favorite Animal: Rabbit
\*\*\*\*\*\*\*\*\*\*\***

Run the program and verify it's correct. Submit the code when you are finished with Exercise 3. You do NOT have to submit code individually for Exercise 1 and 2.

PROGRAM
#include <iostream>
using namespace std;

int main() {

cout << endl;
  cout << "************\n";
  cout << "Programmer: Juan Rojas\n";
  cout << "Zodiac Sign: Leo\n";
  cout << endl;
  cout << "Favorite Color: Burgandy?\n";
  cout << "Favorite Animal: Hedgehog\n";
  cout << "************\n";

}

2.2 READ ME
# Working with Variables and Arithmetic Operators

Fill in the statements in the main.cpp file so that the output will produce the following:  
 
***The circumference of the circle is 33.9292
The area of the circle is 91.6088
The diameter of the circle is 10.8***

Wherever there is a message in the comments saying `"Fill in code ..."` you should add C++ statements as directed.

To square a number you can multiply it by itself.

num squared = num x num

PROGRAM
#include <iostream>
using namespace std;

int main()
{
  cout << endl;
  double pi = 3.14159;
  double radius = 5.4;
  double circumference = 2*pi*radius; 
  // definition of circumference

  double area = 2*pi*radius;
  // Fill in code to define an area variable

  double diameter = circumference/pi;
  // Fill in code to define a diameter variable

  circumference = 2 * pi * radius; // computes circumference

  area = pi*radius*radius;
  // Fill in code to compute the area of a circle

  diameter =circumference/pi;
  // Fill in code to compute the diameter of a circle

  cout << "The circumference of the circle is " << circumference << endl;
  
  cout << "The area of the circle is " << area << endl;
  // Fill in code for a cout statement to output the area
  
  cout << "The diameter of the circle is " << diameter << endl;
  // Fill in code for a cout statement to output the diameter

}

2.3 READ ME
# Rectangle Area and Perimeter

Using Lab 2.2 as an example, develop a program that will determine the area and perimeter of a rectangle. The length and width should be given as variables (length = 8, width = 3)

To get started, copy your code from Lab 2.2 into the editor panel. Now modify it to find the area and perimeter of a rectangle with a length and width of 8 and 3.

Continue to work on it until you get the following output: 

***The area of the rectangle is 24
The perimeter of the rectangle is 22***

PROGRAM
#include <iostream>
using namespace std;

int main()
{
float length;
float width;
float area;
float perimeter;

width = 3;
length = 8;

area = length * width;
perimeter = 2 * (length + width);

cout << "The area of the rectangle is " << area << ".\n";
cout << "The perimeter of the rectangle is " << perimeter << ".\n";

}

