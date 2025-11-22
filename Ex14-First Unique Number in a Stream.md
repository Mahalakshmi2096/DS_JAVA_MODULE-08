# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE: 29.09.2025
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1. Start
2. Read an integer n (number of inputs in the stream).
3. Create an empty LinkedHashMap to store numbers with their frequencies.
4. Repeat for each of the n inputs:
5. Read the next number num.
6. Update its frequency in the map: map[num] = map.getOrDefault(num, 0) + 1
7. Set firstunique = -1
8. Traverse the map in insertion order:
9. If a number has frequency 1, set it as firstunique and break.
10. If firstunique is not -1, print the first unique number.
11. Else, print "No unique number".
12. End

## Program:
```
import java.util.*;

public class FirstUniqueNumberStream {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        LinkedHashMap<Integer, Integer> map= new LinkedHashMap<>();
        for(int i=0; i<n; i++){
            int num = sc.nextInt();
            map.put(num, map.getOrDefault(num, 0)+1);
            int firstunique=-1;
            for(Map.Entry<Integer, Integer> entry : map.entrySet()){
                if(entry.getValue() == 1){
                    firstunique = entry.getKey();
                    break;
                }
            }
            if(firstunique!=-1){
                System.out.println("First unique number: " + firstunique);
            }else{
                System.out.println("No unique number");
            }
        }
        sc.close();
    }
}
```
Developed by: Mahalakshmi B

Reg no: 212224040182
## Output:
<img width="896" height="583" alt="image" src="https://github.com/user-attachments/assets/b484b690-9103-4e6c-8f41-da4fa772f324" />

## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
