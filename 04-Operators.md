

Operators in the Coda programming language are fundamental symbols used to perform various operations on operands, such as variables, constants, or expressions. Coda supports a wide range of operators to manipulate and work with data effectively. This page provides an overview of the binary, unary, relational, logical operators, as well as assignment operators available in Coda.

## Binary Operators

Binary operators are used to perform operations between two operands. Binary operators take two operands, one on the left and one on the right, and combine them to produce a result. They are called "binary" because they work with two values.

- **Addition (`+`)**: Adds two operands.
- **Subtraction (`-`)**: Subtracts the right operand from the left operand.
- **Multiplication (`*`)**: Multiplies two operands.
- **Division (`/`)**: Divides the left operand by the right operand.
- **Modulus (`%`)**: Returns the remainder of the division between two operands.
- **Increment (`++`)**: Increases the value of the operand by 1.
- **Decrement (`--`)**: Decreases the value of the operand by 1.

## Unary Operators

Unary operators perform operations on a single operand.In simple terms, unary operators work with just one piece of data and perform a specific action on it.

- **Unary Plus (`+`)**: Represents the identity of an operand.
- **Unary Minus (`-`)**: Negates the value of an operand.
- **Logical NOT (`!`)**: Inverts the logical value of an operand.
- **`sizeof`**: Returns the size in bytes of a data type or expression.
- **`typeof`**: Returns the data type of an expression.

## Relational Operators

Relational operators are used to compare two operands. In simple terms, relational operators are symbols used to compare two values and determine the relationship between them. 

- **Greater Than (`>`)**: Checks if the left operand is greater than the right operand.
- **Less Than (`<`)**: Checks if the left operand is less than the right operand.
- **Greater Than or Equal To (`>=`)**: Checks if the left operand is greater than or equal to the right operand.
- **Less Than or Equal To (`<=`)**: Checks if the left operand is less than or equal to the right operand.
- **Equal To (`==`)**: Checks if the operands are equal.
- **Not Equal To (`!=`)**: Checks if the operands are not equal.

## Logical Operators

Logical operators are used to perform logical operations. These operators allow you to combine and manipulate Boolean values to make decisions, control the flow of your program, and create more complex conditions.

- **Logical AND (`&&`)**: Returns `true` if both operands are `true`.
- **Logical OR (`||`)**: Returns `true` if at least one operand is `true`.
  
Boolean expressions can be put between braces ( '(' and ')' ) in order to guide the evaluation order.
The AND and OR expressions are lazy evaluated. This means that the second argument to AND will not be evaluated if the first argument already evaluated to false, and for OR similarly if the first argument already evaluated to true.

## Assignment Operators

Assignment operators are used to assign values to variables.They take a value on the right and store it in a variable on the left.

- **Assignment (`=`)**: Assigns the value of the right operand to the left operand.
- **Addition Assignment (`+=`)**: Adds the right operand to the left operand and assigns the result to the left operand.
- **Subtraction Assignment (`-=`)**: Subtracts the right operand from the left operand and assigns the result to the left operand.
- **Multiplication Assignment (`*=`)**: Multiplies the left operand by the right operand and assigns the result to the left operand.
- **Division Assignment (`/=`)**: Divides the left operand by the right operand and assigns the result to the left operand.

## Example
```js
let a = 10;
let b = 5;
let c = 3;

// Binary Operators
let additionResult = a + b;       // 10 + 5 = 15
let subtractionResult = a - b;    // 10 - 5 = 5
let multiplicationResult = a * b; // 10 * 5 = 50
let divisionResult = a / b;       // 10 / 5 = 2
let modulusResult = a % b;        // 10 % 5 = 0
let postIncrement = c++;          // c = 3 (post-increment)
let preDecrement = --c;           // c = 2 (pre-decrement)

// Unary Operators
let unaryPlus = +a;               // 10 (identity)
let unaryMinus = -b;              // -5 (negation)
let logicalNot = !true;           // false (logical NOT)
let sizeOfA = sizeof(a);          // sizeof int (depends on system)
let typeOfA = typeof(a);          // int (data type of 'a')

// Relational Operators
let greaterThan = a > b;          // true (10 is greater than 5)
let lessThan = b < c;             // false (5 is not less than 3)
let greaterThanOrEqual = a >= b;  // true (10 is greater than or equal to 5)
let equalTo = a == c;             // false (10 is not equal to 3)
let notEqualTo = b != c;          // true (5 is not equal to 3)

// Logical Operators
let logicalAnd = greaterThan && lessThan;  // false (true && false = false)
let logicalOr = greaterThan || lessThan;    // true (true || false = true)

// Assignment Operators
let assignment = 7;
assignment += 3;                 // assignment = 10 (7 + 3)
assignment -= 2;                 // assignment = 8 (10 - 2)
assignment *= 5;                 // assignment = 40 (8 * 5)
assignment /= 4;                 // assignment = 10 (40 / 4)

// Output results
println(additionResult);
println(subtractionResult);
println(multiplicationResult);
println(divisionResult);
println(modulusResult);
println(postIncrement);
println(preDecrement);
println(unaryPlus);
println(unaryMinus);
println(logicalNot);
println(sizeOfA);
println(typeOfA);
println(greaterThan);
println(lessThan);
println(greaterThanOrEqual);
println(equalTo);
println(notEqualTo);
println(logicalAnd);
println(logicalOr);
println(assignment);
```
