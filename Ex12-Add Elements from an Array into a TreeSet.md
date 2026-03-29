# Ex12 Add Elements from an Array into a TreeSet
# Date: 28/02/2026

## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start the program.
2. Create an array containing integer elements.
3. Create a TreeSet object.
4. Add all elements of the array to the TreeSet using a loop or Collections method.
5. Display the elements of the TreeSet.
6. Stop the program.

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: KAILASH KUMAR S
RegisterNumber: 212223220041

*/
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        TreeSet<Integer> set = new TreeSet<>();
        for (int a:arr)
            set.add(a);
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

## Output:

<img width="798" height="580" alt="image" src="https://github.com/user-attachments/assets/e3164f22-e559-4c04-9009-91292e909907" />




## Result:
The program successfully adds elements from an array into a TreeSet.
