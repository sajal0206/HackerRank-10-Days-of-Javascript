# Day 5: Inheritance

Objective

In this challenge, we practice implementing inheritance and use JavaScript prototypes to add a new method to an existing prototype. Check out the attached Classes tutorial to refresh what we've learned about these topics.

Task

We provide the implementation for a Rectangle class in the editor. Perform the following tasks:

Add an area method to Rectangle's prototype.
Create a Square class that satisfies the following:
It is a subclass of Rectangle.
It contains a constructor and no other methods.
It can use the Rectangle class' area method to print the area of a Square object.
Locked code in the editor tests the class and method implementations and prints the area values to STDOUT.


# Day 5: Template Literals

Objective

In this challenge, we practice using JavaScript Template Literals. Check the attached tutorial for more details.

Task

The code in the editor has a tagged template literal that passes the area and perimeter of a rectangle to a tag function named sides. Recall that the first argument of a tag function is an array of string literals from the template, and the subsequent values are the template's respective expression values.

Complete the function in the editor so that it does the following:

Finds the initial values of  and  by plugging the area and perimeter values into the formula:
where  is the rectangle's area and  is its perimeter.
Creates an array consisting of  and  and sorts it in ascending order.
Returns the sorted array.
Input Format

The first line contains an integer denoting .
The second line contains an integer denoting .

Constraints

Output Format

Return an array consisting of  and , sorted in ascending order.

Sample Input 0

10
14
Sample Output 0

10
14
Explanation 0

The locked code in the editor passes the following arrays to the tag function:

The value of  is [ 'The area is: ', '.\nThe perimeter is: ', '.' ].
The value of  is [ 140, 48 ], where the first value denotes the rectangle's area, , and the second value denotes its perimeter, .
When we plug those values into our formula, we get the following:

We then store these values in an array, [14, 10], sort the array, and return the sorted array, [10, 14], as our answer.


# Day 5: Arrow Functions

Objective

In this challenge, we practice using arrow functions. Check the attached tutorial for more details.

Task

Complete the function in the editor. It has one parameter: an array, . It must iterate through the array performing one of the following actions on each element:

If the element is even, multiply the element by .
If the element is odd, multiply the element by .
The function must then return the modified array.

Input Format

The first line contains an integer, , denoting the size of .
The second line contains  space-separated integers describing the respective elements of .

Constraints

, where  is the  element of .
Output Format

Return the modified array where every even element is doubled and every odd element is tripled.

Sample Input 0

5
1 2 3 4 5
Sample Output 0

3 4 9 8 15
Explanation 0

Given , we modify each element so that all even elements are multiplied by  and all odd elements are multipled by . In other words, . We then return the modified array as our answer.
