# Day 4: Create a Rectangle Object

Objective

In this challenge, we practice creating objects. Check out the attached tutorial for more details.

Task

Complete the function in the editor. It has two parameters:  and . It must return an object modeling a rectangle that has the following properties:

: This value is equal to .
: This value is equal to .
: This value is equal to 
: This value is equal to 
Note: The names of the object's properties must be spelled correctly to pass this challenge.

Input Format

The first line contains an integer denoting .
The second line contains an integer denoting .

Constraints

Output Format

Return a object that has the properties specified above. Locked code in the editor prints the returned object's , , , and  to STDOUT.

Sample Input 0

4
5
Sample Output 0

4
5
18
20
Explanation 0

Given a  of  and a  of , the Rectangle object's  is  and its  is .


# Day 4: Count Objects

Objective

In this challenge, we learn about iterating over objects. Check the attached tutorial for more details.

Task

Complete the function in the editor. It has one parameter: an array, , of objects. Each object in the array has two integer properties denoted by  and . The function must return a count of all such objects  in array  that satisfy .

Input Format

The first line contains an integer denoting .
Each of the  subsequent lines contains two space-separated integers describing the values of  and .

Constraints

Output Format

Return a count of the total number of objects  such that . Locked stub code in the editor prints the returned value to STDOUT.

Sample Input 0

5
1 1
2 3
3 3
3 4
4 5
Sample Output 0

2
Explanation 0

There are  objects in the  array:

Because we have two objects  that satisfy  (i.e.,  and ), we return  as our answer.


# Day 4: Classes

Objective

In this challenge, we practice using JavaScript classes. Check the attached tutorial for more details.

Task

Create a Polygon class that has the following properties:

A constructor that takes an array of integer values describing the lengths of the polygon's sides.
A perimeter() method that returns the polygon's perimeter.
Locked code in the editor tests the Polygon constructor and the perimeter method.

Note: The perimeter method must be lowercase and spelled correctly.

Input Format

There is no input for this challenge.

Output Format

The perimeter method must return the polygon's perimeter using the side length array passed to the constructor.

Explanation

Consider the following code:

// Create a polygon with side lengths 3, 4, and 5
let triangle = new Polygon([3, 4, 5]);

// Print the perimeter
console.log(triangle.perimeter());
When executed with a properly implemented Polygon class, this code should print the result of .
