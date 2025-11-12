# Ex5 Count Inversions in an Array
## DATE:
## AIM:
To write a Java program  to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j.

## Algorithm
1.Start the program.   
2.Read the number of elements n from the user.  
3.Declare an array arr of size n.  
4.Read all the n elements of the array from the user.  
5.Define a function countInversions(arr) that:    
- a. Initialize count = 0.  
- b. Repeat for i = 0 to n - 2:  
--> i. For each j = i + 1 to n - 1:  
--> ii. If arr[i] > arr[j], increment count by 1.  
- c. Return the value of count.
  
6.Call the function countInversions(arr) and store the result in a variable.  
7.Display the total number of inversions.  
8.Stop the program.    

## Program:
```
/*
Program toto Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
Developed by: K L RAVEENDRANATH
RegisterNumber:  212224060212
*/

import java.util.*;
public class CountInversions {
    static int countInversions(int[] arr) {
        int count = 0;
        for (int i = 0; i < arr.length - 1; i++)
            for (int j = i + 1; j < arr.length; j++)
                if (arr[i] > arr[j])
                    count++;
        return count;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        System.out.println("Number of inversions: " + countInversions(arr));
    }
}

```

## Output:
<img width="432" height="216" alt="image" src="https://github.com/user-attachments/assets/0c69e9d3-7471-45e3-88d0-08f81868a017" />


## Result:
Thus the Java program to to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < jis implemented successfully.
