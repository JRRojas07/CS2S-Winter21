# Lab 3

3.1 READ ME

# cin Statements and Formatting
## Exercise 1

Complete the program so that a sample run inputting `22` for the number of items bought and `10.98` for the price of each item will produce the results below.

Sample run of the program:

`Please input the number of items bought`
**22**
`Please input the price of each item`
**10.98**
`The total bill is $241.5600`


## Exercise 2

Once you have the program working, change the statement:

`cout << setprecision (4) << fixed;`

to

`cout << setprecision(4);`

Rerun the program with the same data given in Exercise 1. 

How does the use of the `fixed`  manipulator change how the `setprecision` function formats the decimal number? Make a note in your notes about how `fixed` and `setprecision` work.

## Exercise 3

Now configure the program so that decimal numbers are formatted for two places to the right of the decimal point when outputted. You may need to put the `fixed` manipulator back and adjust the `setprecision` function.

PROGRAM 
#include <iostream>
#include <iomanip>
using namespace std;

int main()
{
	int	quantity;		// contains the amount of items purchased 
	double itemPrice;	// contains the price of each item
	double totalBill;	// contains the total bill.

  cout << endl;
	cout << setprecision(2) << fixed;	
  // formatted output 
	
	cout << "Please input the number of items bought\n";
	cin >> quantity;

	cout << "Please enter the price for each item\n";
  // Fill in the prompt to ask for the price.

  cin >> itemPrice;
	// Fill in the input statement to bring in the price of each item.

  totalBill = itemPrice * quantity;
	// Fill in the assignment statement to determine the total bill.

  cout << "The total bill is $" << totalBill << ".\n";
	// Fill in the output statement to print total bill,
	// with a label to the screen.

  //Fixed + Set Precision vs Set Precision

  //Fixed + Set Prec. sets my decimal answers to the number that set prec has, in this example it gives my answers with 4 digits after the decimal place
  
  //ONLY set prec cuts off the decimal answer at the next non zero number. 


}

3.2 READ ME
# Furniture Company

The Supremo Furniture Company sells the following three styles of chairs: 

Style             |Price Per Chair 
------------------|---------------
American Colonial | $85.00 
Modern            | $57.50 
French Classical  | $127.75 

Write a program that will input the amount of chairs sold for each style. It will print the total dollar sales of each style as well as the total sales of all chairs in fixed point notation with two decimal places. 

Sample run: 

`Please input the number of American Colonial chairs sold `
**20** 
`Please input the number of Modern chairs sold `
**15**
`Please input the number of French Classical chairs sold `
**5** 

`The total sales of American Colonial chairs $1700.00 `
`The total sales of Modern chairs $862.50 `
`The total sales of French Classical chairs $638.75 `
`The total sales of all chairs $3201.25 `

PROGRAM
#include <iostream>
#include <iomanip>
using namespace std;

int main() {

double americanColonial;
int soldAmerican = 0;
double modern;
int soldModern = 0;
double frenchClassical;
int soldFrench = 0;

cout << setprecision(2) << fixed;	

cout << endl;
cout << "Please enter the amount of American Colonial chairs sold. \n";
cin >> soldAmerican;
cout << endl;
cout << "Please enter the amount of Modern chairs sold\n";
cin >> soldModern;
cout << endl;
cout << "Please enter the amount of French Classical chairs sold\n";
cin >> soldFrench;

americanColonial = 85;
modern = 57.50;
frenchClassical = 127.75;

double totalAmerican = americanColonial * soldAmerican;
double totalModern = modern * soldModern;
double totalFrench = frenchClassical * soldFrench; 

cout << "The total sales of American Colonial chairs is $" << totalAmerican << ".\n";
cout <<"The total sales of Modern chairs is $" << totalModern << ".\n";
cout << "The total sales of French Classical chairs is $" << totalFrench << ".\n";

}

3.3 READ ME
# Sales and Taxes

Write a program that will input total sales that a business generates for a particular month. The program will also input the state and local sales tax percentage. It will output the total sales plus the state tax and local tax to be paid. The output should be in fixed notation with 2 decimal places. 

Sample run: 

`Please input the total sales for the month `
**1080** 
`Please input the state tax percentage in decimal form (.02 for 2%) `
**.06** 
`Please input the local tax percentage in decimal form (.02 for 2%) `
**.02** 

`The total sales for the month is $1080.00 `
`The state tax for the month is $64.80 `
`The local tax for the month is $21.60 `

PROGRAM
#include <iostream>
#include <iomanip>
using namespace std;

int main() {

double totalSalesTax;
double stateTax;
double localTax;

cout << setprecision(2) << fixed;	
cout << endl;


cout << "Please input the total sales tax for each month.\n";
cin >> totalSalesTax;

cout << "Please input the state tax percentage in decimal form.\n";
cin >> stateTax;
cout << "Please input the local tax percentage in decimal form.\n";
cin >> localTax;

cout << "The total sales tax for the month is $" << totalSalesTax << endl;


cout << "The state tax for the month is $" << stateTax * totalSalesTax << endl;
cout << "The local tax for the month is $" << localTax * totalSalesTax << endl;


}

PROGRAM
