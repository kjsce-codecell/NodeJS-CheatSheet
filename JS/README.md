# JS CheatSheet
##Comments
###Single Line Comment
> //  

###Multi Line Comment
> /* */

##Variables
> var variable = 1;

##Operators
###Assignment operators

- x = y : `x = y`   
- x = x + y : `x += y`  
- x = x - y : `x -= y`  
- x = x * y : `x *= y ` 
- x = x / y : `x /= y`  

###Logical operators

- Equal value and type : `===`   
- Not equal value or not equal type : `!==`  
- Greater than or equal to : `>=`   
- Less than or equal to : `<=`   

####Ternary -- shorthand for a conditional : `?`     
 > condition ? 'do this if true': 'do this if false'

Example : 
> var canDrink = age > 21 ? 'Go drink!' : 'Sorry you're too young!'

- Returns true if both are true : `('comparision1' && 'comparison2')` 
- Returns true if at least one is true : ` ('comparison1' || 'comparison2')  `
- Returns opposite of boolean value : `!('comparison')`  

##Arrays

> var arrayName = ['add text', 23, true];
> var arrayName2 = [];


###Access array items

Item in the ith position of the array `arrayName[i]` 


###Add to array
Adds to end, back of the line
> arrayName2.push('what you want to add'); 

Adds the front, un is bad - the items are cutting everyone to get to the front
>arrayName2.unshift('new addition', 'another new additon');  

###Remove from array

Last item pops off
> arrayName2.pop();

First item is removed and all others shift up in line 
> arrayName2.shift(); 


###Splicing arrays

> arrayName[i].splice(j,k,x);
  
  where -
  
  - i is the array index (if you have an array inside an array),
  - j is the item index
  - k is the number of items to remove
  - x is items to add


###Rename item in an array

> arrayName[i] = 'new value'  

where i is the index of the item being replaced


##If Else

<pre>if (condition) {
  console.log('do this if true');
} else {
  console.log('do this if false');
}</pre>

##For loop

Starting value of i :  `i = 0 ` 
How many times loop will run : `i !==10` 
How to increment i after loop, adds 1 to i : `i++` 
 Will increment by the # specified : `i+=#`


<pre>for (var i = 0; i !== 10; i++ ) {
  console.log(i);
}</pre>
  
##While loop

<pre>while (condition) {
  console.log('do this');
}</pre>
 
 Will run until condition is false, could run zero times

##Do while loop

<pre>do {
  console.log('do something')
} while (condition);</pre>
 
 Will run at least once and continues to run until condition is false


##Objects

<pre>var objectName = {
  property1: "can be text",
  property2: ['or', 'an', 'array'],
  property3: true,
  property4: {
    subProperty1: "amanda",
    subProperty2: 10,
  }
}</pre>

Access items in an object (dot notation):
>console.log(objectName.property1);
>console.log(objectName.property2[2]);

Object starting with blank
>var newObject = new Object();

<pre>newObject.property1 = "can add text";
newObject.property2 = [1,2,3,4];
newObject.property3 = {
  subProperty1: 'new text',
  subProperty2: 10,
  subProperty3: [2,4,6]
}</pre>

> console.log(newObject);


##Functions

<pre>function functionName(property) {
  return property;
}</pre>


###Call a function
> functionName(enterProperty);


###Sorting from smallest to largest

<pre>arrayName.sort(function(a, b) {
  return a - b
});</pre>

Change to b - a for largest to smallest


###is NaN

<pre>function isNaN(testValue) {
  return Number.isNaN(Number(testValue));
}</pre>


##Random number generator

Generates number between 0 and 1, multiply to get whole numbers
>Math.random() 

Rounds down to nearest whole number
>Math.floor(number to round down);  

Round to two decimal places
>Math.round(NumberWithMoreDecimals * 100) / 100;
