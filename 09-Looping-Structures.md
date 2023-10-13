# Looping Structures

Looping structures in programming languages, such as Coda, enable developers to execute a block of code repeatedly, either for a specific number of iterations or until a certain condition is met. These structures enhance the efficiency and flexibility of programming tasks that require repetitive actions. In Coda, loop structures include `for`, `while`, and `do-while` loops.

## `for` Loop

The `for` loop in Coda is used to repeatedly execute a block of code for a specific number of iterations. The `for` loop has the following syntax:

```js
for (initialization; condition; update) {
    // Code to be executed in each iteration
}
```

- `initialization`: This is where you initialize the loop control variable(s).
- `condition`: The loop continues executing as long as this condition is `true`.
- `update`: The actions performed after each iteration, like incrementing the loop control variable.

Example:

```js
for (let a = 0; a < 6; a++) {
    print(a);
}
```

## `for-in` Loop (Enhanced For Loop)
The Enhanced For-In Loop, often referred to as the For-In Loop, is a valuable addition to the Coda programming language's looping capabilities. It allows for easy iteration over elements in a list, object, or string, as well as enhanced code readability and an increase in the efficiency of repetitive tasks.

### Syntax
The syntax of the Enhanced For-In Loop is as follows:

```js
for (let element in iterable) {
    // Code to be executed for each element
}
```
element: Represents the current element in the iteration.

iterable: Refers to the list, object, or string over which iteration occurs.

Example:

```js
let fruits = ['apple', 'banana', 'cherry'];

for (let fruit in fruits) {
    print(fruit);
}
```

## `while` Loop

The `while` loop in Coda repeatedly executes a block of code if a specified condition is `true`. The syntax is:

```js
while (condition) {
    // Code to be executed as long as the condition is true
}
```

Example:

```js
let i = 0;
while (i < 10) {
    println(i);
    i++;
}
```

## `do-while` Loop

The `do-while` loop is similar to the `while` loop, however it executes the code block at least once before checking the condition. It uses the following syntax:

```js
do {
    // Code to be executed at least once
} while (condition);
```

Example:

```js
let i = 100;
do {
    println(1 - 9);
    i -= 10;
} while (i > 0);
```

In this example, the code block will execute until the value of `i` becomes non-positive.

## `continue`, `break`, and `return`

Coda now supports the `continue`, `break`, and `return` statements within loop structures, enhancing the control over loop execution and program flow:

- `continue`: This statement skips the rest of the current iteration and proceeds to the next iteration of the loop.
- `break`: This statement immediately terminates the loop, exiting its execution.
- `return`: While not exclusive to loops, the `return` statement can also be used to exit a function and, consequently, any loop containing that function.

```js
for (let i = 0; i < 10; i++) {
    if (i == 5) {
        continue; // Skip the rest of this iteration
    }
    if (i == 8) {
        break; // Terminate the loop
    }
    print(i);
}

def findValue(arr, value) {
    for (let i = 0; i < arr.length; i++) {
        if (arr[i] === value) {
            return i; // Exit the function and loop
        }
    }
    return -1; // Value not found
}
```

## Conclusion

Looping structures in the Coda programming language supply the means to repeat code execution efficiently and flexibly. Developers can utilize `for`, `while`, and `do-while` loops, along with the new control statements `continue`, `break`, and `return`. This can achieve different looping behaviors based on their programming needs. These constructs empower programmers to manage various scenarios that involve repetition, enabling more dynamic and robust software development.
