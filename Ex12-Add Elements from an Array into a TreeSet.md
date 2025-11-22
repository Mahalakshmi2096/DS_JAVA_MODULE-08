# Ex12 Add Elements from an Array into a TreeSet
## DATE: 27.09.2025
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start
2. Read an integer n (size of array).
3. Create an integer array arr of size n.
4. Loop from 0 to n-1:
5. Read each integer and store it in arr[i].
6. Create an empty TreeSet named set.
7. For each element num in arr:
8. Insert num into set (duplicates are automatically removed and sorted).
9. Print all elements of the TreeSet.
10. End
## Program:
```
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        // Type Your Code Here.
        TreeSet<Integer> set = new TreeSet<>();
        for(int num : arr){
            set.add(num);
        }
        return set;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}
```
Developed by: Mahalakshmi B

Reg No: 212224040182

## Output:
<img width="826" height="501" alt="image" src="https://github.com/user-attachments/assets/e3213662-9e95-4059-bd8e-3122165a224c" />

## Result:
The program successfully adds elements from an array into a TreeSet.
