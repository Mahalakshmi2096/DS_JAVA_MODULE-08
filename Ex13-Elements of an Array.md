# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE: 27.09.2025 
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Start
2. Read an integer value from the user.
3. Create an integer array arr of size 10.
4. Fill all elements of arr with the value using:
5. Arrays.fill(arr, value)
6. Print all elements of the array.
7. End   
## Program:
```
import java.util.*;
public class FillArrayUsingArraysFill {
    public static int[] fillArray(int size, int value) {
        // Type Your Code Here.
        int[] arr=new int[size];
        Arrays.fill(arr, value);
        return arr;
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}
```
Developed by: Mahalakshmi B

Reg No: 212224040182
## Output:
<img width="800" height="254" alt="image" src="https://github.com/user-attachments/assets/f2691d9c-89be-4d7f-8943-af48159eaf3a" />

## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
