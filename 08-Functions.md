# Functions: Architects of Logic

In the realm of Coda, functions stand as the architects of logic, meticulously crafting sequences of actions to execute at your command. Much akin to their Python counterparts, Coda functions possess a distinctive elegance in their creation and execution.

## Function Creation
To summon forth a function, the `def` keyword serves as your incantation. Functions are born like any other variable, yet their purpose is imbued within the intricate dance of expressions that follow.

```py
def add(x, y) {
    return x + y;
}
```

## Function Invocation
Unlocking the potential of functions is achieved through the invocation ritual, signaled by the `()` operator. By uttering the function's name within these parentheses, you beckon its execution.

```py
add(5, 5);
```

## Function Assignment
In the realm of functions, the boundaries between variables and functions blur. Functions, too, can take residence within variables, just as any other entity. Such assignments harness the power of functions for further manipulation.

```py
def add(x, y) {
    return x + y;
}

x = add;
k = x(5, 5);
print(k);
```

## Functions in Objects
The union of functions and objects yields an enchanting synergy. Functions become integral to objects, a key to unlocking their potential. As you define functions within objects, the function's name assumes the role of a key, ushering you into a world of structured logic.

```py
let hello = {
    something: def(name){
        println("Hello, " + name + "!");
    },
    earth: def(){
        println("Hello, Earth!");
    }
};
```

## Interaction and Expression
Coda's functions extend an invitation to interaction and expression. As you summon the function's essence with precise parameters, the symphony of actions orchestrated within unfolds, crafting an elegantly choreographed sequence of events.

```py
let inp = input("What is your name? ");
hello.something("World");
hello.earth();
hello.something(inp);
```

## Explicit Return
In the art of function crafting, a distinctive feature emerges: the last executed statement within a function is no longer automatically returned by default. Instead, you can use the `return` keyword to explicitly specify the value to be returned.

```py
def multiply(x, y) {
    return x * y;
}
```

In the world of Coda, functions stand not as mere tools, but as the artisans of your programming tapestry. Their creation, invocation, and integration within objects mark a journey into the realm of structured logic, weaving a narrative of precision and expression.