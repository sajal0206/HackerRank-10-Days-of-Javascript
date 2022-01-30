![image](https://user-images.githubusercontent.com/66727050/151711902-3ef51671-66bf-4a6f-9453-2c35ade05a2b.png)

# Solution:

class Rectangle {
    constructor(w, h) {
        this.w = w;
        this.h = h;
    }
}

/*
 *  Write code that adds an 'area' method to the Rectangle class' prototype
 */
 
 <hr>
    Rectangle.prototype.area = function () {
        return this.w * this.h;
    };
/*
 * Create a Square class that inherits from Rectangle and implement its class constructor
 */
class Square extends Rectangle{
    constructor (s){
        super (s, s);
    }
}
<hr>
if (JSON.stringify(Object.getOwnPropertyNames(Square.prototype)) === JSON.stringify([ 'constructor' ])) {
    const rec = new Rectangle(3, 4);
    const sqr = new Square(3);
    
    console.log(rec.area());
    console.log(sqr.area());
} else {
    console.log(-1);
    console.log(-1);
}
