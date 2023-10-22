# Built-in Functions: Tools of Mastery

In the expansive landscape of Coda, a treasure trove of built-in functions awaits your command, poised to simplify your coding journey. These functions are expertly designed to perform common tasks, enhancing your productivity and making your code dance with elegance.

## `print(...)`
This foundational function serves as your conduit to the digital realm, allowing you to display text and variables on the screen. It accepts any number of parameters, separating them with a space for a seamless display.

```js
print("Hello, World!", "Chaining")
```

## `println(...)`
For a touch of refinement, `println(...)` not only prints the provided text and variables but also gracefully advances the cursor to the next line, ensuring a cleaner and organized output.

```js
println("Hello, World!", "Chaining")
```

## `sleep(sec)`
In the realm of time manipulation, `sleep(...)` holds the key to pause. This function takes a single parameter – the duration in seconds and beckons your program to await the passage of time.

```js
sleep(20)
```

## `parseInt(string)`, `parseFloat(string)`, `parseDouble(string)`, `parseByte(string)`, `parseBool(string)`
The family of parsing functions are your navigators through string-to-number and string-to-boolean conversions. Each function accepts a single parameter – the 'string' to be converted – and return its numerical or boolean equivalent.
As in parseInt(string)- convert string to int
parseFloat() - convert string to float
parseDouble()- convert string to double
parseByte()- convert string to bytes
parseBool()- convert string to bool

```js
let num = parseInt("20")
```

## `quit(int statusCode)`, `exit(int statusCode)`
In the realm of controlled departure, `quit()` and `exit(...)` offer ways to gracefully bid farewell to your program. Both serve the same purpose.
In simple terms, it end's the program.

## `input(prompt)`
The gateway to user interaction, `input(...)` prompt users for input. A single parameter – the prompt you wish to display – guides the user in providing their response.
In simple terms, it takes the input from users whatever it is, number, string, bool or anything.

```js
let numStr = input("Enter a number")
```

In your quest to master Coda, these built-in functions serve as your loyal companions, simplifying common tasks and illuminating the path ahead. With parameters tailored to each function's unique purpose, you hold the key to a world of efficiency and expressiveness.
