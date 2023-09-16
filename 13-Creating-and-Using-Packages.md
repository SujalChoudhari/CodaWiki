Packages in Coda provide a convenient way to organize and reuse code. They allow you to encapsulate related functionality and share it across your projects. In Coda, packages can take two forms: `.coda` packages and `.dll` (Dynamic Link Library) packages. This wiki page will explain how to use and implement packages in Coda.

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

### Using a .coda Package

To use a `.coda` package within your Coda project, you can simply import the respective `.coda` file:

```js
import Maths;

let result = Maths.add(5, 3); // Calls the 'add' function from the Maths package
```

## .dll Packages

### Creating a .dll Package

`.dll` packages are compiled dynamic link libraries containing reusable code. These packages may also include a `.coda` file for documenting the package's functionality. To create a `.dll` package:

1. Compile your code into a `.dll` file (e.g., `Maths.dll`) using the appropriate tools for your programming language.
    The source for a DLL file should contain functions with the same signature;
    `extern "C" __declspec(dllexport) void coda_<function_name_goes_here>(IValuePtr res, IValuePtr args, IEnvironment * env);`
    Find the Interfaces in FFI directory of this repo.

2. Create a `.coda` file that describes the package's functions and variables.
```js

scope Maths{
    def add(first, second) {
        return native Maths coda_add(first, second); // native keyword states that the `coda_add` function is defined in Maths.dll file.
    }
```

### Using a .dll Package

To use a `.dll` package, you'll need to import the corresponding `.coda` file and make sure the `.dll` file is in the same directory as your executable files.

```js
import Maths;

let result = Maths.sqrt(23); // Calls the 'sqrt' function from the Maths.coda which calls `coda_sqrt` from the Maths.dll
```

## Directory Organization

When working with packages, remember to keep the `.coda` and `.dll` files organized. If it's a `.coda` package, place it in your source code directory. For `.dll` packages, ensure the `.dll` file is located in the same directory as your Coda executable files.

Packages in Coda provide a clean and modular way to manage your code, facilitating code reuse and organization in your projects.