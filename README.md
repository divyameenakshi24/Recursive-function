# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:

### Step 1:
Create a function for reversing.

### Step 2:
Get the number from the user.

### Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step 4:
Recusively call this function to get the reversed number.

### Step 5:
print the reversed number.

## Program:
```python
using System;
namespace Recursive
{
    class hello
    {
        public static int m, reverse = 0;
        public static int R(int no)
        {

            if (no > 0)
            {
                hello.m = no % 10;
                hello.reverse = hello.reverse * 10 + m;
                no = no / 10;
                return R(no);
            }
            return hello.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(R(num));
        }
    }
}
```

## Output:
![image](https://user-images.githubusercontent.com/75235402/171101641-3ba61adb-f1b4-4658-a091-24fe83663242.png)


## Result:
Thus the C# program to reverse a number using recursive function is executed successfully.
