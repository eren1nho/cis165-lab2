CIS-165 Lab 2

Name: Ali Eren Olgun
Course Section: CIS-165-W198

Initial Plans

Program 1 - Sum of Two Numbers

I will store 50 and 100 in two integer variables. Then I will add the two numbers and store the answer in a variable called total. Finally, I will display the value of total.

Program 2 - Miles Per Gallon

I will store 312 miles and 16 gallons in variables. I will divide the miles by the gallons and store the result in an mpg variable. I will use a data type that allows decimal values because the MPG can have a fractional result. Finally, I will display the result with MPG units.

How to Compile and Run

Both programs can be compiled separately using:
g++ -std=c++17 -Wall -Wextra sum.cpp -o sum
g++ -std=c++17 -Wall -Wextra mpg.cpp -o mpg

and can be runned using:
./sum
./mpg


Code Explanation and Testing

sum.cpp

The program starts by storing 50 in first_number and 100 in second_number. It adds these two variables together and stores the answer in total. The program then uses cout to display total, which is 150.

Storing the answer in total before printing makes the calculation and output separate steps. It also follows the assignment requirement to calculate the result first instead of doing the calculation directly inside cout.

For my changed-value test, I used 200 as first_number and 70 as second_number and i got 270 as total which verifies the code.

mpg.cpp

The MPG formula is miles divided by gallons. The program stores 312 in miles and 16 in gallons. It calculates miles / gallons and stores the answer in mpg. The result is then displayed with the MPG unit.

I used double because MPG calculations can have decimal answers. If C++ divides two integers, it can perform integer division and remove the fractional part of the result. Using double allows the program to keep the decimal portion.

For my changed-value test, I used 250 miles and 12 gallons. The program calculated 250 / 12, which gave approximately 20.8333 MPG. The result was stored in mpg before being displayed.