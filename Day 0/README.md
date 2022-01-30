# Day 0: Hello, World!
Overview: 10 Days of JavaScript
This series focuses on learning and practicing JavaScript. Each challenge comes with a tutorial article, and you can view these articles by clicking either the Topics tab along the top or the article icon in the right-hand menu.

Objective

In this challenge, we review some basic concepts that will get you started with this series. Check out the tutorial to learn more about JavaScript's lexical structure.

Task

A greeting function is provided for you in the editor below. It has one parameter, . Perform the following tasks to complete this challenge:

Use console.log() to print Hello, World! on a new line in the console, which is also known as stdout or standard output. The code for this portion of the task is already provided in the editor.
Use console.log() to print the contents of  (i.e., the argument passed to main).
You've got this!

Input Format

Data Type	Parameter	Description
string		A single line of text containing one or more space-separated words.
Output Format

Print the following two lines of output:

On the first line, print Hello, World! (this is provided for you in the editor).
On the second line, print the contents of .
Sample Input 0

Welcome to 10 Days of JavaScript!
Sample Output 0

Hello, World!
Welcome to 10 Days of JavaScript!
Explanation 0

We printed two lines of output:

We printed the literal string Hello, World! using the code provided in the editor.
The value of  passed to our main function in this Sample Case was Welcome to 10 Days of JavaScript!. We then passed our variable to console.log, which printed the contents of .


# Day 0: Data Types
Objective

Today, we're discussing data types. Check out the attached tutorial for more details.

Task

Variables named , , and  are declared for you in the editor below. You must use the  operator to perform the following sequence of operations:

Convert  to an integer (Number type), then sum it with  and print the result on a new line using console.log.
Convert  to a floating-point number (Number type), then sum it with  and print the result on a new line using console.log.
Print the concatenation of  and  on a new line using console.log. Note that  must be printed first.
Input Format

Data Type	Parameter	Description
string		The string representation of an integer you must sum with .
string		The string representation of a floating-point number you must sum with .
string		A string of one or more space-separated words you must append to .
Output Format

Print the following three lines of output:

On the first line, print the sum of  and the integer representation of .
On the second line, print the sum of  and the floating-point representation of .
On the third line, print  concatenated with . You must print  before .
Sample Input 0

12
4.32
is the best place to learn and practice coding!
Sample Output 0

16
8.32
HackerRank is the best place to learn and practice coding!
Explanation 0

When we sum the integers  and , we get the integer .
When we sum the floating-point numbers  and , we get . When we concatenate HackerRank with is the best place to learn and practice coding!, we get HackerRank is the best place to learn and practice coding!.

You will not pass this challenge if you attempt to assign the Sample Case values to your variables instead of following the instructions above.


# Day 1: Arithmetic Operators
Objective

In this challenge, we practice using arithmetic operators. Check out the attached tutorial for resources.

Task

Complete the following functions in the editor below:

getArea(length, width): Calculate and return the area of a rectangle having sides  and .
getPerimeter(length, width): Calculate and return the perimeter of a rectangle having sides  and .
The values returned by these functions are printed to stdout by locked stub code in the editor.

Input Format

image

image

Constraints

 and  are scaled to at most three decimal places.
Output Format

image

Sample Input 0

3
4.5
Sample Output 0

13.5
15
Explanation 0

The area of the rectangle is .
The perimeter of the rectangle is .


# Day 1: Functions
Objective

Today, we're discussing JavaScript functions. Check out the attached tutorial for more details.

Task

Implement a function named factorial that has one parameter: an integer, . It must return the value of  (i.e.,  factorial).

Input Format

Locked stub code in the editor reads a single integer, , from stdin and passes it to a function named factorial.

Constraints

Output Format

The function must return the value of .

Sample Input 0

4
Sample Output 0

24
Explanation 0

We return the value of .

