![image](https://user-images.githubusercontent.com/66727050/151692058-397d9c31-6a6a-48de-9485-a2d5c5ed4960.png)

# Solution:

/*
 * Implement a Polygon class with the following properties:
 * 1. A constructor that takes an array of integer side lengths.
 * 2. A 'perimeter' method that returns the sum of the Polygon's side lengths.
 */
 
 <hr>
    class Polygon{
        constructor (sides){
            this.sides = sides;
        }
        perimeter() {
            var perm = 0;
            for (var i = 0; i < this.sides.length ; i++){
                perm = this.sides[i] + perm;
            }
            return perm;
        }
    }
<hr>

const rectangle = new Polygon([10, 20, 10, 20]);
const square = new Polygon([10, 10, 10, 10]);
const pentagon = new Polygon([10, 20, 30, 40, 43]);

console.log(rectangle.perimeter());
console.log(square.perimeter());
console.log(pentagon.perimeter());
