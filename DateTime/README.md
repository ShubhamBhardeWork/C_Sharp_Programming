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


## DateTime Methods:-
### DateTime Static Methods (Type level):- 
1. DateTime.Parse(string)  
    - Converts a string to a DateTime.

1. DateTime.TryParse(string, out DateTime)  
    - Safely converts a string to a DateTime without throwing an exception.

1. DateTime.IsLeapYear(int year)
    - Checks whether a year is a leap year.

### DateTime Instance Methods (Object level):-
1. .AddDays()  
    - Adds or subtracts days.

1. .AddMonths()
    - Adds or subtracts months.

1. .AddYears()  
    - Adds or subtracts years.

1. .AddHours()  
    - Adds or subtracts hours.

1. .AddMinutes()  
    - Adds or subtracts minutes.

1. .AddSeconds()  
    - Adds or subtracts seconds.

1. .AddMilliseconds()  
    - Adds or subtracts milliseconds.

1. .ToString(format) 
    - Converts a DateTime to a formatted string.

1. .ToLocalTime()  
    - Converts UTC time to local time.

1. .Subtract(DateTime)  
    - Returns TimeSpan representing the difference between two dates.


## Hands-on:-
```cs
// Current local date & time
DateTime now = DateTime.Now;
Console.WriteLine($"Current Local Date & Time: {now}");

// Current UTC date & time
DateTime utcNow = DateTime.UtcNow;
Console.WriteLine($"Current UTC Date & Time: {utcNow}");

// Today's date
DateTime today = DateTime.Today;
Console.WriteLine($"Today's Date: {today}");


// Custom date
DateTime dob = new DateTime(2003, 7, 15);
Console.WriteLine($"Custom Date: {dob}");


// Date only
DateTime dateOnly = now.Date;
Console.WriteLine($"Date Only: {dateOnly}");


// Access individual parts
Console.WriteLine($"Day: {now.Day}");
Console.WriteLine($"Month: {now.Month}");
Console.WriteLine($"Year: {now.Year}");

Console.WriteLine($"Hour: {now.Hour}");
Console.WriteLine($"Minute: {now.Minute}");
Console.WriteLine($"Second: {now.Second}");


// Format date
Console.WriteLine(now.ToString("dd-MM-yyyy"));
Console.WriteLine(now.ToString("dd-MM-yyyy HH:mm:ss"));


// Add operations (DateTime is immutable)
DateTime futureDate = now.AddDays(5);

Console.WriteLine($"Original Date: {now}");
Console.WriteLine($"After 5 Days: {futureDate}");

Console.WriteLine($"After 2 Months: {now.AddMonths(2)}");
Console.WriteLine($"After 1 Year: {now.AddYears(1)}");


// Static methods
bool isLeapYear = DateTime.IsLeapYear(2024);
Console.WriteLine($"Is Leap Year: {isLeapYear}");


// UTC to Local Time
DateTime localTime = utcNow.ToLocalTime();
Console.WriteLine($"Local Time: {localTime}");


// Parse string to DateTime
DateTime parsedDate = DateTime.Parse("2026-05-30");
Console.WriteLine(parsedDate);


// Safe parsing
if (DateTime.TryParse("2026-05-30", out DateTime safeDate))
{
    Console.WriteLine(safeDate);
}


// Difference between dates
// TimeSpan difference = now.Subtract(dob);
TimeSpan difference = now - dob;

Console.WriteLine($"Days Difference: {difference.Days}");
Console.WriteLine($"Total Days Difference: {difference.TotalDays}");
```
