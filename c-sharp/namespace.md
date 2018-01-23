# Namespace, Class and Methods

#### Today I learned a good analogy for describing Namespace, Classes and Methods...

If you new to C# or forgotten the difference between namespaces, classes and methods, here is a handy analogy.

- Like an address, method name is the street address, class name is the city and namespace is the state.


#### A few more notes

- Namespaces, Classes and Methods organize code in C#
- Reading a Method call from right to left: Namespace.Class.Method
- For System.Console.write:
  - The method name is "write"
  - The class name is "Console"
  - System is the namespace containing the class Console
- Classes are contained in namespaces
- Namespaces make it possible to have multiple classes with the same name because each class name remains in the namespace
- Put the Class Program in the namespace NASA...
- Namespaces can have multiple levels such as company name, then partition the namespace into smaller namespaces by dots (.), eg NASA.Planets.Saturn
- A Using Directive reduces typing and makes the code more readable.
- A "Using Directive" reduces constant writing out of the namespace by putthing the namespace at the top of the code page, ```using System;```
- Place as many Using Directives as needed at the top of the code page.

```cs
namespace Nasa
{
  class Planets
  {
    ...
  }
}
```
