# C# Specific Concepts

## Range of Data Types:-
- `MinValue` property returns minimum value a datatype can store.
- `MaxValue` property returns maximum value a datatype can store.

```cs
Console.WriteLine($"Byte Range:- {byte.MinValue} to {byte.MaxValue}");
Console.WriteLine($"Short Range:- {short.MinValue} to {short.MaxValue}");
Console.WriteLine($"Int Range:- {int.MinValue} to {int.MaxValue}");
Console.WriteLine($"Float Range:- {float.MinValue} to {float.MaxValue}");
Console.WriteLine($"Long Range:- {long.MinValue} to {long.MaxValue}");
Console.WriteLine($"Double Range:- {double.MinValue} to {double.MaxValue}");
Console.WriteLine($"Decimal Range:- {decimal.MinValue} to {decimal.MaxValue}");
```


## Var Keyword:-
- `var` is a contextual keyword used to declare implicitly typed local variables.

- Compiler automatically determines datatype at compile time based on assigned value.

- `var` must be initialized during declaration.

- Once datatype is assigned, it cannot be changed.

```cs
var age = 21;         // int
var name = "Shubham"; // string
```

#### NOTE:-
`var` is `not dynamic typing`.
`var` can only be `used for local variables`.