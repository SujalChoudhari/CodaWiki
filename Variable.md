# Variables

In the realm of the Coda Programming Language, variables are your dynamic companions, capable of accommodating values of various types. This section will delve into the art of variable declaration, assignment, reassignment, and the intriguing aspect of type specification.

## Variable Declaration and Assignment

When it comes to declaring a variable, the Coda syntax is a symphony of simplicity and clarity. To christen a variable, graciously employ the `let` keyword, gracefully followed by the variable's name and the value it shall embrace.

For instance:

```js
let x = 5
let y = "Hello, World!"
let z = true
```

In the realm of Coda, an intriguing twist awaits. Assignment during declaration is optional, akin to a dance of choice. Should you prefer, the following snippet echoes the same symphony:

```js
let x
x = 5
```

## Reassignment: Embracing Change

Coda's flexibility extends to reassignment, where a variable, much like a chameleon, can gracefully change its attire. Witness this transformation:

```js
let x = 5
x = "Hello, World!"
```

## Assignment without "let": A Subtle Overture

In the annals of Coda, the use of `let` during assignment is both a tradition and a recommendation. However, a subtle choice lies within your grasp:

```js
x = 5
x = "Hello, World!"
```

While the song remains unchanged, the use of `let` adds a touch of elegance to your notation.

## Specifying Types: The Canvas of Clarity

Coda bestows upon you the power to paint clarity with types. Yes, you can express your intent, though not bound by the compiler's scrutiny. A tantalizing taste:

```js
let bool k = true
let string m = "hello"
```

And in a whimsical twist, Coda, ever the accommodating host, welcomes these too:

```js
let bool k = 100
let string m = true
let int i = false
```

While types in Coda may nod to understanding, they dance to the rhythm of possibility.

## Conclusion

In the enchanting realm of Coda, variables are the vessels of versatility. Declare, assign, and let your code flow with the elegance and fluidity that Coda's syntax offers. Whether a tender embrace of types or the grace of unbridled assignments, Coda is your canvas, awaiting your artistic touch.