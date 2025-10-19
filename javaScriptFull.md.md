 # javaScript
## javaScript Basics

- HTML creates the content
- CSS changes the apearance
- JS makes it interactive

- to create pop up
```js
alert('hello');
```
or
```js
alert('Good Job');
```
- javaScript provides mathematics calculation on console

```js
2+2
```
or
```js
10-3
```
- to remove everything on page and show sms / to modify the webpage

```js
document.body.innerHTML = 'hello';
```
- syntax = rules that we have to follow in a programming language.

- homework 1
```js
alert('Good morning!');
alert('Abdur Rouf Robin');
10+5
20-5
2+2-5
document.body.innerHTML = 'Good morning!';
document.body.innerHTML ='Robin';
10+8+20
100-20-50+200
document.body.innerHTML = '';

```

## Numbers

- order of operations
  - BODMAS
  - we can't calculate % . we have to calculate manually 1% = 1/10
      - (..)
      - *, /
      - +, -
- 0.1 + 0.2 = 0.3000000000000004 // computer can't floating number properly
- to avoid this problem ---->> transform into integer (for dollar transform into cents) (to taka          transform into poisa)
- to round
    ```js
    Math.round(2.2)
    Math.round(2.3)
    Math.round((2095 + 799)*0.1)/100
    ```
### How to use Google
- mdn web docs javaScript
- chatgpt
- devdocs
-  homework of chapter 2
```js
//2a
1*10+3*8+1*5
//2b
(1*10+3*8+1*5)*3
//2c
(1850+750*2)/100
//2d
Math.round((1850+7.50*2)*0.1)/100
//2e
Math.round((1850+7.50*2)*0.2)/100
//2f
(2095+799+1899)/100
//2g
(2095+799+1899+499)/100
//2h
Math.round((2095+799+1899+499)*0.1)/100
//2i
(2095+799+1899+499)/100 + Math.round((2095+799+1899+499)*0.1)/100
//2j
Math.floor(2.8)
//2k
Math.ceil(2.2)
//2l
(25*9)/5+32
//2m
(86-32)*5/9
//2n
((-5)*9/5)+32
```
## String
- string = text
- syntax = '...'
- we can add string like
```js
'some' + 'text' //sometext
'some' + 'more' + 'text' //somemoretext
// this is called concatenation = combine strings together
```
- we can see the type of any value
```js
typeof 3 //number
typeof 'hello' //string
```
- we can add number and string

```js
'hello' + 3 //hello3
//this is called type coercion or automatic type conversion
```
- practice
```js
'$' + 20.95 +7.99 //shows error
'$20.95' + 7.99 //shows error
'$' + ((2095+799)/100) //right
'$Items (' + (1 + 1) + '): $'+ (2095+799)/100
alert('$Items (' + (1 + 1) + '): $'+ (2095+799)/100);
```
- 3 ways to create string
  - single quote = '....' // better
  - double quotes = "...." // when we want to use single quote in string like I'm
     - escape character = \\'
     - escape character = \\"
     - escape character = \\n //new line character
  - backtick = template string =\`....\`
    - interpolation = insert value directly into string
    ```js
    `Items(${1+1}): $${(2095+799)/100}`
    ```
    - multi-line strings = strings are in multiple line
   
    ```js
    `some
    text`
    //'some\ntext'
    ```
 - exercise of chapter 3
```js
//3a
'My name is:'
//3b
'Robin'
//3c
'My name is:' + 'Robin'
//3d
'Total cost: $' + (5+3)
//3e
`Total cost: $${5 + 3}`
//3f
alert(`Total cost: $${5 + 3}`)
//3g
'Total cost: $' + (599+295)/100
//3h
`Total cost: $${(599+295)/100}`
//3i
alert(`Total cost: $${(599+295)/100}`)
//3j
`Total cost:$${(599+295)/100}
Thank you, come again!`
//3k
`Items (${2+2}):                 $${(2*2095 + 2*799)/100}`
//3l
`Shipping & handling:        $${(499+499)/100}`
//3m
`Total before tax:       $${(2*2095 + 2*799)/100 + (499+499)/100}`
//3n
`Estimated tax(10%):                   $${Math.round(((2*2095 + 2*799) + (499+499))*0.1)/100}`
//3o
`Order total:   $${(2*2095 + 2*799)/100 + (499+499)/100+Math.round(((2*2095 + 2*799) + (499+499))*0.1)/100}`
```
## Html Css Javascript together
- install a code editor ( VS Code )
- HTML = Hyper Text MarkUp Language
- nesting = element inside an element
- multiple spaces are combined into 1 space
- newline also count as converted space
- webpage is a single page of website
- CSS = Cascading Style Sheets
- Attribute changes the behavior of an element
- onclick = whenever we click the element
- first script tag then onclick js
- // used in js for single line comments
- /*  */ used in js for multiline comments
- \<!-- --> used in HTML for comments
- /**/ used in css
- exercise of chapter 4
```js
//4a
<button>Click</button>
//4b
<button>Simon</button>
<button>chocolate</button>
//4c
<p>Hello, world!</p>
//4d
<p>Hello, world!</p>
<p>Today I went to the grocery store to buy some eggs and vegetables.</p>
//4e
<style>
  .add-to-cart-button {
    background-color: yellow;
  }

  .buy-now-button {
    background-color: orange;
  }
</style>

<button class="add-to-cart-button">Add to cart</button>
<button class="buy-now-button">Buy now</button>
//4f
<!DOCTYPE html>
<html>
  <head>
    <style>
      .add-to-cart-button {
        background-color: yellow;
      }
    
      .buy-now-button {
        background-color: orange;
      }
    </style>
  </head>
  <body>
    <button class="add-to-cart-button">Add to cart</button>
    <button class="buy-now-button">Buy now</button>
  </body>
</html>
//4g
<!DOCTYPE html>
<html>
  <head>
    <title>Buttons</title>
    <style>
      .add-to-cart-button {
        background-color: yellow;
      }
    
      .buy-now-button {
        background-color: orange;
      }
    </style>
  </head>
  <body>
    <button class="add-to-cart-button">Add to cart</button>
    <button class="buy-now-button">Buy now</button>
  </body>
</html>
//4h
<!DOCTYPE html>
<html>
  <head>
    <title>Buttons</title>
    <style>
      .add-to-cart-button {
        background-color: yellow;
      }
    
      .buy-now-button {
        background-color: orange;
      }
    </style>
  </head>
  <body>
    <button class="add-to-cart-button">Add to cart</button>
    <button class="buy-now-button">Buy now</button>

    <script>
      console.log('Welcome!');
    </script>
  </body>
</html>
//4i
<!DOCTYPE html>
<html>
  <head>
    <style>
      .add-to-cart-button {
        background-color: yellow;
      }
    
      .buy-now-button {
        background-color: orange;
      }
    </style>
  </head>
  <body>
    <p>Adults Plain Cotton T-shirt</p>
    <p>Price: $7.99</p>
    <button class="add-to-cart-button">Add to cart</button>
    <button class="buy-now-button">Buy now</button>
  </body>
</html>
//4j
<!DOCTYPE html>
<html>
  <head>
    <style>
      .add-to-cart-button {
        background-color: yellow;
      }
    
      .buy-now-button {
        background-color: orange;
      }
    </style>
  </head>
  <body>
    <p>Adults Plain Cotton T-shirt</p>
    <p>Price: $7.99</p>

    <!-- I added some extra spaces to make the code
    easier to read. -->
    <button class="add-to-cart-button" onclick="
      alert('Added');
    ">Add to cart</button>

    <button class="buy-now-button" onclick="
      console.log('Loading...');
      alert('Purchased');
    ">Buy now</button>
  </body>
</html>
```
## chapter 5 variables
- variable = a container
```js
let variable1 = 3
let calculation = 2 + 2
let result = calculation + 2
let message = 'hello!'
variable1 = variable1 + 1
```
- variable name restriction
   - can't use special word
   - can't use special characters except $ and _
   - can't start with a number
   - ; means end of an instruction
   - semicolon insertion = insert semicolon in last automatically
   - assiging a value to a variable and reassigning a value to the variable
   - cart project
 ```html
  <!DOCTYPE html>
\<html>
  \<head>
    \<title>Cart Quantity</title>
  \</head>
  <body>
    \<button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      cartQuantity++;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Add to Cart</button>

    <button onclick="
      cartQuantity += 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+2</button>

    <button onclick="
      cartQuantity = cartQuantity + 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+3</button>

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
   </body>
   </html>
```
- all these line do the same thing

```js
cartQuantity = cartQuantity + 1
cartQuantity +=1
cantQuantity++
```
- other shortcuts
```
+=
-=
*=
/=
++
--
```
- naming variable
```js
camelCase = cartQuantity // special naming convention for js
PascalCase = CartQuantity
kabab-case = cart-quantity
snake_case = cart_quantity
```
- naming should not too short too long
- naming should be meningful and smart and mediumsize
- 3 ways to create variable in js
```js
let a; // better
var b; // good
const c; // best
```
- we can use 'typeof' with variable
- exercise of chapter 5
```html
//5a
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const name = 'Simon';
    </script>
  </body>
</html>
//5b
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const name = 'Simon';
      console.log(`My name is: ${name}`);
    </script>
  </body>
</html>
//5c
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const cost = 5 + 2 * 3 + 9;
    </script>
  </body>
</html>
//5d
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const cost = 5 + 2 * 3 + 9;
      console.log(`Cost of food: $${cost}`);
    </script>
  </body>
</html>
//5e
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const cost = 5 + 2 * 3 + 9;
      console.log(`Cost of food: $${cost}`);

      const tax = cost * 0.1;
    </script>
  </body>
</html>
//5f
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const cost = 5 + 2 * 3 + 9;
      console.log(`Cost of food: $${cost}`);

      const tax = cost * 0.1;
      console.log(`Tax (10%): $${tax}`);
    </script>
  </body>
</html>
//5g
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const cost = 5 + 2 * 3 + 9;
      console.log(`Cost of food: $${cost}`);

      const tax = cost * 0.1;
      console.log(`Tax (10%): $${tax}`);

      const totalCost = cost + tax;
      console.log(`Total cost: $${totalCost}`);
    </script>
  </body>
</html>
//5h
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      cartQuantity++;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Add to Cart</button>

    <button onclick="
      cartQuantity += 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+2</button>

    <button onclick="
      cartQuantity = cartQuantity + 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+3</button>

    <!-- vvv This code is new. vvv -->
    <button onclick="
      cartQuantity += 4;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+4</button>

    <button onclick="
      cartQuantity += 5;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+5</button>
    <!-- ^^^ This code is new. ^^^ -->

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
  </body>
</html>
//5i
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      cartQuantity++;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Add to Cart</button>

    <button onclick="
      cartQuantity += 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+2</button>

    <button onclick="
      cartQuantity = cartQuantity + 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+3</button>

    <button onclick="
      cartQuantity += 4;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+4</button>

    <button onclick="
      cartQuantity += 5;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+5</button>

    <!-- vvv This code is new. vvv -->
    <button onclick="
      cartQuantity = cartQuantity - 1;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Remove from cart</button>
    <!-- ^^^ This code is new. ^^^ -->

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
  </body>
</html>
//5j
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      cartQuantity++;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Add to Cart</button>

    <button onclick="
      cartQuantity += 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+2</button>

    <button onclick="
      cartQuantity = cartQuantity + 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+3</button>

    <button onclick="
      cartQuantity += 4;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+4</button>

    <button onclick="
      cartQuantity += 5;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+5</button>

    <button onclick="
      cartQuantity = cartQuantity - 1;
      console.log(`Cart quantity: ${cartQuantity}`);
      ">Remove from cart</button>

    <!-- vvv This code is new. vvv -->
    <button onclick="
      cartQuantity = cartQuantity - 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">-2</button>

    <button onclick="
      cartQuantity = cartQuantity - 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">-3</button>
    <!-- ^^^ This code is new. ^^^ -->

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
  </body>
</html>
//5k
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      cartQuantity++;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Add to Cart</button>

    <button onclick="
      cartQuantity += 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+2</button>

    <button onclick="
      cartQuantity = cartQuantity + 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+3</button>

    <button onclick="
      cartQuantity += 4;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+4</button>

    <button onclick="
      cartQuantity += 5;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">+5</button>

    <!-- vvv This code was changed. vvv -->
    <button onclick="
      cartQuantity--;
      console.log(`Cart quantity: ${cartQuantity}`);
      ">Remove from cart</button>

    <button onclick="
      cartQuantity -= 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">-2</button>

    <button onclick="
      cartQuantity -= 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">-3</button>
    <!-- ^^^ This code was changed. ^^^ -->

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
  </body>
</html>
//5l
<!DOCTYPE html>
<html>
  <head></head>
  <body></body>
</html>
//5m
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button>1</button>
    <button>2</button>
    <button>3</button>
    <button>+</button>
    <button>=</button>
  </body>
</html>
//5n
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button>1</button>
    <button>2</button>
    <button>3</button>
    <button>+</button>
    <button>=</button>
    <script>
      let calculation = '';
    </script>
  </body>
</html>
//5o
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      calculation += '1';
      console.log(calculation);
    ">1</button>
    
    <button>2</button>
    <button>3</button>
    <button>+</button>
    <button>=</button>
    <script>
      let calculation = '';
    </script>
  </body>
</html>
//5p
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      calculation += '1';
      console.log(calculation);
    ">1</button>
    
    <button onclick="
      calculation += '2';
      console.log(calculation);
    ">2</button>

    <button onclick="
      calculation += '3';
      console.log(calculation);
    ">3</button>

    <button onclick="
      calculation += ' + ';
      console.log(calculation);
    ">+</button>

    <button>=</button>
    
    <script>
      let calculation = '';
    </script>
  </body>
</html>
//5q
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      calculation += '1';
      console.log(calculation);
    ">1</button>

    <button onclick="
      calculation += '2';
      console.log(calculation);
    ">2</button>

    <button onclick="
      calculation += '3';
      console.log(calculation);
    ">3</button>

    <button onclick="
      calculation += ' + ';
      console.log(calculation);
    ">+</button>

    <button onclick="
      // Note: eval() takes a string and runs it as code.
      // Avoid using eval() in real world projects since
      // it can potentially be given harmful code to run.
      // Only use eval() for learning purposes.
      calculation = eval(calculation);
      console.log(calculation);
    ">=</button>

    <script>
      let calculation = '';
    </script>
  </body>
</html>
//5r
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <p>
      <button onclick="
        calculation += '1';
        console.log(calculation);
      ">1</button>

      <button onclick="
        calculation += '2';
        console.log(calculation);
      ">2</button>

      <button onclick="
        calculation += '3';
        console.log(calculation);
      ">3</button>

      <button onclick="
        calculation += ' + ';
        console.log(calculation);
      ">+</button>
    </p>

    <p>
      <button onclick="
        calculation += '4';
        console.log(calculation);
      ">4</button>

      <button onclick="
        calculation += '5';
        console.log(calculation);
      ">5</button>

      <button onclick="
        calculation += '6';
        console.log(calculation);
      ">6</button>

      <button onclick="
        calculation += ' - ';
        console.log(calculation);
      ">-</button>
    </p>

    <p>
      <button onclick="
        calculation += '7';
        console.log(calculation);
      ">7</button>

      <button onclick="
        calculation += '8';
        console.log(calculation);
      ">8</button>

      <button onclick="
        calculation += '9';
        console.log(calculation);
      ">9</button>

      <button onclick="
        calculation += ' * ';
        console.log(calculation);
      ">*</button>
    </p>

    <p>
      <button onclick="
        calculation += '0';
        console.log(calculation);
      ">0</button>

      <button onclick="
        calculation += '.';
        console.log(calculation);
      ">.</button>

      <button onclick="
        // Note: eval() takes a string and runs it as code.
        // Avoid using eval() in real world projects since
        // it can potentially be given harmful code to run.
        // Only use eval() for learning purposes.
        calculation = eval(calculation);
        console.log(calculation);
      ">=</button>

      <button onclick="
        calculation += ' / ';
        console.log(calculation);
      ">/</button>
    </p>

    <p>
      <button onclick="
        calculation = '';
        console.log(calculation);
      ">Clear</button>
    </p>

    <script>
      let calculation = '';
    </script>
  </body>
</html>
```
- booleans and if statements
- there are only two boolean values - true  - false
- comaprision of numbers
- we don't surround this with quote like 'true'  or 'false'- if we did then it will become string
- true, false --> boolean
- 'true', 'false' --> string
- comparison operator --> >, <, >=, <=, ===, !==
- ( == ) and ( != ) compare only value
- ( === ) and ( !== ) compare both value and type
- in the order of operations comparison operators have the lower priority than math
  1. (...)
  2. \* /
  3. \+ -
  4. comparison operator
  5. logical operators
```js
console.log(3>5-5);
```       
- if statement
```js
if(boolean value or any command that results a boolean value){
command---->>
}
else{
command ----->
}
```
- if command line is one line then no need to use curly brackets
- we can add more branches between 'if' and 'else' named 'else if'
```js
if(age>=){
console.log('You can drive');
}
else if (age>=){
console.log('Almost there..!');
}
else if (age>=70){
console.log('You are overaged to drive');
}
else{
console.log(`You can't drive`);
}
```
- Math.random() generates a random number between 0 and 1 it generates '0<=number<1'
- logical operators = let us combine boolean values
```js
&&
||
!
```
- scope = scope means where a variable exists
- scope helps us to avoid naming conflicts
- when we reassign a variable we heave to set variable type to 'let'
- any variable we create inside the curly brackets will only exist inside the curly brackets
- 'var' doesn't really follow the rules of scope thats why we can't use 'var' in coding
- we can't redeclare block-scope variable but can reassign it even if ...................
- rock paper scissors
```js
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
  </head>
  <body>
    <p>Rock Paper Scissors</p>
    <button onclick="
      const randomNumber = Math.random();

      let computerMove = '';

      if (randomNumber >= 0 && randomNumber < 1 / 3) {
        computerMove = 'rock';
      } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
        computerMove = 'paper';
      } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
        computerMove = 'scissors';
      }

      let result = '';

      if (computerMove === 'rock') {
        result = 'Tie.';
      } else if (computerMove === 'paper') {
        result = 'You lose.';
      } else if (computerMove === 'scissors') {
        result = 'You win.';
      }

      alert(`You picked rock. Computer picked ${computerMove}. ${result}`);
    ">Rock</button>

    <button onclick="
       randomNumber = Math.random();

       computerMove = '';

      if (randomNumber >= 0 && randomNumber < 1 / 3) {
        computerMove = 'rock';
      } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
        computerMove = 'paper';
      } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
        computerMove = 'scissors';
      }

      result = '';

      if (computerMove === 'rock') {
        result = 'You win.';
      } else if (computerMove === 'paper') {
        result = 'Tie.';
      } else if (computerMove === 'scissors') {
        result = 'You lose.';
      }

      alert(`You picked paper. Computer picked ${computerMove}. ${result}`);
    ">Paper</button>

    <button onclick="
      randomNumber = Math.random();

      computerMove = '';

      if (randomNumber >= 0 && randomNumber < 1 / 3) {
        computerMove = 'rock';
      } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
        computerMove = 'paper';
      } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
        computerMove = 'scissors';
      }

      result = '';

      if (computerMove === 'rock') {
        result = 'You lose.';
      } else if (computerMove === 'paper') {
        result = 'You win.';
      } else if (computerMove === 'scissors') {
        result = 'Tie.';
      }

      alert(`You picked scissors. Computer picked ${computerMove}. ${result}`);
    ">Scissors</button>

    <script>
      
    </script>
  </body>
</html>

```
- strategy for javaScript
   - figure out what steps we need
   - convert these steps into code
## More details about boolean and if statements
- Truthy and Falsy Values
- Truthy Values = the value just behave like 'true'
- Falsy Values = the value just behave like 'false'

- Falsy Values
  1. false
  2. 0
  3. NaN
  4. undefined
  5. null
  6. '' //empty value
```js
console.log(!0) //true
```
- NaN = Not a Number
```js
console.log('text'/5) //NaN
```
- undefined = doesn't have a value
```js
let variable1;
console.log(variable1);
```
- for 'const' we must assign a value or undefined
```js
const variable1 = undefined;
```
- null //later
```js
//later
```
- shortcuts for if-statements
   - Ternary operators '?:'
   - Guard oprators '&&'
   - Default operators '||'
- we can set variable for ternary operators
```js
const result = 0 ? 'truthy' : 'falsy';
console.log(result);
```
- short circuit evaluation for && operators and || operators
```
false && value2 // && operator stops early and doesn't even need to runn the code right side value2
```
or
```js
false && console.log('hello')
true && console.log('hello')
const message = 5>3 && 'hello'
const message = 0 && 'hello'
```
- Default operators
```js
const currency = 'EUR' || 'USD';
const currency = undefined || 'USD';
console.log(currency)
```
- homework chapter 6
- 6a
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const hour = 9;

      if (hour >= 6 && hour <= 12) {
        console.log('Good morning!');
      } else if (hour >= 13 && hour <= 17) {
        console.log('Good afternoon!');
      } else {
        console.log('Good night!');
      }
    </script>
  </body>
</html>
```
- 6b
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      // Try changing this variable to
      // display different messages.
      const hour = 15;

      if (hour >= 6 && hour <= 12) {
        console.log('Good morning!');
      } else if (hour >= 13 && hour <= 17) {
        console.log('Good afternoon!');
      } else {
        console.log('Good night!');
      }
    </script>
  </body>
</html>
```
- 6c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const hour = 9;
      const name = 'Simon';

      if (hour >= 6 && hour <= 12) {
        console.log(`Good morning ${name}!`);
      } else if (hour >= 13 && hour <= 17) {
        console.log(`Good afternoon ${name}!`);
      } else {
        console.log(`Good night ${name}!`);
      }
    </script>
  </body>
</html>
```
- 6d
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const age = 5;

      if (age <= 6 || age >= 65) {
        console.log('Discount');
      } else {
        console.log('No discount');
      }
    </script>
  </body>
</html>
```
- 6e
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const age = 5;
      const isHoliday = true;

      // && has a higher priority than || so for
      // this to work correctly, we need to add
      // brackets () around the || check to make
      // sure that it gets done first.
      if ((age <= 6 || age >= 65) && !isHoliday) {
        console.log('Discount');
      } else {
        console.log('No discount');
      }
    </script>
  </body>
</html>
```
- 6f
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const randomNumber = Math.random();
    </script>
  </body>
</html>
```
- 6g
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const randomNumber = Math.random();

      if (randomNumber < 0.5) {
        console.log('heads');
      } else {
        console.log('tails');
      }
    </script>
  </body>
</html>
```
- 6h
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const randomNumber = Math.random();
      let result;

      if (randomNumber < 0.5) {
        result = 'heads';
      } else {
        result = 'tails';
      }
    </script>
  </body>
</html>
```
- 6i
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const randomNumber = Math.random();
      let result;

      if (randomNumber < 0.5) {
        result = 'heads';
      } else {
        result = 'tails';
      }

      const guess = 'heads';

      if (guess === result) {
        console.log('You win!');
      } else {
        console.log('You lose!');
      }
    </script>
  </body>
</html>
```
- 6j
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const randomNumber = Math.random();
      const result = randomNumber < 0.5 ? 'heads' : 'tails';

      const guess = 'heads';
      console.log(guess === result ? 'You win!' : 'You lose!');
    </script>
  </body>
</html>
```
- 6k
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      if (cartQuantity + 1 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity++;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">Add to Cart</button>

    <button onclick="
      if (cartQuantity + 2 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity += 2;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+2</button>

    <button onclick="
      if (cartQuantity + 3 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity = cartQuantity + 3;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+3</button>

    <button onclick="
      if (cartQuantity + 4 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity += 4;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+4</button>

    <button onclick="
      if (cartQuantity + 5 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity += 5;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+5</button>

    <button onclick="
      cartQuantity--;
      console.log(`Cart quantity: ${cartQuantity}`);
      ">Remove from cart</button>

    <button onclick="
      cartQuantity -= 2;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">-2</button>

    <button onclick="
      cartQuantity -= 3;
      console.log(`Cart quantity: ${cartQuantity}`);
    ">-3</button>

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
  </body>
</html>
```
- 6l
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      if (cartQuantity + 1 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity++;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">Add to Cart</button>

    <button onclick="
      if (cartQuantity + 2 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity += 2;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+2</button>

    <button onclick="
      if (cartQuantity + 3 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity = cartQuantity + 3;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+3</button>

    <button onclick="
      if (cartQuantity + 4 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity += 4;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+4</button>

    <button onclick="
      if (cartQuantity + 5 > 10) {
        alert('The cart is full');
      } else {
        cartQuantity += 5;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">+5</button>

    <!-- vvv This code was changed. vvv -->
    <button onclick="
      if (cartQuantity - 1 < 0) {
        alert('Not enough items in the cart');
      } else {
        cartQuantity--;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">Remove from cart</button>

    <button onclick="
      if (cartQuantity - 2 < 0) {
        alert('Not enough items in the cart');
      } else {
        cartQuantity -= 2;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">-2</button>

    <button onclick="
      if (cartQuantity - 3 < 0) {
        alert('Not enough items in the cart');
      } else {
        cartQuantity -= 3;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    ">-3</button>
    <!-- ^^^ This code was changed. ^^^ -->

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;
    </script>
  </body>
</html>
```
## chapter 7 functions

- function lets us reuse code
- make our code easier to update
- following the code line by line = tracing the code

- function basics
- best practice to use camel case
- in function name we use verb or action to start like pickComputerMove(){}
- any variable created between curly bracket only exist between curly brackets like const computerMove
- solution 1. use global variable
           2. use return statement
- we prefer using return statement rather than using global variable because ' scope help us to prevent naming conflicts'
- keep thing inside a scope if we can --> best practice
- return statemnet = let us get a value out of a function also the value of the function when it is     called but we need to save the return value into another variable then console.log it
- we can return 1. a value 2. a variable 3. a calculation 4. a function also
- return; = returns the value 'undefined'
- when we use return it ends the function immediately
- we need to  call the function in where we want to use funtion
- return = gets a value out of a function
- parameter = puts a value into a function
- parameter works same as a variable
- parameter name = camelCase
- argument = when we passing a value while calling the function. it is an actual value
- parameter = it acts as a placeholder for the data
- if we don't give any argument to parameter it will be undefined automatically
- and any caluculation with undefined number results NaN = Not a Number
- to fix this we set a default value in parameter initializing 
- inside a function we can call another function

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Functions</title>
  </head>
  <body>
    <script>
      /*
      function function1() {
        console.log('hello');
        console.log(2 + 2);
      }

      function1();
      function1();
      */

      function calculateTax(cost, taxPercent = 0.1) {
        console.log(cost * taxPercent);
      }

      calculateTax(2000, 0.2);
      calculateTax(5000);
    </script>
  </body>
</html>

```
- rock paper scissors game
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
  </head>
  <body>
    <p>Rock Paper Scissors</p>
    <button onclick="
      playGame('rock');
    ">Rock</button>

    <button onclick="
      playGame('paper');
    ">Paper</button>

    <button onclick="
      playGame('scissors');
    ">Scissors</button>

    <script>
      function playGame(playerMove) {
        const computerMove = pickComputerMove();

        let result = '';

        if (playerMove === 'scissors') {
          if (computerMove === 'rock') {
            result = 'You lose.';
          } else if (computerMove === 'paper') {
            result = 'You win.';
          } else if (computerMove === 'scissors') {
            result = 'Tie.';
          }

        } else if (playerMove === 'paper') {
          if (computerMove === 'rock') {
            result = 'You win.';
          } else if (computerMove === 'paper') {
            result = 'Tie.';
          } else if (computerMove === 'scissors') {
            result = 'You lose.';
          }
          
        } else if (playerMove === 'rock') {
          if (computerMove === 'rock') {
            result = 'Tie.';
          } else if (computerMove === 'paper') {
            result = 'You lose.';
          } else if (computerMove === 'scissors') {
            result = 'You win.';
          }
        }

        alert(`You picked ${playerMove}. Computer picked ${computerMove}. ${result}`);
      }

      function pickComputerMove() {
        const randomNumber = Math.random();

        let computerMove = '';

        if (randomNumber >= 0 && randomNumber < 1 / 3) {
          computerMove = 'rock';
        } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
          computerMove = 'paper';
        } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
          computerMove = 'scissors';
        }

        return computerMove;
      }
    </script>
  </body>
</html>

```
- exercise
- 7a
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function greet() {
        console.log('Hello!');
      }
      greet();
      greet();
    </script>
  </body>
</html>
```
- 7b
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function greet(name) {
        console.log(`Hello ${name}!`);
      }
      greet('Simon');
      greet('Alice');
    </script>
  </body>
</html>
```
- 7c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function greet(name) {
        if (!name) {
          console.log('Hi there!');
        } else {
          console.log(`Hello ${name}!`);
        }
      }
      greet('Simon');
      greet('Alice');
      greet();
    </script>
  </body>
</html>
```
- 7d
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function convertToFahrenheit(celsius) {
        return (celsius * 9 / 5) + 32;
      }
      console.log(convertToFahrenheit(25));
    </script>
  </body>
</html>
```
- 7e
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function convertToCelsius(fahrenheit) {
        return (fahrenheit - 32) * 5 / 9;
      }
      console.log(convertToCelsius(86));
    </script>
  </body>
</html>
```
- 7f
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function convertToFahrenheit(celsius) {
        return (celsius * 9 / 5) + 32;
      }

      function convertToCelsius(fahrenheit) {
        return (fahrenheit - 32) * 5 / 9;
      }

      function convertTemperature(degrees, unit) {
        if (unit === 'C') {
          const result = convertToFahrenheit(degrees);
          return `${result}F`;
        } else if (unit === 'F') {
          const result = convertToCelsius(degrees);
          return `${result}C`;
        }
      }

      console.log(convertTemperature(25, 'C'));
      console.log(convertTemperature(86, 'F'));
    </script>
  </body>
</html>
```
- 7g
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function convertLength(length, from, to) {
        if (from === 'km' && to === 'miles') {
          return `${length / 1.6} miles`;
        } else if (from === 'miles' && to === 'km') {
          return `${length * 1.6} km`;

        // You can also do if (from === 'km' && to === 'km) { ... }
        // if (from === to) is a trick you can use to save some code.
        } else if (from === to) {
          return `${length} ${to}`;
        }
      }

      console.log(convertLength(50, 'miles', 'km'));
      console.log(convertLength(32, 'km', 'miles'));
      console.log(convertLength(50, 'km', 'km'));
    </script>
  </body>
</html>

```
- 7h
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function convertLength(length, from, to) {
        if (from === 'km' && to === 'miles') {
          return `${length / 1.6} ${to}`;

        } else if (from === 'km' && to === 'ft') {
          return `${length * 3281} ${to}`;
          
        } else if (from === 'miles' && to === 'km') {
          return `${length * 1.6} ${to}`;

        } else if (from === 'miles' && to === 'ft') {
          return `${length * 5280} ${to}`;

        } else if (from === 'ft' && to === 'km') {
          return `${length / 3281} ${to}`;

        } else if (from === 'ft' && to === 'miles') {
          return `${length / 5280} ${to}`;

        // You can also do if (from === 'km' && to === 'km) { ... }
        // if (from === to) is a trick you can use to save some code.
        } else if (from === to) {
          return `${length} ${to}`;
        }
      }

      console.log(convertLength(50, 'miles', 'km'));
      console.log(convertLength(32, 'km', 'miles'));
      console.log(convertLength(50, 'km', 'km'));

      console.log(convertLength(5, 'miles', 'km'));
      console.log(convertLength(5, 'miles', 'ft'));
      console.log(convertLength(5, 'km', 'ft'));
    </script>
  </body>
</html>

```
- 7i
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function convertLength(length, from, to) {
        // I like to put invalid checks at the top since it's a bit
        // easier to see. Also, if something is invalid, we can skip
        // the rest of the function.
        if (from !== 'km' && from !== 'miles' && from !== 'ft') {
          return `Invalid unit: ${from}`;
        } else if (to !== 'km' && to !== 'miles' && to !== 'ft') {
          return `Invalid unit: ${to}`;
        }
        
        if (from === 'km' && to === 'miles') {
          return `${length / 1.6} ${to}`;

        } else if (from === 'km' && to === 'ft') {
          return `${length * 3281} ${to}`;
          
        } else if (from === 'miles' && to === 'km') {
          return `${length * 1.6} ${to}`;

        } else if (from === 'miles' && to === 'ft') {
          return `${length * 5280} ${to}`;

        } else if (from === 'ft' && to === 'km') {
          return `${length / 3281} ${to}`;

        } else if (from === 'ft' && to === 'miles') {
          return `${length / 5280} ${to}`;

        // You can also do if (from === 'km' && to === 'km) { ... }
        // if (from === to) is a trick you can use to save some code.
        } else if (from === to) {
          return `${length} ${to}`;
        }
      }

      console.log(convertLength(50, 'miles', 'km'));
      console.log(convertLength(32, 'km', 'miles'));
      console.log(convertLength(50, 'km', 'km'));

      console.log(convertLength(5, 'miles', 'km'));
      console.log(convertLength(5, 'miles', 'ft'));
      console.log(convertLength(5, 'km', 'ft'));

      console.log(convertLength(5, 'lbs', 'lbs'));
    </script>
  </body>
</html>

```
- 7j
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <p>
      <button onclick="
        updateCalculation('1');
      ">1</button>

      <button onclick="
        updateCalculation('2');
      ">2</button>

      <button onclick="
        updateCalculation('3');
      ">3</button>

      <button onclick="
        updateCalculation(' + ');
      ">+</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('4');
      ">4</button>

      <button onclick="
        updateCalculation('5');
      ">5</button>

      <button onclick="
        updateCalculation('6');
      ">6</button>

      <button onclick="
        updateCalculation(' - ');
      ">-</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('7');
      ">7</button>

      <button onclick="
        updateCalculation('8');
      ">8</button>

      <button onclick="
        updateCalculation('9');
      ">9</button>

      <button onclick="
        updateCalculation(' * ');
      ">*</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('0');
      ">0</button>

      <button onclick="
        updateCalculation('.');
      ">.</button>

      <button onclick="
        // Note: eval() takes a string and runs it as code.
        // Avoid using eval() in real world projects since
        // it can potentially be given harmful code to run.
        // Only use eval() for learning purposes.
        calculation = eval(calculation);
        console.log(calculation);
      ">=</button>

      <button onclick="
        updateCalculation(' / ');
      ">/</button>
    </p>

    <p>
      <button onclick="
        calculation = '';
        console.log(calculation);
      ">Clear</button>
    </p>

    <script>
      let calculation = '';

      function updateCalculation(value) {
        calculation += value;
        console.log(calculation);
      }
    </script>
  </body>
</html>

```
- 7k
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      updateCartQuantity(1);
    ">Add to Cart</button>

    <button onclick="
      updateCartQuantity(2);
    ">+2</button>

    <button onclick="
      updateCartQuantity(3);
    ">+3</button>

    <button onclick="
      updateCartQuantity(4);
    ">+4</button>

    <button onclick="
      updateCartQuantity(5);
    ">+5</button>

    <button onclick="
      updateCartQuantity(-1);
    ">Remove from cart</button>

    <button onclick="
      updateCartQuantity(-2);
    ">-2</button>

    <button onclick="
      updateCartQuantity(-3);
    ">-3</button>

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;

      function updateCartQuantity(change) {
        if (cartQuantity + change > 10) {
          alert('The cart is full');

        } else if (cartQuantity + change < 0) {
          alert('Not enough items in the cart');

        } else {
          cartQuantity += change;
          console.log(`Cart quantity: ${cartQuantity}`);
        }
      }
    </script>
  </body>
</html>

```
- 7l
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Show Quantity</button>

    <button onclick="
      updateCartQuantity(1);
    ">Add to Cart</button>

    <button onclick="
      updateCartQuantity(2);
    ">+2</button>

    <button onclick="
      updateCartQuantity(3);
    ">+3</button>

    <button onclick="
      updateCartQuantity(4);
    ">+4</button>

    <button onclick="
      updateCartQuantity(5);
    ">+5</button>

    <button onclick="
      updateCartQuantity(-1);
    ">Remove from cart</button>

    <button onclick="
      updateCartQuantity(-2);
    ">-2</button>

    <button onclick="
      updateCartQuantity(-3);
    ">-3</button>

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');
      console.log(`Cart quantity: ${cartQuantity}`);
    ">Reset Cart</button>

    <script>
      let cartQuantity = 0;

      function updateCartQuantity(change) {
        if (cartQuantity + change > 10) {
          alert('The cart is full');
          return;
        }

        if (cartQuantity + change < 0) {
          alert('Not enough items in the cart');
          return;
        }

        cartQuantity += change;
        console.log(`Cart quantity: ${cartQuantity}`);
      }
    </script>
  </body>
</html>

```
## Chapter 8 Object

- Objects = Object groups multiple values together
- Here in product object 'name' and 'price' are callded 'properties'
- Here in product object 'socks' and '1090' are called 'values'
- name: 'socks'  this is called property value pair
- product.name -->> this is called dot notation
- product.notExists  --->> result in 'undefined'
- product.newProperty = true   -->> to add new value to the object
- to delete a value -->> delete product.name
- object make our code more organized
- we can reduct creating variables by object
- bracket notation lets us use properties that don't work with dot notation
- if the proporty name is like 'delivery-time' then we have to use bracket notation
- we can use bracket notation to show variable or calculation
-  'product2[vairable1]' or product2['delivery' + 'time']
-  we use dot notation bt default bt in case we use bracket notaiton
-  inside an object we can save any type of value like numbers, string, boolean, another objects(nested objects), functions,
-  method = function inside object
-  built in object = console, math, JSON, localStorage
-  JSON = javaScript Object Notation
-  JSON = similar to javaScript Object bt has less features
-  JSON = all property and values (without numbers) must use double quotation
-  JSON doesn't support single quotation, function,
-  JSON syntax is more universal than javaScript Object
-  we use JSON to send and receive data between two devices or applications and we use JSON to store data
- JSON object help us to convert from JavaScript Objet to JSON
- localStorage is use to save values more permanently
- they only exist only current page
- if we reload the page or exit the page variables are reset back to initial value
- variables are temporary
- local storage doesn't get deleted when we refresh the page
```js
localStorage.setItem('message', 'hello' ) /* method to save a value inside local storage where message = name and hello = value 
localStorage only support strings */
// so we need to convert our object into string by
JSON.stringify(score) // here score is an object name and this convert score object into JSON-string
```
- to get that value out of local Storage

```js
localStorage.getItem('message');
console.log(localStorage.getItem('message'))
// we get the result in JSON-string so we need to convert into object
JSON.parse(localStorage.getItem('score'));
const score = JSON.parse(localStorage.getItem('score'));
//if score is change later then we have to change const into let
let score = JSON.parse(localStorage.getItem('score'));
```
- we need to remove the value from local Storage when we reset
```js
localStorage.removeItem('score')
```
- when something doesn't exist in localStorage it is going to provide a value 'null'
- it we try to use any property of null it will give an error
- to solve the problem we can set value with if statement when it will be 'null'
```js
if(score === null){
  score = {
  wins: 0,
  loses= 0,
  ties= 0
  };
  // but in this case set the variable to let not const // 'let score'  not 'const score'
}
```
- we can use short cuts

```js
if(score === null){
  score = {
  wins: 0,
  loses= 0,
  ties= 0
  };
  // but in this case set the variable to let not const // 'let score'  not 'const score'
}
```
- to
```js
if(!score){
  score = {
  wins: 0,
  loses= 0,
  ties= 0
  };
  // but in this case set the variable to let not const // 'let score'  not 'const score'
}
```
- score = null
```js
!score => true
score === null   => true
```
- or if score = {wins:0, loses:0, ties:0}
```js
!score => false
score === null   => false
```

- we can use default operator
```js
let score = JSON.parse(localStorage.getItem('score'));
if(!score){
  score = {
  wins: 0,
  loses= 0,
  ties= 0
  };
}
```
- to
```js
let score = JSON.parse(localStorage.getItem('score')) || {
  wins: 0,
  loses= 0,
  ties= 0
  };
```
- 'null' is one of the falsy value in js it similar to value undefined
- null vs undefined
- null = intentionally want something to be empty
```js
function func(parameter = 'defalult'){
console.log(parameter);
func();  // default
func(undefined);  // default
func(null);     // null
}
```
- Auto-Boxing
- objects have propeties and methods
```js
{
  name: 'shirt', // property
  prict: 799, // property
  fun: function dis(){  // method
  console.log('method');
  }
}
```
- other values also have properties and methods
```js
console.log('hello'.length); // 5  // we use property in string
console.log('hello'.toUpperCase());  // we use method in string
```
- javaScript has a special feature Auto Boxing = javaScript automatically wrap the string into          special-object like a box.
- Autoboxing also works with other type of values like 'number' and 'boolean'
```js
3.0.toString();
true.toString();
```
- Autoboxing doesn't work with 'null' and 'undefined'
```js
null.property // gives error
undefined.method() // gives error
```
- objects are references
- actual values ate stored in somewhere in memory but object1 only has the pointer to the location
- copy by reference = object2 will copy object1's referece
```js
const object1 = {
  message: 'hello'
  // const object1 = references
};
  const object2 = object1; // in here we copy the object1's reference into object2 we don't copy the    object actually
  object1.message = 'Good job';
  console.log(object1);
  console.log(object2);
  // const prevents us to change the reference in the variable but doesn't prevent us to reach  the     references and change the value of the object's property  
```
- eventhough we use const in object we change the property value and the object
- we can't compare objects directly
```js
const object3 = {
   message: 'Good job'
};
console.log(object3 === object1); // false -- different reference
console.log(object2 === object1); // true -- same referemce
console.log(object3.message === object1. message) //
```
- shortcuts for object
```js
const object4 = {
  message: 'Good job!',
  price: 799
};
const message = object4.message; // variable name and property name are same
const {message, price} = object4; // destructing = easier way to take properties out of an object
console.log(message);
console.log(price)
```
- shorthand property
```js
const object4 = {
  message: 'Good job!',
  price: 799
};
/* const object5 = {
  message: message
};
*/
or
const object5 = {
  message
};
console.log(object5)
```
- shorthand method
```js
const object5 = {
  method: function function1() {
    console.log('nothing');
  }
};
console.log(object5);
object5.method();
```
- or
```js
  const object5 = {
    method() {
      console.log('nothing');
  } 
};
console.log(object5);
object5.method();
```

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Objects</title>
  </head>
  <body>
    <script>
      /*
      const product = {
        name: 'socks',
        price: 1090
      };
      console.log(product);
      console.log(typeof product);
      console.log(product.name);
      console.log(product.price);

      product.name = 'cotton socks';
      console.log(product);

      product.newProperty = true;
      console.log(product);

      delete product.newProperty;
      console.log(product);
      */

      /*
      const product2 = {
        name: 'shirt',
        // ['delivery-time']: '1 day' -->> if only have a string inside the brackets then we can skip brackets
        'delivery-time': '1 day',
        rating: {
          stars: 4.5,
          count: 87
        },
        fun: function function1() {
          console.log('function inside object');
        }
      };
      console.log(product2);
      console.log(product2.name);// dot notation
      console.log(product2['name']); // bracket notation
      console.log(product2['delivery-time']);
      
      console.log(product2.rating);
      console.log(product2.rating.count);

      product2.fun(); // this will run the function

      console.log(typeof console); // object
      console.log(typeof console.log); // function

      JSON.stringify(product2)
      console.log(JSON.stringify(product2));
      console.log(typeof JSON.stringify(product2)); // string

      const jsonString = JSON.stringify(product2);
      JSON.parse(jsonString) // to convert from JSON to JavaScript Object 
      console.log(JSON.parse(jsonString));
      */

      console.log('hello'.length);
      console.log('hello'.toUpperCase());

      const object1 = {
        message: 'hello',
        price: 799
      };
      const object2 = object1;

      object1.message = 'Good job!';
      console.log(object1);
      console.log(object2);

      const object3 = {
        message: 'Good job!',
        price: 799
      };
      console.log(object1 === object3);

      // const message = object1.message;
      const { message, price: cost } = object1;
      console.log(message);
      console.log(cost);

      const object4 = {
        // message: message,
        message,
        // method: function function1() {

        // },
        // method: function() {

        // },
        method() {

        }
      };
    </script>
  </body>
</html>

```
- rock paper scissors game

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
  </head>
  <body>
    <p>Rock Paper Scissors</p>
    <button onclick="
      playGame('rock');
    ">Rock</button>

    <button onclick="
      playGame('paper');
    ">Paper</button>

    <button onclick="
      playGame('scissors');
    ">Scissors</button>

    <button onclick="
      score.wins = 0;
      score.losses = 0;
      score.ties = 0;
      localStorage.removeItem('score');
    ">Reset Score</button>

    <script>


      /* const score = {
            wins: 0,
            loses: 0,
            ties: 0
          }; */

      let score = JSON.parse(localStorage.getItem('score')) || {
        wins: 0,
        losses: 0,
        ties: 0
      };

      /*
      if (!score) {
        score = {
          wins: 0,
          losses: 0,
          ties: 0
        };
      }
      */

      function playGame(playerMove) {
        const computerMove = pickComputerMove();

        let result = '';

        if (playerMove === 'scissors') {
          if (computerMove === 'rock') {
            result = 'You lose.';
          } else if (computerMove === 'paper') {
            result = 'You win.';
          } else if (computerMove === 'scissors') {
            result = 'Tie.';
          }

        } else if (playerMove === 'paper') {
          if (computerMove === 'rock') {
            result = 'You win.';
          } else if (computerMove === 'paper') {
            result = 'Tie.';
          } else if (computerMove === 'scissors') {
            result = 'You lose.';
          }
          
        } else if (playerMove === 'rock') {
          if (computerMove === 'rock') {
            result = 'Tie.';
          } else if (computerMove === 'paper') {
            result = 'You lose.';
          } else if (computerMove === 'scissors') {
            result = 'You win.';
          }
        }

        if (result === 'You win.') {
          score.wins += 1;
        } else if (result === 'You lose.') {
          score.losses += 1;
        } else if (result === 'Tie.') {
          score.ties += 1;
        }

        localStorage.setItem('score', JSON.stringify(score));

        alert(`You picked ${playerMove}. Computer picked ${computerMove}. ${result}
Wins: ${score.wins}, Losses: ${score.losses}, Ties: ${score.ties}`);
      }

      function pickComputerMove() {
        const randomNumber = Math.random();

        let computerMove = '';

        if (randomNumber >= 0 && randomNumber < 1 / 3) {
          computerMove = 'rock';
        } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
          computerMove = 'paper';
        } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
          computerMove = 'scissors';
        }

        return computerMove;
      }
    </script>
  </body>
</html>

```
- 8a
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const product = {
        name: 'basketball',
        price: 2095
      };
      console.log(product);
    </script>
  </body>
</html>
```
- 8b
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const product = {
        name: 'basketball',
        price: 2095
      };
      console.log(product);

      product.price += 500;
      console.log(product);
    </script>
  </body>
</html>
```
- 8c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const product = {
        name: 'basketball',
        price: 2095
      };
      console.log(product);

      product.price += 500;
      console.log(product);

      product['delivery-time'] = '3 days';
      console.log(product);
    </script>
  </body>
</html>
```
- 8d
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function comparePrice(product1, product2) {
        if (product1.price < product2.price) {
          return product1;
        } else {
          return product2;
        }
      }

      const product1 = {
        name: 'basketball',
        price: 2095
      };

      const product2 = {
        name: 'socks',
        price: 1090
      };

      console.log(comparePrice(product1, product2));
    </script>
  </body>
</html>
```
- 8e
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function isSameProduct(product1, product2) {
        if (
          product1.name === product2.name &&
          product1.price === product2.price
        ) {
          return true;
        } else {
          return false;
        }
      }

      // Here is an alternative solution that uses less code.
      function isSameProduct(product1, product2) {
        return (
          product1.name === product2.name &&
          product1.price === product2.price
        );
      }

      const product1 = {
        name: 'basketball',
        price: 2095
      };

      const product2 = {
        name: 'socks',
        price: 1090
      };

      const product3 = {
        name: 'basketball',
        price: 2095
      };

      console.log(isSameProduct(product1, product2));
      console.log(isSameProduct(product1, product3));
    </script>
  </body>
</html>
```
- 8f
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      console.log('Good Morning'.toLowerCase());
      console.log('TESTING'.toLowerCase());
    </script>
  </body>
</html>
```
- 8g
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      console.log('hello'.repeat(2));
      console.log('test'.repeat(3));
    </script>
  </body>
</html>
```
- 8h
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <!-- Code changes are at the bottom. -->
    <p>
      <button onclick="
        updateCalculation('1');
      ">1</button>

      <button onclick="
        updateCalculation('2');
      ">2</button>

      <button onclick="
        updateCalculation('3');
      ">3</button>

      <button onclick="
        updateCalculation(' + ');
      ">+</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('4');
      ">4</button>

      <button onclick="
        updateCalculation('5');
      ">5</button>

      <button onclick="
        updateCalculation('6');
      ">6</button>

      <button onclick="
        updateCalculation(' - ');
      ">-</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('7');
      ">7</button>

      <button onclick="
        updateCalculation('8');
      ">8</button>

      <button onclick="
        updateCalculation('9');
      ">9</button>

      <button onclick="
        updateCalculation(' * ');
      ">*</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('0');
      ">0</button>

      <button onclick="
        updateCalculation('.');
      ">.</button>

      <button onclick="
        // Note: eval() takes a string and runs it as code.
        // Avoid using eval() in real world projects since
        // it can potentially be given harmful code to run.
        // Only use eval() for learning purposes.
        calculation = eval(calculation);
        console.log(calculation);

        // Remember to save the calculation here.
        localStorage.setItem('calculation', calculation);
      ">=</button>

      <button onclick="
        updateCalculation(' / ');
      ">/</button>
    </p>

    <p>
      <button onclick="
        calculation = '';
        console.log(calculation);

        // Remember to save the calculation here.
        localStorage.setItem('calculation', calculation);
      ">Clear</button>
    </p>

    <script>
      let calculation = localStorage.getItem('calculation') || '';

      function updateCalculation(value) {
        calculation += value;
        console.log(calculation);
        localStorage.setItem('calculation', calculation);
      }

      // Optional: you can also create a function in order
      // to reuse this code.
      function saveCalculation() {
        localStorage.setItem('calculation', calculation);
      }
    </script>
  </body>
</html>

```
- 8i
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      playGame('heads');
    ">heads</button>

    <button onclick="
      playGame('tails');
    ">tails</button>

    <script>
      function playGame(guess) {
        const randomNumber = Math.random();
        const result = randomNumber < 0.5 ? 'heads' : 'tails';

        console.log(guess === result ? 'You win!' : 'You lose!');
      }
    </script>
  </body>
</html>
```
- 8j
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      playGame('heads');
    ">heads</button>

    <button onclick="
      playGame('tails');
    ">tails</button>

    <script>
      let score = {
        wins: 0,
        losses: 0
      };

      function playGame(guess) {
        const randomNumber = Math.random();
        const result = randomNumber < 0.5 ? 'heads' : 'tails';

        console.log(guess === result ? 'You win!' : 'You lose!');

        if (guess === result) {
          score.wins++;
        } else {
          score.losses++;
        }
        console.log(score);
      }
    </script>
  </body>
</html>
```
- 8k
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      playGame('heads');
    ">heads</button>

    <button onclick="
      playGame('tails');
    ">tails</button>

    <script>
      // We can use const here since score is a reference
      // so we can modify it even if it uses const.
      const score = JSON.parse(localStorage.getItem('score')) || {
        wins: 0,
        losses: 0
      };

      function playGame(guess) {
        const randomNumber = Math.random();
        const result = randomNumber < 0.5 ? 'heads' : 'tails';

        console.log(guess === result ? 'You win!' : 'You lose!');

        if (guess === result) {
          score.wins++;
        } else {
          score.losses++;
        }
        console.log(score);

        localStorage.setItem('score', JSON.stringify(score));
      }
    </script>
  </body>
</html>
```

- DOM = Document Object Model
- another built in object is - 'document' object
- document object and webpage are linked together
- document object represents or models the webpage
- document object has properties and methods
- DOM combines HTML an javaScript together and it gives javaScript control the webpage
- if a HTML element is inside javaScript then the HTML element is converted into JS Object
- with DOM javaScript has full control of the webpage
- method = a function saved inside an object
- document.body = let us get the body element of html
- document.querySelector() = let us get any element from the page and put in inside javaScript as        javaScript Object
- document.querySelector('body') = document.body // same
- Every HTML element has a proprty called 'innerHTML'. that let us control the HTML inside the element
- document.querySelector() only gets the first element of html
- any class usning for CSS can also be used for javaScript
- HTML element inside javaScript is an object. object are values we can set object inside a varible
- we generally set the element variable ending with (--Element or --Elem)
- DOM combines JS and HTML together. it gives JS full control of the webpage
- innerHTML property counts extra spaces around text to solve this we need to use innerText
- innerText don't count extra spaces
- clicks, keydown => events
- onclick, onkeydown => event listeners = they check for events and run js
- eventlisteners
  - onclick          = click
  - onkeydown        = key press
  - onscroll         = scrolling
  - onmouseenter     = hovering mouse
  - onmouseleave    = stop hovering mouse
- if a string only contains a number and we ( - , * , / ) then the string will be converted into         number automatically = type coercion --> not recommneded
- window object is a built in object
- document object represents the webpage
- window object represents the browser
- document object is inside the window object
- console object is inside the window object
- alert function is inside the window object
- javaScript will automatically add window object in front of those object or function
- DOM
```html
<!DOCTYPE html>
<html>
  <head>
    <title>DOM</title>
  </head>
  <body>
    <button>hello</button>
    <button class="js-button">Second button</button>

    <script>
      // documnet.body.innerHTML = 'hello'; // this code removes everything on the page with 'hello'
      // here document --> object then body --> property of document and also an object
      innerHTML = property of body
      // document.title = 'Good job!'; // change the title of the page
      document.querySelector('anyElementName, .anyClassName, #anyIdName') /* get the first element           class or id */
      
      document.querySelector('button')    
      console.log(document.querySelector('button'))
      console.log(document.querySelector('button').innerHTML);
      document.querySelector('button')
        .innerHTML = 'Changed';

      
      document.querySelector('.js-button');
      console.log(document.querySelector('.js-button'));
      const buttonElement = document.querySelector('.js-button');
      console.log(buttonElement);
      
      /*
      console.log(document.title); // to console the title of webpage
      document.title = 'Changed'; // to change the title of webpage

      console.log(document.body); // to console all the code including body element
      console.log(typeof document.body); // object // HTML elemet inside JS = object

      console.log(document.body.innerHTML); // it gives all the html inside the body element without         body element
      document.body.innerHTML = 'changed'; // change innet html with text
      // change inner html with new html code
      document.body.innerHTML = '<button>Good job!</button>'; // change the inner HTML of body element
      */
      
      /*
      document.body.innerHTML = 'hello';
      document.title = 'Good job!';
      */
    </script>
  </body>
</html>
```
- DOM Project
```html
<!DOCTYPE html>
<html>
  <head>
    <title>DOM Projects</title>
  </head>
  <body>
    <p>YouTube Subscribe Button</p>
    <button onclick="
      subscribe();
    " class="js-subscribe-button">
      Subscribe
    </button>

    <p>Amazon Shipping Calculator</p>
    // <input>    this is called a void element
    // placeholder is an attribute
    <input placeholder="Cost of order" class="js-cost-input" onkeydown="
      handleCostKeydown(event);
    ">
    <button onclick="
      calculateTotal();
    ">Calculate</button>
    <p class="js-total-cost"></p>

    <script>
      String(25) // it will convert the number into string
      console.log('25' - 5); //20
      console.log('25' + 5); // 255

      
      window.document
      window.console.log('window');
      window.alert

      function handleCostKeydown(event) {
        // console.log('typring')
        // console.log(event) //object
        // console.log(event.key)
        if (event.key === 'Enter') {
          calculateTotal();
        }
      }

      function calculateTotal() {
        const inputElement = document.querySelector('.js-cost-input');
        inputElement.value // this is how we get the value from an input element but as string
        let cost = Number(inputElement.value);
        // Number() is a built in funciton

        if (cost < 40) {
          cost = cost + 10;
        }

        document.querySelector('.js-total-cost')
          .innerHTML = `$${cost}`;
      }

      function subscribe() {
        const buttonElement = document.querySelector('.js-subscribe-button');

        if (buttonElement.innerText === 'Subscribe') {
          buttonElement.innerHTML = 'Subscribed';
        } else {
          buttonElement.innerHTML = 'Subscribe';
        }
      }
      
    </script>
  </body>
</html>

```
- rock paper scissors
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
  </head>
  <body>
    <p>Rock Paper Scissors</p>
    <button onclick="
      playGame('rock');
    ">Rock</button>

    <button onclick="
      playGame('paper');
    ">Paper</button>

    <button onclick="
      playGame('scissors');
    ">Scissors</button>

    <p class="js-result"></p>
    <p class="js-moves"></p>
    <p class="js-score"></p>

    <button onclick="
      score.wins = 0;
      score.losses = 0;
      score.ties = 0;
      localStorage.removeItem('score');
      updateScoreElement();
    ">Reset Score</button>

    <script>
      let score = JSON.parse(localStorage.getItem('score')) || {
        wins: 0,
        losses: 0,
        ties: 0
      };

      updateScoreElement();

      /*
      if (!score) {
        score = {
          wins: 0,
          losses: 0,
          ties: 0
        };
      }
      */

      function playGame(playerMove) {
        const computerMove = pickComputerMove();

        let result = '';

        if (playerMove === 'scissors') {
          if (computerMove === 'rock') {
            result = 'You lose.';
          } else if (computerMove === 'paper') {
            result = 'You win.';
          } else if (computerMove === 'scissors') {
            result = 'Tie.';
          }

        } else if (playerMove === 'paper') {
          if (computerMove === 'rock') {
            result = 'You win.';
          } else if (computerMove === 'paper') {
            result = 'Tie.';
          } else if (computerMove === 'scissors') {
            result = 'You lose.';
          }
          
        } else if (playerMove === 'rock') {
          if (computerMove === 'rock') {
            result = 'Tie.';
          } else if (computerMove === 'paper') {
            result = 'You lose.';
          } else if (computerMove === 'scissors') {
            result = 'You win.';
          }
        }

        if (result === 'You win.') {
          score.wins += 1;
        } else if (result === 'You lose.') {
          score.losses += 1;
        } else if (result === 'Tie.') {
          score.ties += 1;
        }

        localStorage.setItem('score', JSON.stringify(score));

        updateScoreElement();

        document.querySelector('.js-result').innerHTML = result;

        document.querySelector('.js-moves').innerHTML = `You ${playerMove} - ${computerMove} Computer`;
      }

      function updateScoreElement() {
        document.querySelector('.js-score')
          .innerHTML = `Wins: ${score.wins}, Losses: ${score.losses}, Ties: ${score.ties}`;
      }

      function pickComputerMove() {
        const randomNumber = Math.random();

        let computerMove = '';

        if (randomNumber >= 0 && randomNumber < 1 / 3) {
          computerMove = 'rock';
        } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
          computerMove = 'paper';
        } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
          computerMove = 'scissors';
        }

        return computerMove;
      }
    </script>
  </body>
</html>

```
- Exercise of chapter 9
- 9a
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button>9a</button>

    <script>
      console.log(document.querySelector('button'));
    </script>
  </body>
</html>
```
- 9b
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button>9a</button>
    
    <!-- Feel free to use a different class name. -->
    <button class="js-button">9b</button>

    <script>
      console.log(document.querySelector('button'));
      
      document.querySelector('.js-button')
        .innerHTML = '9b done!';
    </script>
  </body>
</html>
```
- 9c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button onclick="
      document.querySelector('.js-choice')
        .innerHTML = 'You chose: heads';
    ">heads</button>

    <button onclick="
      document.querySelector('.js-choice')
        .innerHTML = 'You chose: tails';
    ">tails</button>

    <p class="js-choice"></p>
  </body>
</html>
```
- 9d
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <input placeholder="Name" class="js-name-input">

    <button onclick="
      const inputElement = document.querySelector('.js-name-input');
      document.querySelector('.js-message')
        .innerHTML = `Your name is: ${inputElement.value}`;
    ">Submit</button>

    <p class="js-message"></p>
  </body>
</html>
```
- 9e
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <input placeholder="Name" class="js-name-input"
      onkeydown="
        if (event.key === 'Enter') {
          // Optional: instead of duplicating this code,
          // you could also put it in a function.
          const inputElement = document.querySelector('.js-name-input');
          document.querySelector('.js-message')
            .innerHTML = `Your name is: ${inputElement.value}`;
        }
      ">

    <button onclick="
      const inputElement = document.querySelector('.js-name-input');
      document.querySelector('.js-message')
        .innerHTML = `Your name is: ${inputElement.value}`;
    ">Submit</button>

    <p class="js-message"></p>
  </body>
</html>
```
- 9f
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <input placeholder="Name" class="js-name-input"
      onkeydown="
        if (event.key === 'Enter') {
          displayMessage();
        }
      ">

    <button onclick="
      displayMessage();
    ">Submit</button>

    <p class="js-message"></p>

    <script>
      function displayMessage() {
        const inputElement = document.querySelector('.js-name-input');
        document.querySelector('.js-message')
          .innerHTML = `Your name is: ${inputElement.value}`;
      }
    </script>
  </body>
</html>
```
- 9g
```html
<!DOCTYPE html>
<html>
  <head>
    <title>DOM Projects</title>
  </head>
  <body>
    <!-- Answer is at the bottom. -->
    <p>Amazon Shipping Calculator</p>
    <input placeholder="Cost of order" class="js-cost-input" onkeydown="
      handleCostKeydown(event);
    ">
    <button onclick="
      calculateTotal();
    ">Calculate</button>
    <p class="js-total-cost"></p>

    <script>
      function handleCostKeydown(event) {
        if (event.key === 'Enter') {
          calculateTotal();
        }
      }

      /*
       * Issue = the calculation is inaccurate.
       * Fix = calculate the number in cents and then
       *       convert back to dollars at the end.
       */
      function calculateTotal() {
        const inputElement = document.querySelector('.js-cost-input');

        // Convert the numbers to cents by * 100.
        let cost = Number(inputElement.value) * 100;

        if (cost < 4000) {
          cost = cost + 1000;
        }

        // Convert back to dollars at the end.
        document.querySelector('.js-total-cost')
          .innerHTML = `$${cost / 100}`;
      }
    </script>
  </body>
</html>
```
- 9h
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <input placeholder="Type something" class="js-input"
      onkeyup="
        const inputElement = document.querySelector('.js-input');
        document.querySelector('.js-message')
          .innerHTML = inputElement.value;
      ">

    <p class="js-message"></p>
  </body>
</html>
```
- 9i
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Cart Quantity</title>
  </head>
  <body>
    <button onclick="
      // Display the cart quantity on the page
      // instead of in the console.
      displayCartQuantity();
    ">Show Quantity</button>

    <button onclick="
      updateCartQuantity(1);
    ">Add to Cart</button>

    <button onclick="
      updateCartQuantity(2);
    ">+2</button>

    <button onclick="
      updateCartQuantity(3);
    ">+3</button>

    <button onclick="
      updateCartQuantity(4);
    ">+4</button>

    <button onclick="
      updateCartQuantity(5);
    ">+5</button>

    <button onclick="
      updateCartQuantity(-1);
    ">Remove from cart</button>

    <button onclick="
      updateCartQuantity(-2);
    ">-2</button>

    <button onclick="
      updateCartQuantity(-3);
    ">-3</button>

    <button onclick="
      cartQuantity = 0;
      console.log('Cart was reset.');

      // Display the cart quantity after updating.
      displayCartQuantity();
    ">Reset Cart</button>

    <!-- Create an element to display the cart quantity. -->
    <p class="js-cart-quantity"></p>

    <script>
      let cartQuantity = 0;

      // Display the cart quantity when the page loads.
      displayCartQuantity();

      function updateCartQuantity(change) {
        if (cartQuantity + change > 10) {
          alert('The cart is full');
          return;
        }

        if (cartQuantity + change < 0) {
          alert('Not enough items in the cart');
          return;
        }

        cartQuantity += change;

        // Display the cart quantity after updating.
        displayCartQuantity();
      }

      function displayCartQuantity() {
        document.querySelector('.js-cart-quantity')
          .innerHTML = `Cart quantity: ${cartQuantity}`;
      }
    </script>
  </body>
</html>

```
- 9j
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <!-- Create an element to display the calculation. -->
    <p class="js-calculation"></p>

    <p>
      <button onclick="
        updateCalculation('1');
      ">1</button>

      <button onclick="
        updateCalculation('2');
      ">2</button>

      <button onclick="
        updateCalculation('3');
      ">3</button>

      <button onclick="
        updateCalculation(' + ');
      ">+</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('4');
      ">4</button>

      <button onclick="
        updateCalculation('5');
      ">5</button>

      <button onclick="
        updateCalculation('6');
      ">6</button>

      <button onclick="
        updateCalculation(' - ');
      ">-</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('7');
      ">7</button>

      <button onclick="
        updateCalculation('8');
      ">8</button>

      <button onclick="
        updateCalculation('9');
      ">9</button>

      <button onclick="
        updateCalculation(' * ');
      ">*</button>
    </p>

    <p>
      <button onclick="
        updateCalculation('0');
      ">0</button>

      <button onclick="
        updateCalculation('.');
      ">.</button>

      <button onclick="
        // Note: eval() takes a string and runs it as code.
        // Avoid using eval() in real world projects since
        // it can potentially be given harmful code to run.
        // Only use eval() for learning purposes.
        calculation = eval(calculation);

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      ">=</button>

      <button onclick="
        updateCalculation(' / ');
      ">/</button>
    </p>

    <p>
      <button onclick="
        calculation = '';

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      ">Clear</button>
    </p>

    <script>
      let calculation = localStorage.getItem('calculation') || '';

      // Display the calculation when the page first loads.
      displayCalculation();

      function updateCalculation(value) {
        calculation += value;

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      }

      function displayCalculation() {
        document.querySelector('.js-calculation')
          .innerHTML = calculation;
      }
    </script>
  </body>
</html>

```

## chapter 10 DOM with CSS
- to change CSS with js
- '.classList' gives us control of the 'class' attribute
- 'classList' is an object
- to add a class
```js
.classList.add('classNameThatWeWantToAdd');
// don't need '.' before classname within single quote
```
- to remove a class
```js
.classList.remove('classNameThatWeWantToRemove');
// don't need '.' before classname within single quote
```
- DOM projects
```html
<!DOCTYPE html>
<html>
  <head>
    <title>DOM Projects</title>
    <style>
      body {
        font-family: Arial;
      }

      .subscribe-button {
        border: none;
        background-color: black;
        color: white;
        padding-top: 10px;
        padding-bottom: 10px;
        padding-left: 15px;
        padding-right: 15px;
        font-weight: bold;
        border-radius: 50px;
        cursor: pointer;
        margin-bottom: 30px;
      }

      .is-subscribed {
        background-color: rgb(240, 240, 240);
        color: black;
      }

      .cost-input {
        font-size: 15px;
        /*
        padding-top: 10px;
        padding-bottom: 10px;
        padding-left: 10px;
        padding-right: 10px;
        */
        padding: 10px;
      }

      .calculate-button {
        background-color: green;
        color: white;
        border: none;
        font-size: 15px;
        padding: 12px 15px;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <p>YouTube Subscribe Button</p>
    <button onclick="
      subscribe();
    " class="js-subscribe-button subscribe-button">
      Subscribe
    </button>

    <p>Amazon Shipping Calculator</p>
    <input placeholder="Cost of order" class="js-cost-input cost-input" onkeydown="
      handleCostKeydown(event);
    ">
    <button onclick="
      calculateTotal();
    " class="calculate-button">Calculate</button>
    <p class="js-total-cost"></p>

    <script>
      String(25)
      console.log('25' - 5);
      console.log('25' + 5);

      window.document
      window.console.log('window');
      window.alert

      function handleCostKeydown(event) {
        if (event.key === 'Enter') {
          calculateTotal();
        }
      }

      function calculateTotal() {
        const inputElement = document.querySelector('.js-cost-input');
        let cost = Number(inputElement.value);

        if (cost < 40) {
          cost = cost + 10;
        }

        document.querySelector('.js-total-cost')
          .innerHTML = `$${cost}`;
      }

      function subscribe() {
        const buttonElement = document.querySelector('.js-subscribe-button');

        if (buttonElement.innerText === 'Subscribe') {
          buttonElement.innerHTML = 'Subscribed';
          buttonElement.classList.add('is-subscribed');
        } else {
          buttonElement.innerHTML = 'Subscribe';
          buttonElement.classList.remove('is-subscribed');
        }
      }

    </script>
  </body>
</html>
```

- rock paper scissors
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
    <link rel="stylesheet" href="styles/10-rock-paper-scissors.css">
  </head>
  <body>
    <p class="title">Rock Paper Scissors</p>
    <button onclick="
      playGame('rock');
    " class="move-button">
      <img src="images/rock-emoji.png" class="move-icon">
    </button>

    <button onclick="
      playGame('paper');
    " class="move-button">
      <img src="images/paper-emoji.png" class="move-icon">
    </button>

    <button onclick="
      playGame('scissors');
    " class="move-button">
      <img src="images/scissors-emoji.png" class="move-icon">
    </button>

    <p class="js-result result"></p>
    <p class="js-moves"></p>
    <p class="js-score score"></p>

    <button onclick="
      score.wins = 0;
      score.losses = 0;
      score.ties = 0;
      localStorage.removeItem('score');
      updateScoreElement();
    " class="reset-score-button">Reset Score</button>

    <script src="scripts/10-rock-paper-scissors.js"></script>
  </body>
</html>

```
- CSS
```css
body {
  background-color: rgb(25, 25, 25);
  color: white;
  font-family: Arial;
}

.title {
  font-size: 30px;
  font-weight: bold;
}

.move-icon {
  height: 50px;
}

.move-button {
  background-color: transparent;
  border: 3px solid white;
  width: 120px;
  height: 120px;
  border-radius: 60px;
  margin-right: 10px;
  cursor: pointer;
}

.result {
  font-size: 25px;
  font-weight: bold;
  margin-top: 50px;
}

.score {
  margin-top: 60px;
}

.reset-score-button {
  background-color: white;
  border: none;
  font-size: 15px;
  padding: 8px 15px;
  cursor: pointer;
}
```
- javaScript
```js
let score = JSON.parse(localStorage.getItem('score')) || {
  wins: 0,
  losses: 0,
  ties: 0
};

updateScoreElement();

/*
if (!score) {
  score = {
    wins: 0,
    losses: 0,
    ties: 0
  };
}
*/

function playGame(playerMove) {
  const computerMove = pickComputerMove();

  let result = '';

  if (playerMove === 'scissors') {
    if (computerMove === 'rock') {
      result = 'You lose.';
    } else if (computerMove === 'paper') {
      result = 'You win.';
    } else if (computerMove === 'scissors') {
      result = 'Tie.';
    }

  } else if (playerMove === 'paper') {
    if (computerMove === 'rock') {
      result = 'You win.';
    } else if (computerMove === 'paper') {
      result = 'Tie.';
    } else if (computerMove === 'scissors') {
      result = 'You lose.';
    }
    
  } else if (playerMove === 'rock') {
    if (computerMove === 'rock') {
      result = 'Tie.';
    } else if (computerMove === 'paper') {
      result = 'You lose.';
    } else if (computerMove === 'scissors') {
      result = 'You win.';
    }
  }

  if (result === 'You win.') {
    score.wins += 1;
  } else if (result === 'You lose.') {
    score.losses += 1;
  } else if (result === 'Tie.') {
    score.ties += 1;
  }

  localStorage.setItem('score', JSON.stringify(score));

  updateScoreElement();

  document.querySelector('.js-result').innerHTML = result;

  document.querySelector('.js-moves').innerHTML = `You
<img src="images/${playerMove}-emoji.png" class="move-icon">
<img src="images/${computerMove}-emoji.png" class="move-icon">
Computer`;
}

function updateScoreElement() {
  document.querySelector('.js-score')
    .innerHTML = `Wins: ${score.wins}, Losses: ${score.losses}, Ties: ${score.ties}`;
}

function pickComputerMove() {
  const randomNumber = Math.random();

  let computerMove = '';

  if (randomNumber >= 0 && randomNumber < 1 / 3) {
    computerMove = 'rock';
  } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
    computerMove = 'paper';
  } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
    computerMove = 'scissors';
  }

  return computerMove;
}
```
- Exercise
- 10a
```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      .amazon-button {
        background-color: rgb(255, 216, 20);
        border: none;
        padding: 5px 40px;
        border-radius: 20px;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <button class="amazon-button">
      Add to Cart
    </button>
  </body>
</html>
```
- 10b
```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      .request-now-button {
        background-color: black;
        color: white;
        border: none;
        font-weight: bold;
        padding: 12px 20px;
        border-radius: 5px;
        cursor: pointer;
        margin-right: 20px;
      }

      .schedule-later-button {
        background-color: rgb(230, 230, 230);
        border: none;
        font-weight: bold;
        padding: 12px 20px;
        border-radius: 5px;
        cursor: pointer;
      }
    </style>
  </head>
  <body>
    <button class="request-now-button">
      Request now
    </button>
    <button class="schedule-later-button">
      Schedule for later
    </button>
  </body>
</html>
```
- 10c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button class="js-button">Test</button>

    <script>
      // I used the variable name 'button' because
      // it's shorter, but feel free to use whatever
      // variable name you want.
      const button = document.querySelector('.js-button');
      console.log(button.classList.contains('js-button'));
    </script>
  </body>
</html>
```
- 10d
```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      /* The word "toggle" means turn on/off. */
      .toggle-button {
        background-color: rgb(230, 230, 230);
        border: none;
        padding: 10px 15px;
        border-radius: 5px;
        margin-right: 10px;
        font-size: 15px;
        cursor: pointer;
      }

      .is-toggled {
        background-color: black;
        color: white;
      }
    </style>
  </head>
  <body>
    <button class="toggle-button js-button" onclick="
      const button = document.querySelector('.js-button');
      if (!button.classList.contains('is-toggled')) {
        button.classList.add('is-toggled');
      } else {
        button.classList.remove('is-toggled');
      }
    ">Gaming</button>
  </body>
</html>
```
- 10e
```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      /* The word "toggle" means turn on/off. */
      .toggle-button {
        background-color: rgb(230, 230, 230);
        border: none;
        padding: 10px 15px;
        border-radius: 5px;
        margin-right: 10px;
        font-size: 15px;
        cursor: pointer;
      }

      .is-toggled {
        background-color: black;
        color: white;
      }
    </style>
  </head>
  <body>
    <button class="toggle-button js-button" onclick="
      let button = document.querySelector('.js-button');
      if (!button.classList.contains('is-toggled')) {
        button.classList.add('is-toggled');
      } else {
        button.classList.remove('is-toggled');
      }
    ">Gaming</button>

    <button class="toggle-button js-button-2" onclick="
       button = document.querySelector('.js-button-2');
      if (!button.classList.contains('is-toggled')) {
        button.classList.add('is-toggled');
      } else {
        button.classList.remove('is-toggled');
      }
    ">Music</button>

    <button class="toggle-button js-button-3" onclick="
       button = document.querySelector('.js-button-3');
      if (!button.classList.contains('is-toggled')) {
        button.classList.add('is-toggled');
      } else {
        button.classList.remove('is-toggled');
      }
    ">Tech</button>
  </body>
</html>
```
- 10f html
```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="10f.css">
  </head>
  <body>
    <button class="toggle-button js-button" onclick="
      toggleButton('.js-button');
    ">Gaming</button>

    <button class="toggle-button js-button-2" onclick="
      toggleButton('.js-button-2');
    ">Music</button>

    <button class="toggle-button js-button-3" onclick="
      toggleButton('.js-button-3');
    ">Tech</button>

    <script src="10f.js"></script>
  </body>
</html>
```
- 10f CSS
```css
.toggle-button {
  background-color: rgb(230, 230, 230);
  border: none;
  padding: 10px 15px;
  border-radius: 5px;
  margin-right: 10px;
  font-size: 15px;
  cursor: pointer;
}

.is-toggled {
  background-color: black;
  color: white;
}
```
- 10f js
```js
// The word "toggle" means turn on/off.
function toggleButton(selector) {
  const button = document.querySelector(selector);
  if (!button.classList.contains('is-toggled')) {
    button.classList.add('is-toggled');
  } else {
    button.classList.remove('is-toggled');
  }
}
```
- 10g
```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="10g.css">
  </head>
  <body>
    <button class="toggle-button js-button" onclick="
      toggleButton('.js-button');
    ">Gaming</button>

    <button class="toggle-button js-button-2" onclick="
      toggleButton('.js-button-2');
    ">Music</button>

    <button class="toggle-button js-button-3" onclick="
      toggleButton('.js-button-3');
    ">Tech</button>

    <script src="10g.js"></script>
  </body>
</html>
```
- 10g CSS
```css
.toggle-button {
  background-color: rgb(230, 230, 230);
  border: none;
  padding: 10px 15px;
  border-radius: 5px;
  margin-right: 10px;
  font-size: 15px;
  cursor: pointer;
}

.is-toggled {
  background-color: black;
  color: white;
}
```
- 10g js
```js
// The word "toggle" means turn on/off.
function toggleButton(selector) {
  const button = document.querySelector(selector);
  if (!button.classList.contains('is-toggled')) {

    // Before turning this button ON, check if there's
    // already a button that's turned ON and turn it OFF.
    turnOffPreviousButton();

    button.classList.add('is-toggled');
  } else {
    button.classList.remove('is-toggled');
  }
}

function turnOffPreviousButton() {
  const previousButton = document.querySelector('.is-toggled');
  if (previousButton) {
    previousButton.classList.remove('is-toggled');
  }
}
```
- 10h
```html
<!DOCTYPE html>
<html>
  <head>
    <title>DOM Projects</title>
    <style>
      body {
        font-family: Arial;
      }

      .cost-input {
        font-size: 15px;
        padding: 10px;
      }

      .calculate-button {
        background-color: green;
        color: white;
        border: none;
        font-size: 15px;
        padding: 12px 15px;
        cursor: pointer;
      }

      /* Give the error message a red color. */
      .error-message {
        color: red;
      }
    </style>
  </head>
  <body>
    <p>Amazon Shipping Calculator</p>
    <input placeholder="Cost of order" class="js-cost-input cost-input" onkeydown="
      handleCostKeydown(event);
    ">
    <button onclick="
      calculateTotal();
    " class="calculate-button">Calculate</button>
    <p class="js-total-cost"></p>

    <!-- Create an element to display the error message. -->
    <p class="js-error-message error-message"></p>

    <script>
      function handleCostKeydown(event) {
        if (event.key === 'Enter') {
          calculateTotal();
        }
      }

      function calculateTotal() {
        const inputElement = document.querySelector('.js-cost-input');
        let cost = Number(inputElement.value);

        // First, reset all previous messages.
        document.querySelector('.js-total-cost')
          .innerHTML = '';
        document.querySelector('.js-error-message')
          .innerHTML = '';

        if (cost < 0) {
          document.querySelector('.js-error-message')
            .innerHTML = 'Error: cost cannot be less than $0';
          // If we display an error, we can use return to
          // end this function immediately. This is called
          // an "early return" and it makes the code cleaner
          // because it reduces nesting / indents.
          return;
        }

        if (cost < 40) {
          cost = cost + 10;
        }

        document.querySelector('.js-total-cost')
          .innerHTML = `$${cost}`;
      }
    </script>
  </body>
</html>

```
- 10i
```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        font-family: Arial;
        background-color: rgb(0, 0, 0);
      }

      .calculation {
        color: white;
        font-size: 45px;
        margin-top: 15px;
        margin-bottom: 5px;
      }

      .calculator-button {
        height: 60px;
        width: 60px;
        border-radius: 60px;
        border: none;
        font-size: 26px;
        cursor: pointer;
        margin-right: 5px;
      }

      .gray-button {
        background-color: rgb(51, 51, 51);
        color: white;
      }

      .orange-button {
        background-color: rgb(254, 160, 10);
        color: white;
      }

      .clear-button {
        font-size: 17px;
      }
    </style>
  </head>
  <body>
    <!-- Create an element to display the calculation. -->
    <p class="js-calculation calculation"></p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('1');
      ">1</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('2');
      ">2</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('3');
      ">3</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' + ');
      ">+</button>
    </p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('4');
      ">4</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('5');
      ">5</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('6');
      ">6</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' - ');
      ">-</button>
    </p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('7');
      ">7</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('8');
      ">8</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('9');
      ">9</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' * ');
      ">*</button>
    </p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('0');
      ">0</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('.');
      ">.</button>

      <button class="calculator-button gray-button" onclick="
        // Note: eval() takes a string and runs it as code.
        // Avoid using eval() in real world projects since
        // it can potentially be given harmful code to run.
        // Only use eval() for learning purposes.
        calculation = eval(calculation);

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      ">=</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' / ');
      ">/</button>
    </p>

    <p>
      <button class="calculator-button gray-button clear-button" onclick="
        calculation = '';

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      ">Clear</button>
    </p>

    <script>
      let calculation = localStorage.getItem('calculation') || '';

      // Display the calculation when the page first loads.
      displayCalculation();

      function updateCalculation(value) {
        calculation += value;

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      }

      function displayCalculation() {
        document.querySelector('.js-calculation')
          .innerHTML = calculation;
      }
    </script>
  </body>
</html>

```
- 10j
```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="10j.css">
  </head>
  <body>
    <!-- Create an element to display the calculation. -->
    <p class="js-calculation calculation"></p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('1');
      ">1</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('2');
      ">2</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('3');
      ">3</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' + ');
      ">+</button>
    </p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('4');
      ">4</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('5');
      ">5</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('6');
      ">6</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' - ');
      ">-</button>
    </p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('7');
      ">7</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('8');
      ">8</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('9');
      ">9</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' * ');
      ">*</button>
    </p>

    <p>
      <button class="calculator-button gray-button" onclick="
        updateCalculation('0');
      ">0</button>

      <button class="calculator-button gray-button" onclick="
        updateCalculation('.');
      ">.</button>

      <button class="calculator-button gray-button" onclick="
        // Note: eval() takes a string and runs it as code.
        // Avoid using eval() in real world projects since
        // it can potentially be given harmful code to run.
        // Only use eval() for learning purposes.
        calculation = eval(calculation);

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      ">=</button>

      <button class="calculator-button orange-button" onclick="
        updateCalculation(' / ');
      ">/</button>
    </p>

    <p>
      <button class="calculator-button gray-button clear-button" onclick="
        calculation = '';

        // Display the calculation on the page
        // instead of console.log
        displayCalculation();

        localStorage.setItem('calculation', calculation);
      ">Clear</button>
    </p>

    <script src="10j.js"></script>
  </body>
</html>

```
- 10j CSS
```css
body {
  font-family: Arial;
  background-color: rgb(0, 0, 0);
}

.calculation {
  color: white;
  font-size: 45px;
  margin-top: 15px;
  margin-bottom: 5px;
}

.calculator-button {
  height: 60px;
  width: 60px;
  border-radius: 60px;
  border: none;
  font-size: 26px;
  cursor: pointer;
  margin-right: 5px;
}

.gray-button {
  background-color: rgb(51, 51, 51);
  color: white;
}

.orange-button {
  background-color: rgb(254, 160, 10);
  color: white;
}

.clear-button {
  font-size: 17px;
}
```
- 10j js
```js
let calculation = localStorage.getItem('calculation') || '';

// Display the calculation when the page first loads.
displayCalculation();

function updateCalculation(value) {
  calculation += value;

  // Display the calculation on the page
  // instead of console.log
  displayCalculation();

  localStorage.setItem('calculation', calculation);
}

function displayCalculation() {
  document.querySelector('.js-calculation')
    .innerHTML = calculation;
}
```

## Arrays and Loops
- array = is another type of value
- array represents a list of values
- array stores values and array is also a value
- we can also write an array in muliple line
- index = position in the array
- in array we can put any type of value like int float string boolean object array itself
- arrays have properties and method
- if an array doesn't have value then it id called empty array
- loops let us run code over and over
- loop body, loop variable, loop condition, increment/decrement step
- the loop is going for ever is called = infinite loop
- iteration = how many times we run the loop body
- loops create a scope
- standard loop  -->> use for loop  ||   for non-standard loop  -->> while loop
- accumulator pattern ==>> 1. create a variable to store the result  2. loop through the array and update the result
- inside HTML we can't set paragraph tag inside another paragraph tag
- difference between div and p is div doesn't have built in padding margin but p has
- div doesn't have default styling but paragraph has
- arrays and loops
- 1. save the data 2. generate the HTML 3.make it interactive
- by default align-items: stretch; but if mother class in center then it will automatically center
- we can group two or more values together by object or object inside an array
- stretch in align-items is align items vertically stretch
- arrays are references
- break = exit a loop early do does using = return
- break in a loop = return in a function = return also break the loop
- continue = skip 1 iteration
- in for loop using continue incremnet will do automatically but while loop we have to do it manually
- in the last of function body console.log(result) = return result; then console.log(funtionname())
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Arrays and Loops</title>
  </head>
  <body>
    <script>
      /*
      const myArray = [
        10, 
        20, 
        30
      ];
      console.log(myArray);
      console.log(typeof myArray); //
       

      console.log(myArray[1]);
      myArray[0] = 99;
      console.log(myArray);

      [1, 'hello', true, { name: 'socks' }, [1, 2]]

      console.log(typeof [1, 2]); // object (special type of object)
      console.log(Array.isArray([1, 2])); //true

      console.log(myArray.length);
      
      myArray.push(100); // adds a value in the end of the array + it removes value from an array
      console.log(myArray);

      myArray.splice(0, 1); (index, number of value we want to remove)
      console.log(myArray);
      */

      /*
      let i = 1;

      while (i <= 5) {
        console.log(i);
        i++;
      }
      console.log(i);

      for (let i = 1; i <= 5; i++) {
        console.log(i);
      }

      let randomNumber = 0;

      while (randomNumber < 0.5) {
        randomNumber = Math.random();
      }

      console.log(randomNumber);
      */

      /* //  looping through an array
      const todoList = [
        'make dinner',
        'wash dishes',
        'watch youtube'
      ];

      for (let i = 0; i < todoList.length; i++) {
        const value = todoList[index];
        console.log(value);
      }
      */

      /* // accumulator patern
      const nums = [1, 1, 3];
      let total = 0; // accumulator variable

      for (let i = 0; i < nums.length; i++) {
        const num = nums[i];
        total += num;
      }
      console.log(total);

      const numsDoubled = []; // accumulator variable can be an array

      for (let i = 0; i < nums.length; i++) {
        const num = nums[i];
        numsDoubled.push(num * 2);
      }
      console.log(numsDoubled);
      */

      const array1 = [1, 2, 3];
      // const array1 = array2
      // avoid the reference problem
      const array2 = array1.slice();
      array2.push(4);
      console.log(array1);
      console.log(array2);

      const array3 = [1, 2, 3]
      // Destructuring
      const [firstValue, secondValue] = [1, 2, 3];

      for (let i = 1; i <= 10; i++) {
        if (i % 3 === 0) {
          continue;
        }
        console.log(i);
        if (i === 8) {
          break;
        }
      }

      let i = 1;

      while (i <= 10) {
        if (i % 3 === 0) {
          i++;
          // in while loop we have to increment the variable before continue;
          continue;
        }
        console.log(i);
        i++;
      }

      function doubleArray(nums) {
        const numsDoubled = [];

        for (let i = 0; i < nums.length; i++) {
          const num = nums[i];
          if (num === 0) {
            return numsDoubled;
          }
          numsDoubled.push(num * 2);
        }
        return numsDoubled;
      }
      console.log(doubleArray([1, 1, 3]));
      console.log(doubleArray([2, 2, 5, 0, 5]));
    </script>
  </body>
</html>

```
- todo list
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Todo List</title>
    <link rel="stylesheet" href="styles/11-todo-list.css">
  </head>
  <body>
    <p>Todo List</p>

    <div class="todo-input-grid">
      <input placeholder="Todo name"
        class="js-name-input name-input">
      <input type="date"
        class="js-due-date-input due-date-input">
      <button onclick="
        addTodo();
      " class="add-todo-button">Add</button>
    </div>

    <div class="js-todo-list todo-grid"></div>

    <script src="scripts/11-todo-list.js"></script>
  </body>
</html>
```
- todo list CSS

```css
body {
  font-family: Arial;
}

.todo-grid,
.todo-input-grid {
  display: grid;
  grid-template-columns: 200px 150px 100px;
  column-gap: 10px;
  row-gap: 10px;
  align-items: center;
}

.todo-input-grid {
  margin-bottom: 10px;
  align-items: stretch;
}

.name-input,
.due-date-input {
  font-size: 15px;
  padding: 6px;
}

.add-todo-button {
  background-color: green;
  color: white;
  border: none;
  font-size: 15px;
  cursor: pointer;
}

.delete-todo-button {
  background-color: darkred;
  color: white;
  border: none;
  font-size: 15px;
  cursor: pointer;
  padding-top: 10px;
  padding-bottom: 10px;
}
```
- todo list js
```js
/* const todoList = ['make dinner', wash dishes,];
let todoListHTML = ``;
for(let i=0; i<todoList.length; i++){
const todo = todoList[i];
const html = `
<p>
  ${todo}
  <button onclick="
    todoList.splice(${i},1);
    renderTodoList();
  ">Delete</button>
</p>
`;
todoListHTML += html;
}
console.log(todoLlistHTML);
*/
const todoList = [{
  name: 'make dinner',
  dueDate: '2022-12-22'
}, {
  name: 'wash dishes',
  dueDate: '2022-12-22'
}];

renderTodoList();

function renderTodoList() {
  let todoListHTML = '';

  for (let i = 0; i < todoList.length; i++) {
    // const todo = todoList[i];
    const todoObject = todoList[i];
    //const name = todoObject.name;
    //const dueDate = todoObject.dueDate;
    // destructuring variable name == property name
    const { name, dueDate } = todoObject;
    /*
    const html = `
    <p>
      ${name} ${dueDate}
      <button onclick="
          todoList.splice(${i}, 1);
          renderTodoList();
      ">Delete</button>
    </p>
    `;
    */
    const html = `
      <div>${name}</div>
      <div>${dueDate}</div>
      <button onclick="
        todoList.splice(${i}, 1);
        renderTodoList();
      " class="delete-todo-button">Delete</button> 
    `;
    todoListHTML += html;
  }

  // console.log(todoListHTML)

  document.querySelector('.js-todo-list')
    .innerHTML = todoListHTML;
}

function addTodo() {
  const inputElement = document.querySelector('.js-name-input');
  const name = inputElement.value;

  const dateInputElement = document.querySelector('.js-due-date-input');
  const dueDate = dateInputElement.value;

  /*
  todoList.push(name);
  console.log(todoList);
  */

  todoList.push({
    //name: name,
    //dueDate: dueDate,
    //shorthand property  property = variable name
    name,
    dueDate
  });
  //console.log(todoList);

  inputElement.value = '';

  renderTodoList();
}
```
- exercise
- 11a
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const nums = [10, 20, 30];
      nums[2] = 99;
      console.log(nums);

      // An alternative solution is:
      // nums[nums.length - 1] = 99;
    </script>
  </body>
</html>
```
- 11b
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function getLastValue(array) {
        const lastIndex = array.length - 1;
        return array[lastIndex];
      }
      console.log(getLastValue([1, 20, 22, 24, 5]));
      console.log(getLastValue(['hi', 'hello', 'hey']));
    </script>
  </body>
</html>
```
- 11c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function arraySwap(array) {
        const lastIndex = array.length - 1;

        // We need to save the values first before
        // swapping. Otherwise, if we swap directly,
        // we would lose one of the values.
        const lastValue = array[lastIndex];
        const firstValue = array[0];

        array[0] = lastValue;
        array[lastIndex] = firstValue;

        return array;
      }
      console.log(arraySwap([1, 20, 22, 24, 5]));
      console.log(arraySwap(['hi', 'hello', 'hey']));
    </script>
  </body>
</html>
```
- 11d
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      for (let i = 0; i <= 10; i += 2) {
        console.log(i);
      }
    </script>
  </body>
</html>
```
- 11e
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      for (let i = 5; i >= 0; i--) {
        console.log(i);
      }
    </script>
  </body>
</html>
```
- 11f
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      let i = 0;

      while (i <= 10) {
        console.log(i);
        i += 2;
      }

      i = 5;

      while (i >= 0) {
        console.log(i);
        i--;
      }
    </script>
  </body>
</html>
```
- 11g
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const array = [1, 2, 3];
      const result = [];

      for (let i = 0; i < array.length; i++) {
        result.push(array[i] + 1);
      }

      console.log(result);
    </script>
  </body>
</html>
```
- 11h
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function addOne(array) {
        const result = [];

        for (let i = 0; i < array.length; i++) {
          result.push(array[i] + 1);
        }

        return result;
      }

      console.log(addOne([1, 2, 3]));
      console.log(addOne([-2, -1, 0, 99]));
    </script>
  </body>
</html>
```
- 11i
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function addNum(array, num) {
        const result = [];

        for (let i = 0; i < array.length; i++) {
          result.push(array[i] + num);
        }

        return result;
      }

      console.log(addNum([1, 2, 3], 2));
      console.log(addNum([1, 2, 3], 3));
      console.log(addNum([-2, -1, 0, 99], 2));
    </script>
  </body>
</html>
```
- 11j
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function addArrays(array1, array2) {
        const result = [];

        for (let i = 0; i < array1.length; i++) {
          result.push(array1[i] + array2[i]);
        }

        return result;
      }

      console.log(addArrays([1, 1, 2], [1, 1, 3]));
      console.log(addArrays([1, 2, 3], [4, 5, 6]));
    </script>
  </body>
</html>
```
- 11k
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function countPositive(nums) {
        let result = 0;

        for (let i = 0; i < nums.length; i++) {
          if (nums[i] > 0) {
            result++;
          }
        }

        return result;
      }

      console.log(countPositive([1, -3, 5]));
      console.log(countPositive([-2, 3, -5, 7, 10]));
    </script>
  </body>
</html>
```
- 11l
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function minMax(nums) {
        // We'll set the starting values of min and max
        // as the first value in the array. (This is
        // just one way to set the starting values. You
        // can use another way if you like.)
        const result = {
          min: nums[0],
          max: nums[0]
        };

        for (let i = 0; i < nums.length; i++) {
          const value = nums[i];

          // If the value is less than the min,
          // update the min.
          if (value < result.min) {
            result.min = value;
          }

          // If the value is greater than the max,
          // update the max.
          if (value > result.max) {
            result.max = value;
          }
        }

        return result;
      }

      console.log(minMax([1, -3, 5]));
      console.log(minMax([-2, 3, -5, 7, 10]));

    </script>
  </body>
</html>
```
- 11m
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function minMax(nums) {
        // We'll set the starting values of min and max
        // to null this time.
        const result = {
          min: null,
          max: null
        };

        for (let i = 0; i < nums.length; i++) {
          const value = nums[i];

          // If the min is null OR the value is
          // less than the min, update the min.
          if (result.min === null || value < result.min) {
            result.min = value;
          }

          // If the max is null OR the value is
          // greater than the max, update the max.
          if (result.max === null || value > result.max) {
            result.max = value;
          }

          // We have to use 2 if-statements above instead of
          // an if-else statement. This makes sure both the
          // min and max are set if they are null.
        }

        return result;
      }

      console.log(minMax([1, -3, 5]));
      console.log(minMax([-2, 3, -5, 7, 10]));

      console.log(minMax([]));
      console.log(minMax([3]));
    </script>
  </body>
</html>
```
- 11n
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function countWords(words) {
        const result = {};

        for (let i = 0; i < words.length; i++) {
          const word = words[i];

          // result[word] adds/accesses a property using whatever is
          // saved inside the 'word' variable.
          // If word = 'apple', result[word] will do result['apple']
          // If word = 'grape', result[word] will do result['grape']
          if (!result[word]) {
            result[word] = 1;
          } else {
            result[word]++;
          }
        }

        return result;
      }

      console.log(countWords(['apple', 'grape', 'apple', 'apple']));
    </script>
  </body>
</html>
```
- 11o
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      let words = ['hello', 'world', 'search', 'good'];

      // Set the index to -1 at the start (so we'll assume
      // the string 'search' doesn't exist in the array).
      // If we find the string 'search' in the array, we
      // will update the index.
      let index = -1;

      for (let i = 0; i < words.length; i++) {
        if (words[i] === 'search') {
          index = i;
        }
      }

      console.log(index);

      words = ['not', 'found'];
      index = -1;

      for (let i = 0; i < words.length; i++) {
        if (words[i] === 'search') {
          index = i;
        }
      }

      console.log(index);
    </script>
  </body>
</html>
```
- 11p
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      let words = ['hello', 'world', 'search', 'good', 'search'];
      let index = -1;

      for (let i = 0; i < words.length; i++) {
        if (words[i] === 'search') {
          index = i;
          // Once we find 'search', immediately exit
          // the loop since we want the index of the
          // first appearance of 'search'.
          break;
        }
      }

      console.log(index);

      words = ['not', 'found'];
      index = -1;

      for (let i = 0; i < words.length; i++) {
        if (words[i] === 'search') {
          index = i;
          break;
        }
      }

      console.log(index);
    </script>
  </body>
</html>
```
- 11q
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function findIndex(array, word) {
        for (let i = 0; i < array.length; i++) {
          if (array[i] === word) {
            // Instead of creating an accumulator
            // variable and updating it in the loop,
            // we can just return i directly, when
            // we find it since this is a function.
            return i;
          }
        }

        // If the function has not returned by now,
        // logically that means the word must not
        // exist in the array, so we'll return -1.
        return -1;
      }
    </script>
  </body>
</html>
```
- 11r
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function removeEgg(foods) {
        const result = [];

        for (let i = 0; i < foods.length; i++) {
          // If the string is 'egg', use continue to skip it.
          if (foods[i] === 'egg') {
            continue;
          }

          // We don't need to have an else here because
          // the only way to reach this code is if the 
          // if-statement above is false.
          result.push(foods[i]);
        }

        return result;
      }

      console.log(removeEgg(['egg', 'apple', 'egg', 'egg', 'ham']));
    </script>
  </body>
</html>
```
- 11s
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function removeEgg(foods) {
        const result = [];
        let eggsRemoved = 0;

        for (let i = 0; i < foods.length; i++) {
          // Only skip 'egg' if we removed less than 2
          // of them so far.
          if (foods[i] === 'egg' && eggsRemoved < 2) {
            // Update the number of 'egg' we have removed.
            // This must be done before continue, otherwise,
            // doing continue first will just skip this code.
            eggsRemoved++;
            continue;
          }

          result.push(foods[i]);
        }

        return result;
      }

      console.log(removeEgg(['egg', 'apple', 'egg', 'egg', 'ham']));
    </script>
  </body>
</html>
```
- 11t
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function removeEgg(foods) {
        // To remove the last 2 'egg', reverse the array first.
        const reversedFoods = foods.reverse();

        const result = [];
        let eggsRemoved = 0;

        for (let i = 0; i < reversedFoods.length; i++) {
          if (reversedFoods[i] === 'egg' && eggsRemoved < 2) {
            eggsRemoved++;
            continue;
          }

          result.push(reversedFoods[i]);
        }

        // At the end, remember to .reverse() back the result.
        return result.reverse();
      }

      console.log(removeEgg(['egg', 'apple', 'egg', 'egg', 'ham']));
    </script>
  </body>
</html>
```
- 11u
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function removeEgg(foods) {
        // To prevent modifying the original array, we
        // can create a copy of the array using .slice()
        const foodsCopy = foods.slice();
        const reversedFoods = foodsCopy.reverse();

        // Advanced technique:
        // Since foods.slice() results in an array, we
        // can also use .reverse() directly like this:
        // foods.slice().reverse();
        
        // This technique is called "method chaining"
        // because we use one method after another
        // (like a chain of methods).
        const result = [];
        let eggsRemoved = 0;

        for (let i = 0; i < reversedFoods.length; i++) {
          if (reversedFoods[i] === 'egg' && eggsRemoved < 2) {
            eggsRemoved++;
            continue;
          }

          result.push(reversedFoods[i]);
        }

        return result.reverse();
      }

      const foods = ['egg', 'apple', 'egg', 'egg', 'ham'];
      console.log(removeEgg(foods));
      console.log(foods);
    </script>
  </body>
</html>
```
- 11v
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      for (let i = 1; i <= 20; i++) {
        // The trick to this problem is to check if
        // the number is divisible by 3 and 5 first.
        // Otherwise, it will always display 'Fizz'.
        if (i % 3 === 0 && i % 5 === 0) {
          console.log('FizzBuzz');

        } else if (i % 3 === 0) {
          console.log('Fizz');

        } else if (i % 5 === 0) {
          console.log('Buzz');
          
        } else {
          console.log(i);
        }
      }
    </script>
  </body>
</html>
```
- 11w
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function findIndex(array, word) {
        for (let i = 0; i < array.length; i++) {
          if (array[i] === word) {
            return i;
          }
        }

        return -1;
      }

      function unique(array) {
        const result = [];

        for (let i = 0; i < array.length; i++) {
          const word = array[i];

          // Using the findIndex() function from above, we
          // can check if the string is already in the
          // result array. If it's not in the result array
          // (index is -1), then add it to the result array.
          if (findIndex(result, word) === -1) {
            result.push(word);
          }
        }

        return result;
      }

      console.log(unique(['green', 'red', 'blue', 'red']));
      console.log(unique(['red', 'green', 'green', 'red']));
    </script>
  </body>
</html>
```
- 11x html
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Todo List</title>
    <link rel="stylesheet" href="11x.css">
  </head>
  <body>
    <p>Todo List</p>

    <div class="todo-input-grid">
      <input placeholder="Todo name"
        class="js-name-input name-input">
      <input type="date"
        class="js-due-date-input due-date-input">
      <button onclick="
        addTodo();
      " class="add-todo-button">Add</button>
    </div>

    <div class="js-todo-list todo-grid"></div>

    <script src="11x.js"></script>
  </body>
</html>

```
- 11x css
```css
body {
  font-family: Arial;
}

.todo-grid,
.todo-input-grid {
  display: grid;
  grid-template-columns: 200px 150px 100px;
  column-gap: 10px;
  row-gap: 10px;
  align-items: center;
}

.todo-input-grid {
  margin-bottom: 10px;
  align-items: stretch;
}

.name-input,
.due-date-input {
  font-size: 15px;
  padding: 6px;
}

.add-todo-button {
  background-color: green;
  color: white;
  border: none;
  font-size: 15px;
  cursor: pointer;
}

.delete-todo-button {
  background-color: darkred;
  color: white;
  border: none;
  font-size: 15px;
  cursor: pointer;
  padding-top: 10px;
  padding-bottom: 10px;
}
```
- 11x js
```js
// When loading the page, load from localStorage.
const todoList = JSON.parse(localStorage.getItem('todoList')) || [{
  name: 'make dinner',
  dueDate: '2022-12-22'
}, {
  name: 'wash dishes',
  dueDate: '2022-12-22'
}];

renderTodoList();

function renderTodoList() {
  let todoListHTML = '';

  for (let i = 0; i < todoList.length; i++) {
    const todoObject = todoList[i];
    //const name = todoObject.name;
    //const dueDate = todoObject.dueDate;
    const { name, dueDate } = todoObject;
    const html = `
      <div>${name}</div>
      <div>${dueDate}</div>
      <button onclick="
        todoList.splice(${i}, 1);
        renderTodoList();

        // Whenever we update the todo list, save in localStorage.
        saveToStorage();
      " class="delete-todo-button">Delete</button> 
    `;
    todoListHTML += html;
  }

  document.querySelector('.js-todo-list')
    .innerHTML = todoListHTML;
}

function addTodo() {
  const inputElement = document.querySelector('.js-name-input');
  const name = inputElement.value;

  const dateInputElement = document.querySelector('.js-due-date-input');
  const dueDate = dateInputElement.value;

  todoList.push({
    //name: name,
    //dueDate: dueDate,
    name,
    dueDate
  });

  inputElement.value = '';

  renderTodoList();

  // Whenever we update the todo list, save in localStorage.
  saveToStorage();
}

function saveToStorage() {
  localStorage.setItem('todoList', JSON.stringify(todoList));
}
```

## advamced function

- advanced function
- functions are values
- anonymous function = function without a name
- function saved with a variable can't provide the feature hoisting
- but function with only function keyword can provide hoisting feature
- we can save a funtion(a value) in an object = method
- we can pass a value into a function
- anything we do with a value we can do with a function
- setTimeout() = allows us to run a function in the future
- setTimeout() is a built in funtion
- setTimeout(function(){console.log('timeout');}, 3000);
- Synchronous Code = will wait for a line to finish before going to the next line
- Asynchronous Code = won't wait for a line to finish before going to the next line
- Advantages of Asynchronous Code = it doesn't block our code for given time
- setInterval() is a built in function
- setInterval(function(){console.log('interval');}, 3000); // it also asynchronous
- setInterval() returns a number = we can use that numbr to stop the interval
- clearInterval(intervalID) = to stop the setInterval()
- .forEach(function(value, index){})
- forEach() method won't provide the loop term 'continue'
- in forEach() method return = continue || forEach() method doesn't have break
- if we need to use break in forEach() then it is better to use a regular for loop
- Arrow function
- Arrow functions have shorcuts
- if one parameter in arrow function then parenthisis(round bracket) is optional
- if one line code only inside arrow funtion body then  1. put the code in oneline 2.curly bracket is   optional 3.return keyword is optional
- passing a function into another function ==>> use  arrow funtion
- regular funtion in initial funtion provides 1. easier to read 2. hoisting
- hoisting = call this function before it is created
- uses of arrow funtion
  1. funtion into another funtion
  2. inside an object but it is better that we also shorthand method
  3. inside addEventListener() method or other method
- we use addEventListener() rather than using onclick = "" attribute
- every HTML element has a method called addEventListener() = let us run some code when we interact     with the element
- addEventListener has some benifits
  1. add multiple event listeners for an event
  2. remove listener from an event
- we can remove event listener by removeEventListener()
- But removeEventListener() must have the exact funtion that addEventListener() have
- for this reason we save the funtion in a variable first then in funtion parameter we just put the     same variable
- if we want to use keyboard event listener == document.body.addEventListener('keydown' (event)=>{
  console.log(event.key);});
- addEventListener() also provide 'event' object but it provide this as a parameter
- in order to addEventListenr() we need to add the html first (by js)
- if we select all element = document.querySelectorAll('.class-name')
  it gives us a list just like an array
- .filter(value, index)
  1. creates new array[]
  2. return true, put value in array
  3. return false, not put value in array
- .map(value, index)
  1. creates a new array
  2. return , add in new array
  3. transform an array into another array
- if a function has access to a value -> it wil always have access to that value
  value gets packaged together (enclosed) with the function
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Advanced Functions</title>
  </head>
  <body>
    <button onclick="" class="js-button">Click</button>

    <script>
      /* function greeting(){
      console.log('hello')
      }
      greeting();
      const num = 2;
      const function1 = function greeting(){
      console.log('hello2')
      };
      function1(); // calling the function // hello2
      console.log(function1); // f greeting(){console.log('hello2');}
      console.log(typeof function1); // function
      /*
      /*
      // cleanup
      
      const function1 = function(){ //anonymous function
      console.log('hello2');
      }
      */
      const buttonElement = document.querySelector('.js-button');

      const eventListener = () => {
        console.log('click');
      };
      buttonElement.addEventListener('click', eventListener);

      buttonElement.removeEventListener('click', eventListener);

      buttonElement.addEventListener('click', () => {
        console.log('click2');
      });
      */

      /*
      greeting();
      function greeting() {
        console.log('hello');
      }
      greeting();

      const num = 2;
      const function1 = function() {
        console.log('hello2');
      };

      console.log(function1);
      console.log(typeof function1);
      function1();

      const object1 = {
        num: 2,
        // fun: function greeting() { //we can remove the name because we can access the function by
        // -- object1.fun()
        fun: function() {
          console.log('hello3'); 
        } // function inside an object called method
      };
      object1.fun();

      function display(param) { // here is param = parameter = passing a value into a function
        console.log(param);
      }
      display(2); // here 2 is argument

      function run(param) {
        param();
      }
      run(function() {  // passing a function into a function 
        console.log('hello4');
      // the function that is passing into is called = callback funtion
      });
      */
      // Asynchronous Programming
      /*
      setTimeout(function() {
        console.log('timeout'); // inside this function is also synchronous
        console.log('timeout2'); // inside this function is also synchronous
      }, 3000);

      console.log('next line');

      setInterval(function() {
        console.log('interval');
      }, 3000);

      console.log('next line 2');
      */

      /*
      // loop through an array
      [
        'make dinner',
        'wash dishes',
        'watch youtube'
      ].forEach((value, index) => {
        // console.log(index);
        // console.log(value);
        if (value === 'wash dishes') {
          return; // end this function early
        }

        console.log(index);
        console.log(value);
      });

      const regularFunction = function(param, param2) {
        console.log('hello');
        return 5;
      };
      regularFuntion(2,3);

      const arrowFunction = (param, param2) => {
        console.log('hello');
        return 5;
      };
      arrowFunction(2,3);

      const oneParam = param => {
        console.log(param + 1);
      };
      oneParam(2);

      const oneLine = () => 2 + 3;
      console.log(oneLine());

      const object2 = {
        method: () => {

        },
        method() { // shorthand method

        }
      };
      */

      console.log([1, -3, 5].filter((value, index) => {
        /*
        if (value >= 0) {
          return true;
        } else {
          return false;
        }
        */
        return value >= 0;
      }));

      console.log([1, 1, 3].map((value, index) => {
        return value * 2;
      }));

      console.log([1, 1, 3].map(value => value * 2));
    </script>
  </body>
</html>

```
- rock paper scissors html
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
    <link rel="stylesheet" href="styles/12-rock-paper-scissors.css">
  </head>
  <body>
    <p class="title">Rock Paper Scissors</p>
    <button class="move-button js-rock-button">
      <img src="images/rock-emoji.png" class="move-icon">
    </button>

    <button class="move-button js-paper-button">
      <img src="images/paper-emoji.png" class="move-icon">
    </button>

    <button class="move-button js-scissors-button">
      <img src="images/scissors-emoji.png" class="move-icon">
    </button>

    <p class="js-result result"></p>
    <p class="js-moves"></p>
    <p class="js-score score"></p>

    <button onclick="
      score.wins = 0;
      score.losses = 0;
      score.ties = 0;
      localStorage.removeItem('score');
      updateScoreElement();
    " class="reset-score-button js-reset-score-button">Reset Score</button>

    <button class="auto-play-button" onclick="
      autoPlay();
    ">Auto Play</button>
    
    <script src="scripts/12-rock-paper-scissors.js"></script>
  </body>
</html>

```
- rock paper scissors css
```css
body {
  background-color: rgb(25, 25, 25);
  color: white;
  font-family: Arial;
}

.title {
  font-size: 30px;
  font-weight: bold;
}

.move-icon {
  height: 50px;
}

.move-button {
  background-color: transparent;
  border: 3px solid white;
  width: 120px;
  height: 120px;
  border-radius: 60px;
  margin-right: 10px;
  cursor: pointer;
}

.result {
  font-size: 25px;
  font-weight: bold;
  margin-top: 50px;
}

.score {
  margin-top: 60px;
}

.reset-score-button,
.auto-play-button {
  background-color: white;
  border: none;
  font-size: 15px;
  padding: 8px 15px;
  cursor: pointer;
}
```

- rock paper scissors js
```js
let score = JSON.parse(localStorage.getItem('score')) || {
  wins: 0,
  losses: 0,
  ties: 0
};

updateScoreElement();

/*
if (!score) {
  score = {
    wins: 0,
    losses: 0,
    ties: 0
  };
}
*/

let isAutoPlaying = false;
let intervalId; // in order to save the last id

//const autoPlay = () => {

//};
function autoPlay() {
  if (!isAutoPlaying) {
    intervalId = setInterval(() => {
      const playerMove = pickComputerMove();
      playGame(playerMove);
    }, 1000);
    isAutoPlaying = true;

  } else {
    clearInterval(intervalId);
    isAutoPlaying = false;
  }
}

document.querySelector('.js-rock-button')
  .addEventListener('click', () => {
    playGame('rock');
  });

document.querySelector('.js-paper-button')
  .addEventListener('click', () => {
    playGame('paper');
  });

document.querySelector('.js-scissors-button')
  .addEventListener('click', () => {
    playGame('scissors');
  });

document.body.addEventListener('keydown', (event) => {
  if (event.key === 'r') {
    playGame('rock');
  } else if (event.key === 'p') {
    playGame('paper');
  } else if (event.key === 's') {
    playGame('scissors');
  }
});

function playGame(playerMove) {
  const computerMove = pickComputerMove();

  let result = '';

  if (playerMove === 'scissors') {
    if (computerMove === 'rock') {
      result = 'You lose.';
    } else if (computerMove === 'paper') {
      result = 'You win.';
    } else if (computerMove === 'scissors') {
      result = 'Tie.';
    }

  } else if (playerMove === 'paper') {
    if (computerMove === 'rock') {
      result = 'You win.';
    } else if (computerMove === 'paper') {
      result = 'Tie.';
    } else if (computerMove === 'scissors') {
      result = 'You lose.';
    }
    
  } else if (playerMove === 'rock') {
    if (computerMove === 'rock') {
      result = 'Tie.';
    } else if (computerMove === 'paper') {
      result = 'You lose.';
    } else if (computerMove === 'scissors') {
      result = 'You win.';
    }
  }

  if (result === 'You win.') {
    score.wins += 1;
  } else if (result === 'You lose.') {
    score.losses += 1;
  } else if (result === 'Tie.') {
    score.ties += 1;
  }

  localStorage.setItem('score', JSON.stringify(score));

  updateScoreElement();

  document.querySelector('.js-result').innerHTML = result;

  document.querySelector('.js-moves').innerHTML = `You
<img src="images/${playerMove}-emoji.png" class="move-icon">
<img src="images/${computerMove}-emoji.png" class="move-icon">
Computer`;
}

function updateScoreElement() {
  document.querySelector('.js-score')
    .innerHTML = `Wins: ${score.wins}, Losses: ${score.losses}, Ties: ${score.ties}`;
}

function pickComputerMove() {
  const randomNumber = Math.random();

  let computerMove = '';

  if (randomNumber >= 0 && randomNumber < 1 / 3) {
    computerMove = 'rock';
  } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
    computerMove = 'paper';
  } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
    computerMove = 'scissors';
  }

  return computerMove;
}
```

- todo list html

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Todo List</title>
    <link rel="stylesheet" href="styles/12-todo-list.css">
  </head>
  <body>
    <p>Todo List</p>

    <div class="todo-input-grid">
      <input placeholder="Todo name"
        class="js-name-input name-input">
      <input type="date"
        class="js-due-date-input due-date-input">
      <button class="add-todo-button js-add-todo-button">Add</button>
    </div>

    <div class="js-todo-list todo-grid"></div>

    <script src="scripts/12-todo-list.js"></script>
  </body>
</html>

```
- todo list css
```css
body {
  font-family: Arial;
}

.todo-grid,
.todo-input-grid {
  display: grid;
  grid-template-columns: 200px 150px 100px;
  column-gap: 10px;
  row-gap: 10px;
  align-items: center;
}

.todo-input-grid {
  margin-bottom: 10px;
  align-items: stretch;
}

.name-input,
.due-date-input {
  font-size: 15px;
  padding: 6px;
}

.add-todo-button {
  background-color: green;
  color: white;
  border: none;
  font-size: 15px;
  cursor: pointer;
}

.delete-todo-button {
  background-color: darkred;
  color: white;
  border: none;
  font-size: 15px;
  cursor: pointer;
  padding-top: 10px;
  padding-bottom: 10px;
}
```
- todo list js
```js
const todoList = [{
  name: 'make dinner',
  dueDate: '2022-12-22'
}, {
  name: 'wash dishes',
  dueDate: '2022-12-22'
}];

renderTodoList();

function renderTodoList() {
  let todoListHTML = '';

  todoList.forEach((todoObject, index) => {
    const { name, dueDate } = todoObject;
    const html = `
      <div>${name}</div>
      <div>${dueDate}</div>
      <button class="delete-todo-button js-delete-todo-button">Delete</button> 
    `;
    todoListHTML += html;
  });

  document.querySelector('.js-todo-list')
    .innerHTML = todoListHTML;

  document.querySelectorAll('.js-delete-todo-button')
    .forEach((deleteButton, index) => {
      deleteButton.addEventListener('click', () => {
        todoList.splice(index, 1);
        renderTodoList();
      });
    });
}

document.querySelector('.js-add-todo-button')
  .addEventListener('click', () => {
    addTodo();
  });

function addTodo() {
  const inputElement = document.querySelector('.js-name-input');
  const name = inputElement.value;

  const dateInputElement = document.querySelector('.js-due-date-input');
  const dueDate = dateInputElement.value;

  todoList.push({
    //name: name,
    //dueDate: dueDate,
    name,
    dueDate
  });

  inputElement.value = '';

  renderTodoList();
}
```
- exercise
- 12a
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const add = function() {
        console.log(2 + 3);
      };

      add();
      add();
    </script>
  </body>
</html>
```
- 12b
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const add = function() {
        console.log(2 + 3);
      };

      add();
      add();

      function runTwice(fun) {
        fun();
        fun();
      }

      runTwice(function() {
        console.log('12b');
      });
      
      runTwice(add);
    </script>
  </body>
</html>
```
- 12c
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button class="js-button" onclick="
      updateButton();
    ">Start</button>

    <script>
      // Grouping the JavaScript code into a function
      // is optional, but it is a bit cleaner.
      function updateButton() {
        const button = document.querySelector('.js-button');

        setTimeout(function() {
          button.innerHTML = 'Finished!';
        }, 1000);
      }
    </script>
  </body>
</html>
```
- 12d
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button class="js-button" onclick="
      updateButton();
    ">Start</button>

    <script>
      function updateButton() {
        const button = document.querySelector('.js-button');
        
        button.innerHTML = 'Loading...';
        setTimeout(function() {
          button.innerHTML = 'Finished!';
        }, 1000);
      }
    </script>
  </body>
</html>
```
- 12e
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button class="js-button" onclick="
      displayMessage();
    ">Add to cart</button>
    
    <p class="js-message"></p>

    <script>
      function displayMessage() {
        const messageElement = document.querySelector('.js-message');
        messageElement.innerHTML = 'Added';

        setTimeout(function() {
          messageElement.innerHTML = '';
        }, 2000);
      }
    </script>
  </body>
</html>
```
- 12f
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <button class="js-button" onclick="
      displayMessage();
    ">Add to cart</button>
    
    <p class="js-message"></p>

    <script>
      let timeoutId;

      function displayMessage() {
        const messageElement = document.querySelector('.js-message');
        messageElement.innerHTML = 'Added';

        // First, cancel the previous timeout so that
        // it doesn't remove the message too quickly.
        clearTimeout(timeoutId);

        timeoutId = setTimeout(function() {
          messageElement.innerHTML = '';
        }, 2000);
      }
    </script>
  </body>
</html>
```
- 12g
```html
<!DOCTYPE html>
<html>
  <head>
    <title>App</title>
  </head>
  <body>
    <script>
      setInterval(function() {
        if (document.title === 'App') {
          document.title = '(2) New messages';
        } else {
          document.title = 'App';
        }
      }, 1000);
    </script>
  </body>
</html>
```
- 12h
```html
<!DOCTYPE html>
<html>
  <head>
    <title>App</title>
  </head>
  <body>
    <button onclick="
      messages++;
    ">Add</button>

    <button onclick="
      messages--;
    ">Remove</button>

    <script>
      let messages = 2;

      setInterval(function() {
        if (document.title === 'App') {
          document.title = `(${messages}) New messages`;
        } else {
          document.title = 'App';
        }
      }, 1000);
    </script>
  </body>
</html>
```
- 12i
```html
<!DOCTYPE html>
<html>
  <head>
    <title>App</title>
  </head>
  <body>
    <!--
      Note: This is just a sample solution. Other
      solutions are possible so don't worry if
      your solution looks different.
    -->
    <button onclick="
      messages++;
      displayNotification();
    ">Add</button>

    <button onclick="
      if (messages > 0) {
        messages--;

        // If there are no new messages, stop displaying
        // the notification in the tab.
        if (messages === 0) {
          stopNotification();
        }
      }
    ">Remove</button>

    <script>
      let messages = 2;

      // Save the intervalId in case we need to cancel it.
      let intervalId;

      // We'll use this variable to keep track of whether
      // or not we're displaying the notification.
      let isDisplayingNotification;

      // Start displaying the notification in the tab
      // when the page first loads.
      displayNotification();

      function displayNotification() {
        // If we're already displaying the notification,
        // stop this function because we don't want to
        // create 2 intervals at the same time.
        if (isDisplayingNotification) {
          return;
        }

        isDisplayingNotification = true;

        intervalId = setInterval(function() {
          if (document.title === 'App') {
            document.title = `(${messages}) New messages`;
          } else {
            document.title = 'App';
          }
        }, 1000);
      }

      function stopNotification() {
        isDisplayingNotification = false;

        clearInterval(intervalId);
        document.title = 'App';
      }
    </script>
  </body>
</html>
```
- 12j
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const multiply = (a, b) => {
        return a * b;
      };

      console.log(multiply(2, 3));
      console.log(multiply(7, 10));
    </script>
  </body>
</html>
```
- 12k
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      const multiply = (a, b) => a * b;

      console.log(multiply(2, 3));
      console.log(multiply(7, 10));
    </script>
  </body>
</html>
```
- 12l
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function countPositive(nums) {
        let positiveNumbers = 0;

        // When there is only 1 parameter,
        // the brackets are optional. So
        // we can also write: num => { ... }
        nums.forEach((num) => {
          if (num > 0) {
            positiveNumbers++;
          }
        });

        return positiveNumbers;
      }

      console.log(countPositive([1, -3, 5]));
      console.log(countPositive([-2, 3, -5, 7, 10]));
    </script>
  </body>
</html>
```
- 12m
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function addNum(array, num) {
        // When there is only 1 parameter,
        // the brackets are optional. So we
        // can also write: value => value + num
        return array.map((value) => value + num);
      }

      console.log(addNum([1, 2, 3], 2));
      console.log(addNum([-2, -1, 0, 99], 2));
    </script>
  </body>
</html>
```
- 12n
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function removeEgg(foods) {
        // If food is 'egg', the inner function returns false
        //   and the food is not included in the result.
        // Otherwise, the inner function returns true
        //   and the food is included in the result. 
        return foods.filter((food) => food !== 'egg');
      }

      console.log(removeEgg(['egg', 'apple', 'egg', 'egg', 'ham']));
    </script>
  </body>
</html>
```
- 12o
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <script>
      function removeEgg(foods) {
        let eggsRemoved = 0;

        return foods.filter((food) => {
          // If the food is 'egg', we should return false
          // but only if we haven't removed 2 eggs already.
          if (food === 'egg' && eggsRemoved < 2) {
            eggsRemoved++;
            return false;
          }

          return true;
        });
      }

      console.log(removeEgg(['egg', 'apple', 'egg', 'egg', 'ham']));
    </script>
  </body>
</html>
```
- 12p
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <!--
      This is the updated code for exercise 12c
      just as an example. Feel free, to update
      12d - 12i as well for more practice.
    -->
    <button class="js-button" onclick="
      updateButton();
    ">Start</button>

    <script>
      function updateButton() {
        const button = document.querySelector('.js-button');

        // The function below was changed
        // to an arrow function.
        setTimeout(() => {
          button.innerHTML = 'Finished!';
        }, 1000);
      }
    </script>
  </body>
</html>
```
- 12q
```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <!--
      This is the updated code for exercise 12c
      just as an example. Feel free, to update
      12d - 12i as well for more practice.
    -->
    <button class="js-button">Start</button>

    <script>
      document.querySelector('.js-button')
        .addEventListener('click', () => {
          const button = document.querySelector('.js-button');

          // The function below was changed
          // to an arrow function.
          setTimeout(() => {
            button.innerHTML = 'Finished!';
          }, 1000);
        });
    </script>
  </body>
</html>
```
- 12r html
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Rock Paper Scissors</title>
    <link rel="stylesheet" href="12r.css">
  </head>
  <body>
    <p class="title">Rock Paper Scissors</p>
    <button class="move-button js-rock-button">
      <img src="images/rock-emoji.png" class="move-icon">
    </button>

    <button class="move-button js-paper-button">
      <img src="images/paper-emoji.png" class="move-icon">
    </button>

    <button class="move-button js-scissors-button">
      <img src="images/scissors-emoji.png" class="move-icon">
    </button>

    <p class="js-result result"></p>
    <p class="js-moves"></p>
    <p class="js-score score"></p>

    <!-- Solution for exercise 12v. -->
    <button class="reset-score-button js-reset-score-button">
      Reset Score
    </button>

    <!-- Solution for exercise 12s. -->
    <button class="auto-play-button js-auto-play-button">
      Auto Play
    </button>

    <!-- Solution for exercise 12x. -->
    <p class="js-reset-confirmation"></p>
    
    <script src="12r.js"></script>
  </body>
</html>

```
- 12r css
```css
body {
  background-color: rgb(25, 25, 25);
  color: white;
  font-family: Arial;
}

.title {
  font-size: 30px;
  font-weight: bold;
}

.move-icon {
  height: 50px;
}

.move-button {
  background-color: transparent;
  border: 3px solid white;
  width: 120px;
  height: 120px;
  border-radius: 60px;
  margin-right: 10px;
  cursor: pointer;
}

.result {
  font-size: 25px;
  font-weight: bold;
  margin-top: 50px;
}

.score {
  margin-top: 60px;
}

.reset-score-button,
.auto-play-button,
/* Solution for exercise 12x. */
.reset-confirm-button {
  background-color: white;
  border: none;
  font-size: 15px;
  padding: 8px 15px;
  cursor: pointer;
}

/* Solution for exercise 12x. */
.reset-confirm-button {
  margin-left: 10px;
}
```
- 12r js
```js
let score = JSON.parse(localStorage.getItem('score')) || {
  wins: 0,
  losses: 0,
  ties: 0
};

updateScoreElement();

/*
if (!score) {
  score = {
    wins: 0,
    losses: 0,
    ties: 0
  };
}
*/

let isAutoPlaying = false;
let intervalId;

//const autoPlay = () => {

//};
function autoPlay() {
  if (!isAutoPlaying) {
    intervalId = setInterval(() => {
      const playerMove = pickComputerMove();
      playGame(playerMove);
    }, 1000);
    isAutoPlaying = true;
    
    // Solution for 12t.
    document.querySelector('.js-auto-play-button')
      .innerHTML = 'Stop Playing';

  } else {
    clearInterval(intervalId);
    isAutoPlaying = false;

    // Solution for 12t.
    document.querySelector('.js-auto-play-button')
      .innerHTML = 'Auto Play';
  }
}

// Solution for exercise 12s.
document.querySelector('.js-auto-play-button')
  .addEventListener('click', () => {
    autoPlay();
  });

document.querySelector('.js-rock-button')
  .addEventListener('click', () => {
    playGame('rock');
  });

document.querySelector('.js-paper-button')
  .addEventListener('click', () => {
    playGame('paper');
  });

document.querySelector('.js-scissors-button')
  .addEventListener('click', () => {
    playGame('scissors');
  });

  document.body.addEventListener('keydown', (event) => {
    if (event.key === 'r') {
      playGame('rock');
    } else if (event.key === 'p') {
      playGame('paper');
    } else if (event.key === 's') {
      playGame('scissors');
    
    // Solution for 12u.
    } else if (event.key === 'a') {
      autoPlay();
    
    // Solution for 12w.
    } else if (event.key === 'Backspace') {
      // Solution for 12w.
      // resetScore();

      // Solution for 12x.
      showResetConfirmation();
    }
  });

function playGame(playerMove) {
  const computerMove = pickComputerMove();

  let result = '';

  if (playerMove === 'scissors') {
    if (computerMove === 'rock') {
      result = 'You lose.';
    } else if (computerMove === 'paper') {
      result = 'You win.';
    } else if (computerMove === 'scissors') {
      result = 'Tie.';
    }

  } else if (playerMove === 'paper') {
    if (computerMove === 'rock') {
      result = 'You win.';
    } else if (computerMove === 'paper') {
      result = 'Tie.';
    } else if (computerMove === 'scissors') {
      result = 'You lose.';
    }
    
  } else if (playerMove === 'rock') {
    if (computerMove === 'rock') {
      result = 'Tie.';
    } else if (computerMove === 'paper') {
      result = 'You lose.';
    } else if (computerMove === 'scissors') {
      result = 'You win.';
    }
  }

  if (result === 'You win.') {
    score.wins += 1;
  } else if (result === 'You lose.') {
    score.losses += 1;
  } else if (result === 'Tie.') {
    score.ties += 1;
  }

  localStorage.setItem('score', JSON.stringify(score));

  updateScoreElement();

  document.querySelector('.js-result').innerHTML = result;

  document.querySelector('.js-moves').innerHTML = `You
<img src="images/${playerMove}-emoji.png" class="move-icon">
<img src="images/${computerMove}-emoji.png" class="move-icon">
Computer`;
}

function updateScoreElement() {
  document.querySelector('.js-score')
    .innerHTML = `Wins: ${score.wins}, Losses: ${score.losses}, Ties: ${score.ties}`;
}

function pickComputerMove() {
  const randomNumber = Math.random();

  let computerMove = '';

  if (randomNumber >= 0 && randomNumber < 1 / 3) {
    computerMove = 'rock';
  } else if (randomNumber >= 1 / 3 && randomNumber < 2 / 3) {
    computerMove = 'paper';
  } else if (randomNumber >= 2 / 3 && randomNumber < 1) {
    computerMove = 'scissors';
  }

  return computerMove;
}

// Solution for 12v.
function resetScore() {
  score.wins = 0;
  score.losses = 0;
  score.ties = 0;
  localStorage.removeItem('score');
  updateScoreElement();
}

// Solution for 12v.
document.querySelector('.js-reset-score-button')
  .addEventListener('click', () => {
    // Solution for 12v.
    // resetScore();

    // Solution for 12x.
    showResetConfirmation();
  });

// Solution for 12x.
function showResetConfirmation() {
  document.querySelector('.js-reset-confirmation')
    .innerHTML = `
      Are you sure you want to reset the score?
      <button class="js-reset-confirm-yes reset-confirm-button">
        Yes
      </button>
      <button class="js-reset-confirm-no reset-confirm-button">
        No
      </button>
    `;
  
  document.querySelector('.js-reset-confirm-yes')
    .addEventListener('click', () => {
      resetScore();
      hideResetConfirmation();
    });
  
  document.querySelector('.js-reset-confirm-no')
    .addEventListener('click', () => {
      hideResetConfirmation();
    });
}

function hideResetConfirmation() {
  document.querySelector('.js-reset-confirmation')
    .innerHTML = '';
}
```
- 12s html
```html
<!--
  Remove onclick="" from the Auto Play button.
  And add class="js-auto-play-button" so we can
  select it in JavaScript and use .addEventListener()
  See 12r.html for the full code.
-->
<button class="auto-play-button js-auto-play-button">
  Auto Play
</button>
```
- 12s css
```
```
- 12s js
```js
/*
  Get the auto play button using the DOM and
  use .addEventListener()
  See 12r.js for the full code.
*/
document.querySelector('.js-auto-play-button')
  .addEventListener('click', () => {
    autoPlay();
  });
```
- 12t js
```js
// See 12r.js for the full code.
function autoPlay() {
  if (!isAutoPlaying) {
    intervalId = setInterval(() => {
      const playerMove = pickComputerMove();
      playGame(playerMove);
    }, 1000);
    isAutoPlaying = true;
    
    // When the game is auto playing, change
    // the text in the button to 'Stop Playing'.
    document.querySelector('.js-auto-play-button')
      .innerHTML = 'Stop Playing';

  } else {
    clearInterval(intervalId);
    isAutoPlaying = false;

    // When the game is not playing, change
    // the text back to 'Auto Play'.
    document.querySelector('.js-auto-play-button')
      .innerHTML = 'Auto Play';
  }
}
```
- 12u js
```js
// See 12r.js for the full code.
document.body.addEventListener('keydown', (event) => {
  if (event.key === 'r') {
    playGame('rock');
  } else if (event.key === 'p') {
    playGame('paper');
  } else if (event.key === 's') {
    playGame('scissors');
  
  // Add an if-statement condition to
  // check if 'a' was pressed.
  } else if (event.key === 'a') {
    autoPlay();
  }
});
```
- 12v html
```html
<!--
  Remove onclick="" from the Reset Score button
  and use .addEventListener instead.
  See 12r.html for the full code.
-->
<button class="reset-score-button js-reset-score-button">
  Reset Score
</button>
```
- 12v js
```js
// Create a new resetScore function so
// we can reuse this code.
// See 12r.js for the full code.
function resetScore() {
  score.wins = 0;
  score.losses = 0;
  score.ties = 0;
  localStorage.removeItem('score');
  updateScoreElement();
}

// Add an event listener for the reset score
// button using .addEventListener
document.querySelector('.js-reset-score-button')
  .addEventListener('click', () => {
    resetScore();
  });
```
- 12w js
```js
// See 12r.js for the full code.
document.body.addEventListener('keydown', (event) => {
  if (event.key === 'r') {
    playGame('rock');
  } else if (event.key === 'p') {
    playGame('paper');
  } else if (event.key === 's') {
    playGame('scissors');
  } else if (event.key === 'a') {
    autoPlay();
  
  // Add an if-statement condition to
  // check if 'Backspace' was pressed.
  } else if (event.key === 'Backspace') {
    resetScore();
  }
});
```
- 12x html
```html
<!--
  Add an element for displaying the
  confirmation message.
  See 12r.html for the full code.
-->
<p class="js-reset-confirmation"></p>
```
- 12x css
```css
/* See 12r.css for the full code. */
.reset-score-button,
.auto-play-button,
/*
  Reuse the style for the reset-score-button
  by using a comma in the selector.
*/
.reset-confirm-button {
  background-color: white;
  border: none;
  font-size: 15px;
  padding: 8px 15px;
  cursor: pointer;
}

/*
  Add extra margin to the confirm buttons.
  In CSS, we can add multiple sets of styles
  to the same class. Styles written later
  will override styles written before.
*/
.reset-confirm-button {
  margin-left: 10px;
}
```
- 12x js
```js
// Below are 3 parts that need to be
// changed in the JavaScript code for
// this exercise.
// See 12r.js for the full code.
document.body.addEventListener('keydown', (event) => {
  if (event.key === 'r') {
    playGame('rock');
  } else if (event.key === 'p') {
    playGame('paper');
  } else if (event.key === 's') {
    playGame('scissors');
  } else if (event.key === 'a') {
    autoPlay();

  } else if (event.key === 'Backspace') {
    // Update 'Backspace' to show the
    // confirmation message instead of
    // resetting the score immediately.
    showResetConfirmation();
  }
});

document.querySelector('.js-reset-score-button')
  .addEventListener('click', () => {
    // Update the click event listener to
    // show the confirmation message instead
    // of restting the score immediately.
    showResetConfirmation();
  });

// Function for showing the confirmation message.
function showResetConfirmation() {
  document.querySelector('.js-reset-confirmation')
    .innerHTML = `
      Are you sure you want to reset the score?
      <button class="js-reset-confirm-yes reset-confirm-button">
        Yes
      </button>
      <button class="js-reset-confirm-no reset-confirm-button">
        No
      </button>
    `;
  
  // You could use onclick="..." in the HTML above,
  // but it's recommended to use .addEventListener()
  document.querySelector('.js-reset-confirm-yes')
    .addEventListener('click', () => {
      resetScore();
      hideResetConfirmation();
    });
  
  document.querySelector('.js-reset-confirm-no')
    .addEventListener('click', () => {
      hideResetConfirmation();
    });
}

// A helper function (it helps us reuse the
// code for hiding the confirmation message).
function hideResetConfirmation() {
  document.querySelector('.js-reset-confirmation')
    .innerHTML = '';
}
```








