# Import Statements in Coda

In the Coda programming language, import statements provide a convenient way to include the contents of other files within your code. Similar to the `#include` directive in C++, import statements allow you to reuse code and organize your projects more efficiently. When you use an import statement, the contents of the imported file are essentially copied and pasted in place of the statement. This enables you to build modular and maintainable codebases by splitting your code into smaller, reusable units.

## Basic Syntax

The basic syntax for using an import statement in Coda is as follows:

```js
import folder.file
import folder.subfolder.file
```

Here, `folder` represents the directory path where the file is located, and `file` is the name of the file you want to import. You can use import statement to include code from other file without the need to explicitly copy and paste the content. This not only save you time but also help you avoid redundancy and keep your codebase more organized.

## Usage and Examples

### Example 1: Reusing Code

So like any other language, in which you make functions which can be used later here you can do that with import statements.

```js
// math.coda
def add(a, b) {
    return a + b;
}

def subtract(a, b) {
    return a - b;
}
```

Now, you can import and use these functions in another file:
Refer to the example given below

```js
import math

let result = add(5, 3);
print(result); // Output: 8
```

### Example 2: Organizing Codebase

In larger project, you might have multiple files that are part of different modules. Using import statements, you can create a more structured codebase:

```js
// geometry.coda
def calculateArea(radius) {
    return 3.14 * radius * radius;
}
```

```js
// main.coda
import geometry

let circleArea = calculateArea(5);
print(circleArea); // Output: 78.5
```

### Example 3: Managing Configuration

You can use import statements to manage configuration setting or constants in a centralized file:

```js
// config.coda
const API_URL = "https://api.example.com";
const API_KEY = "your-api-key";
```

```js
// api.coda
import config

def fetchData(endpoint) {
    let url = API_URL + endpoint;
    // ... rest of the code
}
```

## Import Behavior

It's important to note that when you use the import statement, the content of the imported file are effectively copied and inserted at the location of the statement. This can lead to potential issues, such as circular dependencies, if not managed carefully.

## Conclusion
Coda's approach is quite different from traditional programming languages, but it's designed to be user-friendly and accessible for a wide range of users, even those without a programming background. It leverages the document-based structure to manage data and automate tasks.
Import statements in Coda provide a powerful mechanism for code reuse, organization, and modularization. By including the contents of other files seamlessly, you can create more maintainable and structured codebases. Whether you're reusing utility functions, managing configuration settings, or organizing your project into meaningful modules, import statements offer a versatile tool for enhancing your code's readability and maintainability.
