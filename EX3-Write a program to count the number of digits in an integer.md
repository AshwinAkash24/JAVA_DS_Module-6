# EX3 Write a program to count the number of digits in an integer.
## DATE: 24-09-2025
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Read the integer n from input.
2. Initialize count to 0.
3. Repeat while n is greater than 0.
4. Divide n by 10 each time and increment count.
5. After the loop ends, print the value of count as the number of digits.

## Program:
```JAVA
/*
Program to to count the number of digits in an integer
Developed by: Ashwin Akash M
RegisterNumber: 212223230024
*/
import java.util.Scanner;

public class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n=sc.nextInt();
        int count=0;
        while(n>0){
            n/=10;
            count++;
        }
        System.out.println("Number of digits: " + count);
    }
}

```

## Output:
<img width="1246" height="323" alt="image" src="https://github.com/user-attachments/assets/267c794a-bfba-420b-8e22-8aae3040f602" />



## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
