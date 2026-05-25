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


## Variable:-
- It is name given to memory location which acts as a container for storing data.

```cs
dataType variableName = value; 

// example
int age = 21;
```

### Variable Declaration:-
- Creating a variable without assigning a value.

```cs
int age;
```

### Variable Initialization:-
- Assigning a value to an already declared variable.

```cs
age = 21;
```

### Variable Declaration & Initialization
- Declaring and assigning a value at the same time.

```cs
int age = 21;
```

### Types of Variable:-
1. Local Variable
1. Global Variable
1. Instance Variable
1. Static Variable

```NOTE:- C# does not directly support true global variables.```

### Naming Conventions for variable:- 
1. First character must be start from alphabat or `$` or `_`.
1. It can't start with a number.
1. White spaces are not allowed
1. Special symbols are not allowed other than `$`, `_`.
1. Reserved keywords are not allowed.
1. Variable names should be meaningful & descriptive.
1. C# is case sensitive. It treats uppercase & lowercase letters differently. 


## Constant:-
- It is a value that can't be change during program execution.

```cs
const float PI = 3.14f;
const string MyName = "Shubham Bharde"; 
```


## Keyword:-
- It is reserved words whose meaning is already known by the compiler.

- examples:- 

    ``` int , float, string, if, else, break, continue, for, while, do, return, class, public, private, protected, enum  etc.``` 


## Statement:-
- It is a single executable instruction/line of code. 

- Statements are executed one by one during program execution.

- Most statements are terminated by (`;`).

```cs
int age = 21; // statement

age++; // statement
Console.WriteLine("Age is:- " + age); // statement
```

### Types of Statements:-
1. Declaration Statement
1. Assignment Statement
1. Conditional Statement
1. Looping Statement
1. Jump Statement


## Expression:-
- It is a combination of operands and operators that produces a value/result.

```cs
10 + 20; // expression
 
age > 18; // expression

num1 + num2; // expression
```


## Statement vs Expression:-
- Expression produces a value.
- Statement performs an action.

```cs
10 + 20 // expression

int age = 21; // statement
```


## Operators:-
- It is a symbol that performs some operation on operands.

### Types of Operators:-
1. Arithmetic Operators:-
    - ```[+, -, *, /, %]```
    - `% :- returns remainder`

1. Assignment Operators:-
    - ```[=, +=, -=, *=, /=, %= ]```

1. Relational/Comparison Operators:-
    - ```[<, >, <=, >=, ==, !=]```

1. Logical Operators:-
    - ```[&&, ||, !]```

1. Bitwise Operators:-
    - ```[&, |, ^, ~, <<, >>]```

1. Increment / Decrement Operators:-
    - ```[++, --]```

1. String Operator:- used for string concatenation.
    - ```[+]```

1. Ternary Operator (?:):-
    - ```[condition ? true : false]```


## Type Casting/Conversion:-
- It is the process of converting one type into another type.

### Types of Type Casting:-
1. Implicit Type Casting
1. Explicit Type Casting

### Implicit Casting:-
- Automatically converts smaller datatype into larger datatype.

```cs
int num = 10;
double d = num;
```

### Explicit Casting:-
- Manually converts larger datatype into smaller datatype.

```cs
double d = 10.5;
int num = (int)d;
```

### Type Conversion Methods:-
1. Convert.ToByte()
1. Convert.ToInt16()
1. Convert.ToInt32()
1. Convert.ToInt64()
1. Convert.ToSingle()
1. Convert.ToDouble()
1. Convert.ToDecimal()
1. Convert.ToBoolean()
1. Convert.ToChar()
1. Convert.ToString()

## Taking Input from User:-
- Console.ReadLine();

```cs
Console.Write("Enter Your Name:- ");
string name = Console.ReadLine();

Console.Write("Enter Your Age:- ");
int age = int.Parse(Console.ReadLine());

Console.Write("Enter Your Standard:- ");
int standard = Convert.ToInt32(Console.ReadLine());
```


## Print/Display Output on Console/Screen:-
- Console.WriteLine();

```cs
// prints output on same line.
Console.Write("Hello World."); 

// prints output and moves cursor to next line.
Console.WriteLine("Hello Coders.");
```