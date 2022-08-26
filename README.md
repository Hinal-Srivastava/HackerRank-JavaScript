# HackerRank-JavaScript
## [Day 3: Try, Catch and Finally](https://www.hackerrank.com/challenges/js10-try-catch-and-finally/problem?isFullScreen=true)
Objective: In this challenge, we learn about strings and exceptions. Check out the attached tutorials for more details.
- Task: Complete the reverseString function; it has one parameter, . You must perform the following actions:
Try to reverse string  using the split, reverse, and join methods.
If an exception is thrown, catch it and print the contents of the exception's  on a new line.
Print  on a new line. If no exception was thrown, then this should be the reversed string; if an exception was thrown, this should be the original string.
- Input Format: Locked stub code in the editor reads variable  from stdin and passes it to the function.
- Output Format:
You must write two print statements using console.log():
Print the contents of a caught exception's  on a new line. If no exception was thrown, this line should not be printed.
Print  on a new line. If no exception was thrown, then this should be the reversed string; if an exception was thrown, this should be the original string.
#### Solution
`function reverseString(s) {
  try{
      let temp = s.split("").reverse().join("");
      console.log(temp);
  } 
  catch(ex){
      console.log("s.split is not a function");
      console.log(s);
  }`
## [Day 3: Throw](https://www.hackerrank.com/challenges/js10-throw/problem?isFullScreen=true)
In this challenge, we practice using throw and catch statements to work with custom error messages.
### Solution
`return a>0?"YES":a==0?"Zero Error":"Negative Error";`
## [Day 4: Classes](https://www.hackerrank.com/challenges/js10-class/problem?isFullScreen=true)
- Objective: In this challenge, we practice using JavaScript classes. Check the attached tutorial for more details.
- Task: Create a Polygon class that has the following properties:
A constructor that takes an array of integer values describing the lengths of the polygon's sides.
A perimeter() method that returns the polygon's perimeter.
Locked code in the editor tests the Polygon constructor and the perimeter method.
- Note: The perimeter method must be lowercase and spelled correctly.
### Solution
`class Polygon{
    constructor(arr){
        this.arr=arr;
    }
    perimeter(){
        var sum=0;
        for(let i=0; i<this.arr.length; i++){
            sum+=this.arr[i];
        }
        return sum; 
    }
}`

