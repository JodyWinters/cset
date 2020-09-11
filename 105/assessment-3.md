How do you feel about the pace of the program so far? Is it too slow? Too fast? Or just right?

If you were to ask me that question two weeks ago I would definitely have said the class was moving 
too slow.  Now, with the new concepts that are being introduced and the project, that I admit is a 
bit intimidating, I would say the class is moving at just the right pace. There is plenty of challanges
with the work but we are also reusing old concepts continually to help make them stick.


Why do you think functions are a useful tool to organize large programs?

It helps by making the code you are working on easier to read. Instead of having a large amount of code
all jumbled together, you can have a function that has less presence inside the blocks of code to make the
entirety of the program easier to read.

In class, we've been using the analogy of a zoo to explain scope. Describe the different types of scope using
this analogy and provide examples using real JavaScript code.
  Quick tip: Markdown formatting creates code blocks by using backticks, just like Slack.
  Surround code with a single backtick for inline code, like `this`.
  Or start a code block by surrounding multiple lines with three backticks, like this:
  ```
  
  ```
  
 The two main types of scope are global and local. When used in the analogy of a zoo the zookeeper is the global,
 while the many animals in their pens are the local. Each of the different animals are in their own pens and cannot
 interact with each other. The zookeeper on the otherhand is allowed to go to each and everyone of the animal pens.
 Here's and example using a loop that counts to four:
 ```
 Example A
 let x = 4;
  for(let count = 0; count =< x; count++) {
    console.log(count);
  }
 console.log(x);
 console.log(count);
 ```
 The output for running this code would look like this:
 // 0,1,2,3,4,4, Error: count is not defined
 In two different spots the variable "count" is output, yet one works as expected while the other gives an error. This is 
 because "count" was defined inside the local scope of the for loop, or in otherwords, inside its own animal pen. It can't be reached
 outside of its local scope so when called it gives the error message. Two ways you know if a binding is within a local scope is when
 it is defined inside of a function(lexical rule) and when it is defined inside of curly brackets {}(block rule). The variable "count"
 in the example above is and example of the block rule. The variable "total" from example B is an example of the lexical rule. 
 The variable "x" in example A however is used inside and out of the for loops local scope. Thats because "x" is acting as the zookeeper, "x" is allowed to 
 enter all the animal pens, or all of the local scopes. 
 ```
 Example B
 const add = function (x,y) {
  let total = x + y;
  return total;
  }
  ```
 
