

Operators in the Coda programming language are fundamental symbols used to perform various operations on operands, such as variables, constant, or expressions. Coda supports a wide range of operators to manipulate and work with data effectively.An operator in a programming language is a symbol that tells the compiler or interpreter to perform specific mathematical, relational or logical operation and produce final result. This page provides an overview of the binary, unary, relational, logical operators, as well as assignment operators available in Coda.

## Binary Operators
Binary, bi means two. Therefore binary operators are used for performing operations between two operands.

- **Addition (`+`)**: Adds two operands.
- **Subtraction (`-`)**: Subtracts the operand.
- **Multiplication (`*`)**: Multiplies two operands.
- **Division (`/`)**: Divides the operand.
- **Modulus (`%`)**: Returns the remainder of the division between two operands.
- **Increment (`++`)**: Increases the value of the operand by 1.
- **Decrement (`--`)**: Decreases the value of the operand by 1.
- <img width="391" alt="image" src="https://github.com/th-shristi/CodaWiki/assets/119031272/9f131c77-1491-49b0-b024-c63955781f08">

For example- 
```js
let a = 10;
let b = 5;
let c = 3;

let additionResult = a + b;       // 10 + 5 = 15
let subtractionResult = a - b;    // 10 - 5 = 5
let multiplicationResult = a * b; // 10 * 5 = 50
let divisionResult = a / b;       // 10 / 5 = 2
let modulusResult = a % b;        // 10 % 5 = 0
let postIncrement = c++;          // c = 3 (post-increment)
let preDecrement = --c;           // c = 2 (pre-decrement)

OUTPUT

println(additionResult);
println(subtractionResult);
println(multiplicationResult);
println(divisionResult);
println(modulusResult);
println(postIncrement);
println(preDecrement);


## Unary Operators
Unary, uni means one. Unary operations perform operations on single operand.

- **Unary Plus (`+`)**: Represents the identity of an operand.
- **Unary Minus (`-`)**: Negates the value of an operand.
- **Logical NOT (`!`)**: Inverts the logical value of an operand.
- **`sizeof`**: Returns the size in bytes of a data type or expression.
- **`typeof`**: Returns the data type of an expression.

For example- 
```js
let a = 10;
let b = 5;
let c = 3;

let unaryPlus = +a;               // 10 (identity)
let unaryMinus = -b;              // -5 (negation)
let logicalNot = !true;           // false (logical NOT)
let sizeOfA = sizeof(a);          // sizeof int (depends on system)
let typeOfA = typeof(a);          // int (data type of 'a')

OUTPUT

println(unaryPlus);
println(unaryMinus);
println(logicalNot);
println(sizeOfA);
println(typeOfA);

## Relational Operators

Relational operators are used to compare two operands.

- **Greater Than (`>`)**: Checks if the left operand is greater than the right operand.
- **Less Than (`<`)**: Checks if the left operand is less than the right operand.
- **Greater Than or Equal To (`>=`)**: Checks if the left operand is greater than or equal to the right operand.
- **Less Than or Equal To (`<=`)**: Checks if the left operand is less than or equal to the right operand.
- **Equal To (`==`)**: Checks if the operands are equal.
- **Not Equal To (`!=`)**: Checks if the operands are not equal.
<img width="415" alt="image" src="https://github.com/th-shristi/CodaWiki/assets/119031272/beff548d-acf9-45a1-8113-911318752eea">

For example- 
```js
let a = 10;
let b = 5;
let c = 3;

let greaterThan = a > b;          // true (10 is greater than 5)
let lessThan = b < c;             // false (5 is not less than 3)
let greaterThanOrEqual = a >= b;  // true (10 is greater than or equal to 5)
let equalTo = a == c;             // false (10 is not equal to 3)
let notEqualTo = b != c;          // true (5 is not equal to 3)

OUTPUT

println(greaterThan);
println(lessThan);
println(greaterThanOrEqual);
println(equalTo);
println(notEqualTo);

## Logical Operators

Logical operators are used to perform logical operations.

- **Logical AND (`&&`)**: Returns `true` if both operands are `true`.
- **Logical OR (`||`)**: Returns `true` if at least one operand is `true`.
<img width="429" alt="image" src="https://github.com/th-shristi/CodaWiki/assets/119031272/de1bee12-7599-41e8-821f-2ec19560e470">

For example- 
```js
let a = 10;
let b = 5;
let c = 3;

let logicalAnd = greaterThan && lessThan;  // false (true && false = false)
let logicalOr = greaterThan || lessThan;    // true (true || false = true)

OUTPUT

println(logicalAnd);
println(logicalOr);

## Assignment Operators

Assignment operators are used to assign values to variables.

- **Assignment (`=`)**: Assigns the value of the right operand to the left operand.
- **Addition Assignment (`+=`)**: Adds the right operand to the left operand and assigns the result to the left operand.
- **Subtraction Assignment (`-=`)**: Subtracts the right operand from the left operand and assigns the result to the left operand.
- **Multiplication Assignment (`*=`)**: Multiplies the left operand by the right operand and assigns the result to the left operand.
- **Division Assignment (`/=`)**: Divides the left operand by the right operand and assigns the result to the left operand.

For example- 
let assignment = 7;
assignment += 3;                 // assignment = 10 (7 + 3)
assignment -= 2;                 // assignment = 8 (10 - 2)
assignment *= 5;                 // assignment = 40 (8 * 5)
assignment /= 4;                 // assignment = 10 (40 / 4)

OUTPUT

println(assignment);


