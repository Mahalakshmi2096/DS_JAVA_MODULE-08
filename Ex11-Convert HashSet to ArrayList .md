# Ex11 Convert HashSet to ArrayList in Java
## DATE: 27.09.2025
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1. Start
2. Read an integer n (number of elements).
3. Create an empty HashSet set.
4. Repeat n times:
5. Read an integer num.
6. Insert num into set.
7. Convert the HashSet into an ArrayList using: list = new ArrayList<>(set)
8. Print all elements of the ArrayList.
9. End   
## Program:
```
import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
        // Type Your Code Here.
        return new ArrayList<>(set);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

```
Developed by: Mahalakshmi B

Reg No: 212224040182
## Output:
<img width="838" height="631" alt="image" src="https://github.com/user-attachments/assets/29a01fd4-c0e4-4534-b327-d5474f5adb28" />

## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
