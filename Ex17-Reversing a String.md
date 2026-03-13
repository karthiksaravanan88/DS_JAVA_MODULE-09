# Ex17 Reversing a String Using Stack Data Structure
## DATE: 03-10-2026
## AIM:
To write a Java program that reverses an input string using a stack, without using built-in reverse functions.

## Algorithm
1. Read the input string from the user.
2. Create a stack and push each character of the string onto it.
3. Create a StringBuilder to build the reversed string.
4. Pop characters from the stack one by one and append them to the StringBuilder.
5. Return and print the final reversed string.

## Program:
```JAVA
/*
Program to reverses an input string using a stack
Developed by: karthik
RegisterNumber: 212224230118
*/
import java.util.Scanner;
import java.util.Stack;

public class ReverseStringWithStack {

    public static String reverseString(String input) {
        //Type code here...
        Stack<Character> stack = new Stack<>();
        for (char ch : input.toCharArray())
        stack.push(ch);
        StringBuilder reversed = new StringBuilder();
        while (!stack.isEmpty())
        reversed.append(stack.pop());
        return reversed.toString();
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine();

        // Reverse using stack
        String reversed = reverseString(input);

        // Display result
        System.out.println(reversed);

        scanner.close();
    }
}
```
## Output:
<img width="1291" height="285" alt="image" src="https://github.com/user-attachments/assets/1148eae1-6f96-41f6-b360-48f56040a286" />



## Result:
Thus, the program successfully reverses the given string using a stack without relying on built-in reverse functions.
