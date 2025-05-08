# Basic-Programs

### Get count of vowels

```c#

Console.WriteLine("Please enter a string to count the vowels:");
var input = Console.ReadLine();

Console.WriteLine($"You entered: {input} and the number of vowels in it is {GetVowelCount(input)}.");
Console.ReadLine();

static int GetVowelCount(string value)
{
    var count = 0;
    for (int i = 0; i < value.Length; i++)
    {
        if (IsVowel(char.ToLower(value[i])))
        {
            count++;
        }
    }
    return count;
}

static bool IsVowel(Char value)
{
    return value == 'a' || value == 'e' || value == 'i' || value == 'o' || value == 'u';
}

----Output
Please enter a string to count the vowels:
Akshay
You entered: Akshay and the number of vowels in it is 2.
```
