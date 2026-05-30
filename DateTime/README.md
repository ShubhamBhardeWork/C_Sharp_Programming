# DateTime

## DateTime:-
- DateTime is used to represent dates and times in C#.

- `DateTime` is a `value type (struct)` provided by the `System` namespace.

- `DateTime is immutable`, meaning once created it cannot be modified/updated.

- Methods such as AddDays(), AddMonths(), AddYears(), AddHours(), and AddMinutes() return a new DateTime instance instead of modifying the existing one.

- It is commonly `used for scheduling, logging, timestamps, and date/time calculations`.


## DateTime Properties:-
### DateTime Static Properties (Type level):-
1. DateTime.Now  
    - Returns the current local date and time.

1. DateTime.UtcNow  
    - Returns the current UTC date and time.

1. DateTime.Today  
    - Returns the current date with the time set to 00:00:00.

### DateTime Instance Properties (Object level):-
1. .Date
    - Returns a new DateTime containing only the date part (time = 00:00:00)

1. .Day  
    - Gets the day of the month.

1. .Month  
    - Gets the month.

1. .Year  
    - Gets the year.

1. .Hour  
    - Gets the hour component.

1. .Minute  
    - Gets the minute component.

1. .Second  
    - Gets the second component.

