![image](https://user-images.githubusercontent.com/66727050/151688670-0fd2f304-bba6-43b7-97e2-42a220bacba7.png)

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
 * Complete the vowelsAndConsonants function.
 * Print your output using 'console.log()'.
 */
 
 <hr>
 
function vowelsAndConsonants(s) {
    for(var i = 0; i < s.length; i++){
        if (s[i] == "a" || s[i] == "e" || s[i] == "i" || s[i] == "o" || s[i] == "u"){
            console.log(s[i]);
        }
    }
    for(var i = 0; i < s.length; i++){
        if (s[i] != "a" && s[i] != "e" && s[i] != "i" && s[i] != "o" && s[i] != "u"){
            console.log(s[i]);
        }
    }
}
<hr>

function main() {
    const s = readLine();
    
    vowelsAndConsonants(s);
}
