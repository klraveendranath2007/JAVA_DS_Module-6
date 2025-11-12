# EX3 Write a program to count the number of digits in an integer.
## DATE:
## AIM:
To write a C program to count the number of digits in an integer.

## Algorithm
Step 1: Start  
Step 2: Read an integer num from the user.  
Step 3: Define a recursive function countDigits(num) that:  
            • Checks if num is equal to 0.    
            • If yes, return 0 (base condition).    
            • Otherwise, return 1 + countDigits(num / 10).    
Step 4: In the main function, call countDigits(num) and store the result in count.  
Step 5: Display "Number of digits: " followed by the value of count.  
Step 6: Stop.  

## Program:
```
/*
Program to to count the number of digits in an integer
Developed by: K L RAVEENDRANATH
RegisterNumber:  212224060212
*/

import java.util.*;
public class CountDigits {
	static int countDigits(int num) {
		if (num == 0)
			return 0;
		return 1 + countDigits(num / 10);
	}

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.print("Enter an integer: ");
		int num = sc.nextInt();

		int count = countDigits(num);
		System.out.println("Number of digits: " + count);
	}
}

```


## Output:
<img width="592" height="181" alt="image" src="https://github.com/user-attachments/assets/5d7a8fd9-7f0f-4a2d-aa0a-f234e864f6a6" />



## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
