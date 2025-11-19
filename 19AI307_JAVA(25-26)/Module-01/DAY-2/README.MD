# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:

A library charges a fine for every book returned late. For first 5 days the fine is 50 paise, for 6-10 days fine is one rupee and above 10 days fine is 5 rupees. If you return the book after 30 days your membership will be cancelled - Print ("Your Membership would be Cancelled.")

Write a program to accept the number of days the member is late to return the book and display the fine or the appropriate message

## AIM:
To write a program to accept the number of days the member is late to return the book and display the fine or the appropriate message

## ALGORITHM :
1.	Start the program.
2.Import the necessary package java.util for using the Scanner class.
3.Declare the Main class.
4.Inside the class, define the main() method.
5.Create an object of Scanner to accept user input.
6.Prompt the user to enter the number of days the book is returned late.
7.Read and store the value in a variable, e.g., days.
8.If days > 30, display: "Your Membership would be Cancelled."
9.Else if days > 10, display the fine as 5 rupees.
10.Else if days >= 6, display the fine as 1 rupee.
11.Else if days >= 1, display the fine as 50 paise.
12.Else, display "No fine".
13.End the program.




## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: GOGINENI BIDHISHA
RegisterNumber:  212223040048
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

public class LibraryFineCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int daysLate = scanner.nextInt();
        double fine = 0.0;
        if (daysLate > 30) {
            System.out.println("Fine Amount Pay to Rs :170.00");
            System.out.println("Your Membership would be Cancelled.");
        } else if (daysLate > 10) {
            fine = daysLate * 5;
            System.out.printf("Fine Amount Pay to Rs :%.2f\n", fine);
        } else if (daysLate > 5) {
            fine = daysLate * 1;
            System.out.printf("Fine Amount Pay to Rs :%.2f\n", fine);
        } else if (daysLate > 0) {
            fine = daysLate * 0.5;
            System.out.printf("Fine Amount Pay to Rs :%.2f\n", fine);
        } else {
            System.out.println("No fine.");
        }

        scanner.close();
    }
}

```





## OUTPUT:


## RESULT:

The program successfully accepts the number of late days and displays the correct fine or message based on the library rules.
