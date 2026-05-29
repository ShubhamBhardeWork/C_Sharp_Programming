# Dictionary

## Dictionary:-
- It is a ```collection of key-value pairs```.

- Keys must be unique.

- Provides fast lookup based on keys.

- Supports key-based access using indexer or safer method `TryGetValue()`.

- Average time complexity for insertion, lookup, and deletion is O(1).

- Worst-case time complexity can become O(n) because of hash collisions.

- Dictionary is optimized for fast lookups, not for maintaining sorted order.

- It is available in the `System.Collections.Generic` namespace.

#### NOTE:-
```Internally, Dictionary<TKey, TValue> uses hashing and is implemented using a hash table.```


## Dictionary Methods:-
1. Count
1. Add(key, value)
1. Remove(key)
1. ContainsKey(key)
1. ContainsValue(value)
1. TryGetValue(key, out value)
1. Keys
1. Values
1. Clear()


## Hands-on:-
```cs
// Empty Dictionary
var emptyDictionary = new Dictionary<int, string>();

var phonebooks = new Dictionary<string, long>
{
    {"Shubham", 9166582689},
    {"Mom", 5366893269}
};


Console.WriteLine($"Total Contacts:- {phonebooks.Count}");

// READ
Console.WriteLine($"Mom's number:- {phonebooks["Mom"]}"); // If key does not exist:- throws KeyNotFoundException

// READ (✅ Safe Read using TryGetValue())
if(phonebooks.TryGetValue("Mom", out long momNumber))
{
    Console.WriteLine($"Mom's number:- {momNumber}");
}

// Add
phonebooks.Add("Bhagya", 8255765324);

// Update
if(phonebooks.ContainsKey("Mom"))
{
    phonebooks["Mom"] = 8962651374;
}

// Delete 
phonebooks.Remove("Mom");

// ContainsKey:- Checks whether key exists
bool isKeyExists = phonebooks.ContainsKey("Shubham");
Console.WriteLine($"Shubham key exists:- {isKeyExists}");

// ContainsValue:- Checks whether value exists
bool isValueExists = phonebooks.ContainsValue(9132054568);
Console.WriteLine($"'9132054568' value exists:- {isValueExists}");

// Keys & Values
var phonebookKeys = phonebooks.Keys;
var phonebookValues = phonebooks.Values;

// Iterate over a Phonebook Dictionary
foreach(var contact in phonebooks)
{
    Console.WriteLine($"{contact.Key} ==> {contact.Value}");
}

// Clear dictionary
phonebooks.Clear();
```