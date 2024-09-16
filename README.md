Overview....

This C++ program demonstrates a simplified implementation of Shamir's Secret Sharing algorithm using Lagrange interpolation. The code is designed to compute the constant term of a polynomial given a set of points in different bases. The polynomial is used to share a secret, and the constant term (which is the secret) is reconstructed from the provided points.

Functionality.......

Base Conversion: Converts numbers from various bases to decimal format.
Lagrange Interpolation: Calculates the constant term of the polynomial given points using Lagrange interpolation.

Test Cases: Computes and outputs the constant term for two example test cases.
Compilation and Execution
Prerequisites
Ensure you have a C++ compiler installed. You can use compilers like g++ for Linux or MinGW for Windows.

Compilation.........

To compile the code, run the following command in your terminal or command prompt:

g++ -o secret_sharing
secret_sharing.cpp


This will generate an executable named secret_sharing.

Execution.....
To run the compiled executable, use the following command:

./secret_sharing
On Windows, use:

secret_sharing.exe

Code Breakdown....
Functions....
baseToDecimal(const string& number, int base): Converts a number from a given base to decimal. The number is provided as a string, and base specifies the base of the number system.

calculateConstantTerm(const vector<pair<int, int>>& points): Calculates the constant term (the secret) of the polynomial using Lagrange interpolation. It processes the given points and computes the constant term of the polynomial.

Main Function
The main function includes two test cases:

Test Case 1:

Input points are given in various json format these points.
Computes and outputs the constant term for the polynomial.
Test Case 2:

Similar to Test Case 1 but with a different set of input points and a different number of required points.
Outputs the constant term for this test case.
Example Output...

The constant term (c) for test case 1 is: 4
The constant term (c) for test case 2 is:  3.04 

The output shows the computed constant term for each test case.

Notes.....
The program assumes valid input and does not include extensive error handling for base conversion or interpolation calculations.
For real-world applications, additional checks and error handling would be required to ensure the robustness of the implementation.
