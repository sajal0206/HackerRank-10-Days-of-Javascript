![image](https://user-images.githubusercontent.com/66727050/151691439-37350fe9-c149-44cb-a4c3-8fa59ac9c335.png)

# Solution:

'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Return a count of the total number of objects 'o' satisfying o.x == o.y.
 * 
 * Parameter(s):
 * objects: an array of objects with integer properties 'x' and 'y'
 */
 <hr>
function getCount(objects) {
    var count = 0;
    for (var i = 0; i<Object.keys(objects).length; i++){
        if (objects[i].x == objects[i].y){
            count++;
        }
    }
        return count;    
}
<hr>

function main() {
    const n = +(readLine());
    let objects = [];
    
    for (let i = 0; i < n; i++) {
        const [a, b] = readLine().split(' ');
        
        objects.push({x: +(a), y: +(b)});
    }
    
    console.log(getCount(objects));
}
