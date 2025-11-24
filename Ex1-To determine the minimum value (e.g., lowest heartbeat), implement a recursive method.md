## EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE: 19-08-2025
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
Read n and store the n input elements into the array.
Call getMin(arr, 0, n) to compute the minimum.
In getMin, if only one element remains (n == 1), return that element.
Otherwise recursively find the minimum of the rest of the array by calling getMin(arr, i+1, n-1).
Compare arr[i] with the minimum from recursion and return the smaller value.
## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: 
RegisterNumber:  
*/

/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: Ashwin Akash M
RegisterNumber: 212223230024
*/
import java.util.*;

public class Main {
    static int getMin(int[] arr, int i, int n)
    {
        if (n==1){
            return arr[i];
        }
        
       int minRest = getMin(arr,i+1,n-1);
       return Math.min(arr[i],minRest);
        
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.println(getMin(arr, 0, n));
    }
}

```

## Output:



## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
