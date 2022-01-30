![image](https://user-images.githubusercontent.com/66727050/151713494-8126e21f-8f8c-47fe-9278-4a04c81619a3.png)

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
 * Modify and return the array so that all even elements are doubled and all odd elements are tripled.
 * 
 * Parameter(s):
 * nums: An array of numbers.
 */
function modifyArray(nums) {
    <hr>
    for (var i = 0; i < nums.length; i++){
        if(nums[i]%2 == 0){
            nums[i] = nums[i] * 2;
        } else {
            nums[i] = nums[i] * 3;            
        }
    }
    return nums;
}
<hr>

function main() {
    const n = +(readLine());
    const a = readLine().split(' ').map(Number);
    
    console.log(modifyArray(a).toString().split(',').join(' '));
}
