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
