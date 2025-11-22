# Ex15 Value Existence Check in a TreeMap
## DATE: 29.09.2025
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Start
2. Read an integer n (number of key–value pairs).
3. Create an empty TreeMap<Integer, String>.
4. Repeat n times:
5. Read an integer key.
6. Read a string value.
7. Insert (key, value) into the TreeMap.
8. Read the string searchValue.
9. Check if the TreeMap contains searchValue using containsValue().
10. If true, print that the value exists.
11. Else, print that the value does not exist.
12. End  

## Program:
```
import java.util.*;
public class TreeMapValueExistenceCheck {
    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        // Type Your Code Here.
        if(map.containsValue(searchValue)){
            System.out.println("Value \"" + searchValue + "\" exists in the TreeMap.");
        }
        else{
            System.out.println("Value \"" + searchValue + "\" does not exist in the TreeMap.");
        }
    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();
        int n = sc.nextInt();
        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();
        checkValue(map, searchValue);
        sc.close();
    }
}
```
Developed by: Mahalakshmi B

Reg No: 212224040182
## Output:
<img width="1071" height="734" alt="image" src="https://github.com/user-attachments/assets/d29af1a7-c5f3-4e8e-bb3d-ac146f2a3b1b" />

## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
