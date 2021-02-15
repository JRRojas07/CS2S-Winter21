# LAB 1

1.1 READ ME

# Running Your First Program 
Examine the program in the code editor panel.


Run the program by clicking the "run" button above the panel.


You should see a message printed in the console window that corresponds with the text inside the quotes.


Change the program so it produces this **exact** output:


**C++**
**programming**
**is fun!**


You may have to add an extra line of code.

PROGRAM
#include <iostream>

using namespace std;

int main() {
  cout << endl;
  cout << "C++\n";
	cout << "programing\n";
  cout << "is so fun!";

}

1.2 READ ME
# Fixing a Program with a Syntax Error 

A Syntax Error is an error in the "grammar" of the programming language. These are caught by the compiler and listed out with line number and error found. You will learn how to understand what they tell you with experience. All syntax errors must be corrected before the program will run. If the program runs, this does not mean that it is correct, only that there are no syntax errors. Examples of syntax errors are spelling mistakes in variable names, missing semicolon, unpaired curly braces, etc. 

Try running the program. Here we have our first example of the many syntax errors that you no doubt will encounter in this course. The error message you receive may be different depending on the system you are using, but the compiler insists that there is a syntax error somewhere. Unfortunately, where the message indicates that the problem exists, and where the problem actually occurs may be two different places. 

To correct the problem place a closing  semicolon after the line:

`cout << "Today is a great day for Lab"` 

Most syntax errors are not as easy to spot and correct as this one. 

Re-compile the program and when you have no syntax errors, run the program and input 9 when asked (press enter after entering 9). Make sure the answer is correct (18).

PROGRAM
#include <iostream>

using namespace std;

int main() {
  
  int number;
	float total;
	
	cout << "Today is a great day for Lab\n";
	cout << "Type in a number of your choice and press Enter\n";
	cin  >> number;
	
	total = number * 2;
	cout << total << " is twice the number you typed\n";
  
}
LAB 1.3
# Running a Program with a Runtime Error 

Run time errors—errors that do not occur until the program is run, and then may only occur with some data. These errors emphasize the need for completely testing your program. 

Compile and run the program. Enter a number and press return. You should now see a run time error. There was no syntax or grammatical error in the program. However, just like commanding someone to break a law of nature, the program is asking the computer to break a law of math by dividing by zero. It cannot be done. 

Correct this program by having the code divide by 2 instead of 0.

Re-compile and run the program. Type 9 when asked for input. 

The runtime error should be gone, but does it gives the correct output? If not, change the data type of the `number` variable from `int` to `float.` Floating-point type variables are needed to hold numbers with a decimal point. Re-compile, run the program again, and see if entering 9 now gives the correct output.

PROGRAM
#include <iostream>

using namespace std;

int main() {
  
  float number;
	int divider;
	
	divider = 2;
	
	cout << "Hi there\n";
	cout << "Please input a number and then hit return\n";
	cin  >> number;
	
	number = number / divider;
	
	cout << "Half of your number is " << number << endl;
  
}

1.4 READ ME
# Working with Logic Errors

Logic Errors—errors in the logic of the algorithm. These errors emphasize the need for a correct algorithm. If the statements are out of order, if there are errors in a formula, or if there are missing steps, the program can still run and give you output, but it may be the wrong output. Since there is no list of errors for logic errors, you may not realize you have errors unless you check your output. 

It is very important to know what output you expect. You should test your programs with different inputs, and know what output to  expect in each case. Calculate each case by hand before running your program so that you know what to expect. You may get a correct answer for one case, but not for another case. This will help you figure out where your logic errors are.

Compile and run this program. You should get no syntax errors. Is the output correct? If not, why?

This program has no syntax or runtime errors, but it certainly has a logic error. Logic errors may create a challenge for the programmer. Find the problem. 

Fix the bug. Ask for help if needed.

PROGRAM
#include <iostream>
#include <string>

using namespace std;

int main() {
  
  float TAX_RATE = 0.055;
  float price;
  float tax;
  float total;
  string item;
  
  // Display prompts and get input.
  cout << "Item description (no spaces):  ";
  cin >> item;
  cout << "Item price:  $";
  cin >> price;
  
  // Perform the calculations.
  tax = (price * TAX_RATE);
  total = (price + tax);

  // Display the results.
  cout << item << "   $" << price << endl;
  cout << "Tax   $" << tax << endl;
  cout << "Total   $" << total << endl;
}

1.5 READ ME
# Writing Your First Program

Develop a program that converts from kilometers to miles. 

Read in a number that represents the number of kilometers traveled. 

Convert this number to miles and then output it to the console.

1 kilometer = 0.621 miles.

To get started, make a copy of your solution from Lab 1.2 and paste it in the code editor panel. Modify this file to implement your solution to convert kilometers to miles. 

Try running your program.  If you get syntax errors, try to fix them and re-compile until your program is free of syntax errors. Is your output what you expect from the input you gave? If not, try to find and correct the logic error and run the program again. Continue this process until you have a program that produces the correct result. 

PROGRAM

#include <iostream>

using namespace std;

int main() {
  
  float kilometers;
	float miles;
	
  cout << "Please enter number of kilometers.\n";
	cin  >> kilometers;
	
	miles = kilometers * 0.621;
  cout << endl;
  cout << kilometers << " kilometers = " << miles << " miles";

}

