# List

## List:-
- It is a collection of elements of the same type.

- Flexible size & It can grow or shrink dynamically.

- Supports index based access.

- List is mutable, meaning we can perform update & deletion operations on it.

- Stores elements in contiguous memory locations internally.

- It is available in `System.Collections.Generic` namespace.
 
#### NOTE:-
```Internally List<T> uses an array. When capacity becomes full, it creates a new larger array and copies existing elements into it.```


## List Methods:-
1. .Count
1. .Add(element)
1. .AddRange(collection / IEnumerable<T>)
1. .Remove(element)
1. .RemoveAt(index)
1. .Insert(index, element)
1. .Contains(element)
1. .IndexOf(element)
1. .Find(predicate)
1. .FindAll(predicate)
1. .Clear()
1. .Reverse()
1. .Sort() 

1. .Exists(predicate)
1. .RemoveAll(predicate)
1. .RemoveRange(index, count)

```Predicate is a method/function that returns a boolean value (true or false) based on a condition.```


## Hands-on:-
```cs
// Empty list
var emptyList = new List<string>();

var numbers = new List<int>{1, 2, 3, 4};
var friends = new List<string>
{"Pranav", "Akshay", "Rahul", "Rohit"};

Console.WriteLine($"Total Friends:- {friends.Count}");

// Add element
friends.Add("Gaurav");

// Remove element
friends.Remove("Gaurav");

// Remove element at specific given index
friends.RemoveAt(2); 

// Insert element at specific given index
friends.Insert(2, "Rahul");

// Checks whether element exists or not
var isExisted = friends.Contains("Akshay");
Console.WriteLine($"Akshay exists:- {isExisted}");

// Find first matching element (based on condition)
friends.Find(n => n == "Rahul");

// Find all matching elements (Filter based on condition)
friends.FindAll(n => n.StartsWith('r'));
friends.FindAll(n => n.StartsWith("n", StringComparison.OrdinalIgnoreCase));

// Reverse (reversed original list)
numbers.Reverse();

// Sort (sorted original list)
numbers.Sort();
friends.Sort();


// Iterate over a friends(string) list
Console.WriteLine("Iterate over a friends list:- ");
foreach(var friend in friends)
{
    Console.WriteLine(friend);
}

// Clear the list
numbers.Clear();
```