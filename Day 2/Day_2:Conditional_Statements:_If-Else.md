![image](https://user-images.githubusercontent.com/66727050/151688498-88a82463-5e62-4732-92e2-4d21727cd2b4.png)

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

<hr>

function getGrade(score) {
    let grade;
    // Write your code here
    if(score > 25 && score <= 30){
        return "A";
    } else if(score > 20 && score <= 25){
        return "B";
    } else if(score > 15 && score <= 20){
        return "C";
    } else if(score > 10 && score <= 15){
        return "D";
    } else if(score > 5 && score <= 10){
        return "E";
    } else{
        return "F";
    }
    return grade;
}

<hr>

function main() {
    const score = +(readLine());
    
    console.log(getGrade(score));
}
