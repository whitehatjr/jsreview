# JavaScript Review

## Numbers and Strings
 
 JavaScript can understand different kinds of data like numbers and string. 
Try entering a number in the console:
```
> 2
```
Similarly, try entering any string in the console:

```
> "Hello world"
``` 
Remember, strings are enclosed by quotes

## Variables

You can store data inside containers (variables) using "var"

Can you store your name inside a variable?
```
> var name = "Rajeev"
```
Now call the variable to see what is inside it.
```
> name
```
You can see your name printed in the console.

Strings are objects in JavaScript and they have some properties and functions defined. You can try some of them.

```
name.length
```
```
name.toUpperCase()
```
You will be able to see your name in all caps.

You can also store any number inside the variable.

```
> var num = 5
```

You can also convert a string into a number:

```
parseInt("123")
```

## Arithmetic Operations
You can use arithmetic operations on numbers using arithmetic operators (+ , - , /, *, %).

_Note: Remind students that modulo(%) sign gives you a remainder between two numbers._

You can try doing different arithmetic operations on the console.  
```
2+3
```
```
2-3
```
```
5*7
```
```
36/12
```
```
12%5
```
Try using '+' arithmetic operator on strings and guess what will happen:

```
"Hi" + "Friend"
```
Strings get joined together when you add them.

Now try using any other arithmetic operation on strings like division (/)

```
"a" / "b"
```
You will get **NaN** which means not a number.

Now try dividing any number with 0:

```
1/0
```
You will get **Infinity** as an answer.

## Booleans
There is another boolean data type in JavaScript which can hold only **true** or **false**
```
var bool = true
```

Comparison operators (>,<,>=,<=,===, !=) also evaluate to a boolean value.
Try to use any of the comparison operators with numbers on the console
```
2===3
```
This will print false on the console.

## Other data types
There are two other kinds of data in JavaScript - **null** and **undefined**

**null** is used when you want a variable to hold nothing.
**undefined** is the value inside a variable when you have forgot to assign anything to it.

```
var test
```
Now try to see what is inside 'test'
```
test
```
## Conditional programming
We can use if-else block to create conditional programming. 
Try writing a simple if-else statement:
```
if(3>2){
	console.log("Happy")
}
else{
	console.log("Not Happy")
}
```
If the condition evaluates to **true**, if block is executed; otherwise else block is executed.

Switch statement is another way in which we can do conditional programming.

```
var name = "My name";

switch(name) {  
case  "My name":  
console.log("Condition 1");  
break;  
case  "my Name":  
console.log("Condition 2");  
break;  
default:  
console.log("None of the conditions are true");
}
```

## Loops
Computers do not like to repeat themselves. We use loops to perform repeated function. There are two kinds of loops - **for** and **while** loop.

Write a simple **for** loop:

```
for(var i=0; i<=5; ++){
	console.log(i)
}
```

Write a simple **while** loop:

```
var i =0
while (i<=5){
	console.log(i)
	i=i+1
}
```

## Arrays
Arrays are a type of data structure where you can use single variable to store a list of items.

Write an array which stores a list of items.

```
var friends = ["friend1","friend2","friend3"]
```
You can access any item in the list using indexes.
_Note: Counting starts from 0 on computers_
```
friends[0]
```

You can also loop over all the items using **for-each** loop

```
for(var index in friends){
	console.log(friends[index])
}
```

Arrays are also objects in javaScript. They have some properties and function defined.
For example, you can get the length of the array using length property:

```
friends.length
```

You can also push new elements into the array using push():

```
friends.push("friend4")
```
You can see the elements in the friends array now:
```
friends
```

You can also pop out the last element from the array using pop():

```
friends.pop();
```

## Functions
Javascript has certain in-built functions which you can use.
You can also write your own functions.
Write a function to calculate the circumference of a circle. It should take radius as the argument.

```
function circumference(radius){
	var circumference = 2 * 3.14 * radius
	return circumference
}
```
Now you can use the circumference functions to calculate the radius of any circle.

```
circumference(5)
```

## Objects
We used classes to design blue prints of objects in javascript and then used **new** to create new object using the class.

Internally JavaScript creates a new object using *new Object()*
```
var paddle = new Object();
```
You can assign new properties and functions to test object.

Ask the student to assign a new property and function to a test object

```
paddle.length = 60
```

```
paddle.showLength = function(){
	console.log(paddle.length);
}
```

Call paddle.showLength() to see the length of the paddle.

```
paddle.showLength()
```

Call paddle object to see what's stored inside the paddle.

```
paddle
```
