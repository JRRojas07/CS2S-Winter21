# LAB 4

4.1 READ ME
# Working with Integer Division

## Step 1

Run this program and examine the output. The program is trying to calculate a batting average but it does not seem to be working correctly. 

There is a logic error in this program centering around data types. Does changing the data type of `batAvg` from `int` to `double` solve the problem? Make that change and run the program again and examine the result. 

## Step 2: Why is the result zero?

When you use the division operator / on two integer numbers, the result is an integer number. This can be a problem if you expect a fraction. Moreover, the problem can easily go unnoticed, resulting in a program that looks fine but is producing incorrect output without your even being aware of the problem. In order to receive a floating-point result when dividing 2 numbers, at least one of the numbers must be a floating-point type.

Continue to work with this program until you get the correct result. The correct result should be around 0.292162.

PROGRAM
#include <iostream>
using namespace std;

int main()
{
  float atBats = 421;
  float hits = 123;
	float batAvg;

	batAvg = hits / atBats;									
  // an assignment statement 
	cout << "The batting average is " << batAvg << endl;	// output the result

}

4.2 READ ME

