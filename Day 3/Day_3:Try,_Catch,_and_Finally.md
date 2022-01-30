![image](https://user-images.githubusercontent.com/66727050/151689173-dcc00639-c087-4c65-9c7e-3a4da1ce203e.png)

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
 * Complete the reverseString function
 * Use console.log() to print to stdout.
 */
 <hr>
function reverseString(s) {
    try{
        let newStr = s.split("");
        let reversed = newStr.reverse();
        console.log(reversed.join(""));
    } catch (e){
        console.log(e.message+"\n"+s);
    }
}
<hr>

function main() {
    const s = eval(readLine());
    
    reverseString(s);
}
