# Easy C# Compiling With Mono Software


_Today I learn the Mono compiler makes it easy to quickly run C# programs._

- Mono is an open-source implementation of .NET libraries and enables cross-platform compatible tools. It is ECMA compatible and provides .NET framework to the Linux environment.
Mono is developed by Xamarin and .NET Foundation

- Once you download Mono, two commands get your C# code compiled and running.

## Compile a C# Console Program
### SETUP
- Download [Mono](http://www.Mono-project.com/) and install it.
- Create a C# ".cs" file or copy the below code into a hello-world.cs 

```cs
    public class HelloWorld
    {
        static public void Main ()
        {
            Console.WriteLine ("Hello Mono World");
        }
    }
```

### COMPILE & RUN
- Open the Mono Command Prompt and change directory to your project folder

#### Compile
- To Compile, run "MCS filename" in the Mono Command Prompt

```
mcs hello-world.cs
```
- RESULT: the file hello-world.exe is created

#### Run your program
- In the Mono command prompt, run "Mono hello-world.exe"
```cs
  Mono hello-world.exe
```
- RESULT: your C# program runs and you get rich and famous.

## TL;DR
- Mono is a fast cross-platform framework that compiles C# with minimal configuration.
- It provides an open-source version of the .NET which is also compatible with Linux



-------------------------------------------------------

## REFERENCES 
- [Mono Project](http://www.Mono-project.com/)
- [Wikipedia: Mono](https://en.wikipedia.org/wiki/Mono_%28software%29)
- [Difference between .NET and Mono](https://stackoverflow.com/questions/37738106/net-core-vs-Mono)
- [Mono, An Alternative to .NET](https://www.codeproject.com/Articles/13434/Mono-an-alternative-for-the-NET-framework)


