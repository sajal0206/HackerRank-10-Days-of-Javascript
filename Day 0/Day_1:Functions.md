![image](https://user-images.githubusercontent.com/66727050/151688321-ad3b5db8-86e6-44a5-8484-7bb8ea7e346e.png)

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
 * Create the function factorial here
 */
 <hr>
    function factorial(n){
        let fact = n;
        while(n > 2){
            fact *= (n-1);
            n--;
        }
        return fact;
    }
<hr>
