# JavaScript-Function-and-Spread-args-Operator
In this illustrations, we show Functions and the use of JavaScript spread operator

<pre>
<code>
// In this illustrations, we show functions and the use of JavaScript spread operator


// EXAMPLE 1
// Using spread operator, with no specified arguments in the function
'use strict'    

// Using 'strict' mode before the program helps ensure writing good code and ensure the JavaScript code is secure

function Reading(...args){
    console.log(args);
}
Reading(12);                    // [12]  only one argument is passed
Reading(12, 14);                // [12, 14]    two arguments are passed
Reading(12, 14, 12);          // [ 12, 14, 12 ]  three arguments are passed
                            // here, spread allows to enter the arguments one needs, either one, two, three or more
                            // then the function is called


// EXAMPLE 2
// With specified arguments, i.e., a, b, c

function summed (a, b, c, d){
    return a * b * c * d;    
}
summed(12, 12, 12, 12);
console.log(`The Product of the values is ${summed(12,12,12,12)}`);        // 20736


// The above can also be rewritten in this form, and give the same product result
function summed1 (a, b, c, d){
    console.log(a * b * c * d);
}
summed1(12,12,12,12);               // 20736


// EXAMPLE 3
// To return true if arguments entered are true, and
// return false if entered arguments are false based on statement

function trueFalse (a, b){
    return console.log(a == b);
}
trueFalse(12,12);             // True
trueFalse(12,13);           // False


// EXAMPLE 4
// Checking conditions, with adoption of if...else
function check(m, n){
    if (m == n){
        console.log(true);
    } else
    {
        console.log(false);
    }
}
check(12,13);           // false
check(12,12);           // true
check(2,12);            // false


// EXAMPLE 5
// Additional conditional checking with adoption of if...else methods

function runner (g, t){
    if (g == t){
        return console.log(g + t);   // adds the values if equal
    } else
    {
        return console.log(g * t);     // multiplies the values if not equal
    }
}
runner(12,12);              // 24, i.e., 12 + 12 since 1st condition  is met
runner(12,13);              // 156, i.e., 12*13 since since its 2nd condition that is met
runner(34,2);               // 68, i.e., 34*2 since its 2nd condition that is met


</code>
</pre>

ALL SUMMARIZED RESULTS

<pre>
<code>
/*

[ 12 ]
[ 12, 14 ]
[ 12, 14, 12 ]
The Product of the values is 20736
20736
true
false
false
true
false
24
156
68

*/
</code>
</pre>
