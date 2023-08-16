# Palindrome


## Aim:
To write a C# program to find whether the given string is a Palindrome or not.
## Algorithm:
**Step 1:** Start
**Step 2:** Declare a string variable s and an empty string variable revs.
**Step 3:** Print "Enter string".
**Step 4:** Read input and store it in variable s.
**Step 5:** Initialize a loop with i starting from the length of s minus 1 and going down to 0.
**Step 5.1:** Append the character at index i of s to the string revs.
**Step 6:** Check if revs is equal to s.
**Step 6.1:** If they are equal, print "String is Palindrome" along with the original string s and the reversed string revs.
**Step 6.2:** If they are not equal, print "String is not Palindrome" along with the original string s and the reversed string revs.
**Step 7:** End
## Program:
```
using System;
namespace palindrome
{
    class Program
    {
        static void Main(string[] args)
        {
            string s, revs = "";
            Console.WriteLine(" Enter string");
            s = Console.ReadLine();
            for (int i = s.Length - 1; i >= 0; i--) //String Reverse  
            {
                revs += s[i];
            }
            if (revs == s) // Checking whether string is palindrome or not  
            {
                Console.WriteLine("String is Palindrome \n Entered String Was {0} and reverse string is {1}", s, revs);
            }
            else
            {
                
                Console.WriteLine("String is not Palindrome \n Entered String Was {0} and reverse string is {1}", s, revs);
            }
            Console.ReadKey();
        }
    }
}
```
## Output:
![out](https://github.com/Praveen22042005/Palindrome/assets/112475766/fe44cde1-3b3c-45e9-a4a3-1ab90426ca1e)

## Result:
Thus the C# program to display whether the given string is Palindrome or not is executed successfully.
