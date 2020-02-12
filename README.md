# Answers for Lab 04
Q1.) Is the keyword "fixes" the only way to auto-close an issue from a PR (pull request). Are there other keywords that can accomplish the same thing?

A.) No! There are other keywords that are able to auto-close an issue from a PR. The other keywords are:

* close, closes, closed

* fix, fixes, fixed

* resolve, resolves, resolved


Q2.) Do you have to create a new PR EVERYTIME you want to close an issue,or is it possible to close multiple issues within a single PR? If so, how?

A.) No! You don't have to create a new PR EVERYTIME we want to close an issue. We can close multiple issues with a single PR by using the following syntax in the title:

* _resolves #10, resolves #11, resolves #18_

We need to separate each resolved issue with a comma within a single pull request in order to close multiple issues!

Q3.) Provide an example of using map that is different from the one I have done. Your example must use map both as a named function declaration and with an anonymous function. 

    /*Anonymous Function*/
    let arr = ["hello", "hi", "shalom", "hola"];  
    let newArr = arr.map(function (greeting) { 
       /* Map creates a new array by going through each array element in array "arr". 
       This anonymous function then returns each element with "world" appended at the end*/
	    return greeting + " world";
    })
    
    /*Named Function Declaration*/
    let numArr = [0, 4, 9, 16];
    
    // This named function declaration will return a new array with the square root of each numArr value
    function squareNum(arr){
      let squareArr = arr.map(Math.sqrt);
      return squareArr;
    }
    
    squareNum(numArr);
    
The transformation function is sometimes called a _callback function_ because **it passes a function as an argument**, as seen in the first example up above. The passed function is then applied for each element in an array. 
