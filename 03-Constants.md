# Constants

In simple terms, a constant is something that doesn't change. It is like a fixed value that stays the same no matter what. Think of a number of days in a week - it's always 7! (And weekend has always only 2 days, unfortunately)

One example of a constant in nature is the speed of light. The speed of light in a vacuum is about 299,792 kilometers per second (or about 186,282 miles per second). This means that light always travels at this speed, and it never changes.

An analogy that could help you understand constants is a faucet. When you turn on a faucet, the water flow can be adjusted from a tiny drip to a steady stream. In this case, the water pressure can be considered a variable because it can change. However, the temperature of the water coming out of the faucet can be considered a constant because it remains the same (for example, warm or cold) regardless of the water pressure.

So, a constant is something that doesn't change, like the speed of light or the temperature of water from a faucet.

## Declaration of Constants

Much like variables, constants hold a prominent place in Coda's syntax. To declare a constant, you can rely on the `const` keyword. This serves as a clear indicator that the value you assign is intended to remain unchanged.
You can assign any type of value to `const` variable - numeric, text or boolean.

```js
const pi = 3.14159265359;
const firstMonth = "JANUARY";
const isTrue = true;
```

## Consistency with Flexibility

The most important thing to remember about contants is that **they cannot be changed**. Once you assign a value to your constant, you will never be able to reassign.

In programming, such property is called `immutability`. For example, the genetic code of an individual is immutable. This means that the DNA sequence that makes up your genes cannot be changed. It is the blueprint that determines your physical characteristics, and it cannot be altered.

```js
const pi = 3.14159265359;
pi = 10; // This will result in an error, rightly!
```

## The Symphony of Properties

In a harmonious convergence, constants align with variables in their essence. Types, expressions, and all the facets you appreciate about variables are seamlessly woven into the fabric of constants. This consistency simplifies your coding experience and streamlines your understanding of these foundational elements.

The constants are immutable, but not immune to the allure of types and the captivating dance of expressions.

In other words, you can treat `const` as other Coda variables - just the special ones. You will soon notice how great they are!
