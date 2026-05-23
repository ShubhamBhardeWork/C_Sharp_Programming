# C# Programming Language

## Pre-Requisites:-
1. Code Editor
    1. Visual Studio
    1. VS Code

1. Compiler / Interpreter
    1. Download & Install dotnet sdk & dotnet runtime from browser. 


## Data types:-
- It defines what kind of value a variable can store.

1. byte  => 1 byte
1. short => 2 bytes
1. int => 4 bytes
1. float => 4 bytes
1. long => 8 bytes
1. double => 8 bytes
1. decimal => 16 bytes
1. bool => 1 byte
1. char => 2 bytes
1. string => 2 bytes each character
1. array 
1. class
1. interface
1. object
1. delegate
1. list
1. dictionary
1. hashset
1. arraylist
1. stack
1. queue
1. enum
1. struct

## Main Types of Data Types:-
1. Value Type
1. Reference Type

### Value Type:-
- Stores actual value directly.
- Generally faster access than reference types.
- Can not store `null` by default.
- Memory is allocated directly for value.

- Examples:-
    1. byte
    1. short
    1. int
    1. float
    1. long
    1. double
    1. decimal
    1. char
    1. bool
    1. struct
    1. enum

### Reference Type:-
- Stores reference or memory address of object.
- Objects are generally stored in heap memory.
- Can store `null` value.
- Slightly slower than value types because reference lookup is needed.
- Examples:-
    1. string
    1. array
    1. class
    1. object
    1. interface
    1. list
    1. dictionary
    1. arraylist
    1. linkedlist
    1. hashset
    1. stack
    1. queue
    1. delegate
        

## Comment:-
- Comments are ignored by compiler.
- Comments are never executed.
- Comments are used to improve code readability and explain logic.
- Good comments explain "why" not "what".


### Types of comment:-
1. Single-line comment
1. Multi-line comment

```cs
// this is single line comment

/* this  is 
           multi line
        comment
*/
```


## Token:-
It is the smallest individual unit/element of a program.

### Types of Tokens:-
1. Identifiers
1. Keywords
1. Constants/Literals
1. Operators
1. Separators/Special Symbols


## Identifier:-
- It is a name used to identify:-
    1. Variables
    1. Functions/Methods
    1. Classes
    1. Objects
    1. Namespaces

```cs
int age = 21;
// here age is an Identifier
```
