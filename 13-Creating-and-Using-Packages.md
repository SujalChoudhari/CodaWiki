Coda packaging provides a convenient and efficient means to organize and reuse code. Their functionality allows you to encapsulate related integration and share it across your various projects. In Coda, packages can take one of two formats: `.coda` packages and `.dll` (Dynamic Link Library) packages. This wiki page will explain how to use and implement packages in Coda.

## .coda Packages

### Creating a .coda Package

A `.coda` package consists of a `.coda` file containing a collection of functions and definitions. These packages are easy to create and ideal for encapsulating code within your project. To create a `.coda` package:

1. Create a `.coda` file with a name that reflects the purpose of the package (e.g., `Maths.coda`).

2. Define your functions and variables within the `.coda` file.

Example (.coda file - `Maths.coda`):

```js
scope Maths {
    def add(first, second) {
        return first + second;
    }
}

```

### How to use a .coda Package

To integrate a `.coda` package within your Coda project, simply import the respective `.coda` file as shown below:

```js
import Maths;

let result = Maths.add(5, 3); // Calls the 'add' function from the Maths package
```

## .dll Packages

### Creating a .dll Package

`.dll` packages are compiled dynamic link libraries which contain reusable code. These packages may also include a `.coda` file for documenting the package's functionality. To create a `.dll` package:

1. Compile your code into a `.dll` file (e.g., `Maths.dll`) using the appropriate tools for your programming language.
    The source for a DLL file should contain functions with the same signature;
    `extern "C" __declspec(dllexport) void coda_<function_name_goes_here>(IValuePtr res, IValuePtr args, IEnvironment * env);`
    (You may find the Interfaces in the FFI directory of this repo).

2. Create a `.coda` file that describes the package's functions and variables.
```js

scope Maths{
    def add(first, second) {
        return native Maths coda_add(first, second); // native keyword states that the `coda_add` function is defined in Maths.dll file.
    }
```

### How to use a .dll Package

To apply a `.dll` package, you will need to import the corresponding `.coda` file and ensure the `.dll` file is located in the same directory as your executable files.

```js
import Maths;

let result = Maths.sqrt(23); // Calls the 'sqrt' function from the Maths.coda which calls `coda_sqrt` from the Maths.dll
```

## Directory Organization

When working with packages, it is important to keep the `.coda` and `.dll` files well organized. For `.coda` packages, place it in your source code directory while for `.dll` packages, ensure the `.dll` file is located in the same directory as your executable Coda files.

In summary, Coda's package sytstem provides a cleanly structured and modular approach to managing your code, facilitating code reuse and efficient organization within your projects.
