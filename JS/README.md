# JS CheatSheet
## Comments
### Single Line Comment
`// This is a single line comment `

### Multi Line Comment
    /* This is a
       multi-line comment */

## Variables
`var variable = 1;`

## Operators
### Assignment operators

- `x = y`   
- `x += y`, equivalent to `x = x + y`
- `x -= y`, equivalent to `x = x - y`
- `x *= y`, equivalent to `x = x * y`
- `x /= y`, equivalent to `x = x / y`

### Logical operators

- Equal value and type: `===`   
- Not equal value or not equal type: `!==`  
- Greater than or equal to: `>=`   
- Less than or equal to: `<=`   

#### Ternary -- shorthand for a conditional : `?`     
 `condition ? 'do this if true': 'do this if false'`

Example: `var canDrink = age > 21 ? 'Go drink!' : 'Sorry you're too young!';`

- Returns true if both are true : `('comparision1' && 'comparison2')` 
- Returns true if at least one is true : ` ('comparison1' || 'comparison2')  `
- Returns opposite of boolean value : `!('comparison')`  

## Arrays

    var arrayName = ['add text', 23, true];
    var arrayName2 = [];


### Access array items

Item in the ith position of the array `arrayName[i]` 


### Add to array
Adds to end, back of the line: `arrayName2.push('what you want to add');` 

Adds the front, un is bad - the items are cutting everyone to get to the front

`arrayName2.unshift('new addition', 'another new additon');` 

### Remove from array

Last item pops off: `arrayName2.pop();`

First item is removed and all others shift up in line: `arrayName2.shift();`


### Splicing arrays

`arrayName[i].splice(j,k,x);`
  
  where -
  
  - `i` is the array index (if you have an array inside an array),
  - `j` is the item index
  - `k` is the number of items to remove
  - `x` is items to add


### Rename item in an array

`arrayName[i] = 'new value'`  

where `i` is the index of the item being replaced


## If-Else

    if (condition) {
      console.log('do this if true');
    } else {
      console.log('do this if false');
    }

## For loop

    for (var i = 0; i !== 10; i++ ) {
      console.log(i);
    }

 - Starting value of `i`:  `i = 0 ` 
 - How many times loop will run: `i !== 10` 
 - How to increment `i` after loop, adds 1 to `i`: `i++` 
 - Will increment by the # specified: `i += #`
  
## While loop

    while (condition) {
      console.log('do this');
    }

Will run until condition is false, could run zero times.

## Do-while loop

    do {
      console.log('do something')
    } while (condition);
 
 Will run at least once and continues to run until condition is false.


## Objects

    var objectName = {
      property1: "can be text",
      property2: ['or', 'an', 'array'],
      property3: true,
      property4: {
        subProperty1: "amanda",
        subProperty2: 10,
      }
    }

Access items in an object (dot notation):

    console.log(objectName.property1);
    console.log(objectName.property2[2]);

Object starting with blank

    var newObject = new Object();

    newObject.property1 = "can add text";
    newObject.property2 = [1,2,3,4];
    newObject.property3 = {
      subProperty1: 'new text',
      subProperty2: 10,
      subProperty3: [2,4,6]
    }

    console.log(newObject);


## Functions

    function functionName(property) {
      return property;
    }


### Call a function

`functionName(enterProperty);`


### Sorting from smallest to largest

    arrayName.sort(function(a, b) {
      return a - b
    });

Change to `b - a` for largest to smallest


### is NaN

    function isNaN(testValue) {
      return Number.isNaN(Number(testValue));
    }


## Random number generator

Generates number between 0 and 1, multiply to get whole numbers

`Math.random()`

Rounds down to nearest whole number

`Math.floor(floating_point_number_to_round_down);`

Round to two decimal places

`Math.round(NumberWithMoreDecimals * 100) / 100;`
