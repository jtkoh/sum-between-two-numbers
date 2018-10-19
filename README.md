# sum-between-two-numbers
program should ask for both the lower and upper bound. 
You can assume that the users first gives the smaller number and then the greater number.

Example outputs:

First: 3
Last: 5
The sum 12
    
First: 2
Last: 8
The sum is 35

import java.util.Scanner;


public class TheSumBetweenTwoNumbers {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        System.out.print("First: ");
        int userInt0 = Integer.parseInt(reader.nextLine());
        System.out.print("Second: ");
        int userInt1 = Integer.parseInt(reader.nextLine());
        int block = 0, sum = 0;
        while (block <= (userInt1 - userInt0)) {
            sum = sum + userInt0;
            userInt0 = userInt0 + 1;
            block++;
        }
        System.out.println("sum, userInt0, block "+ sum +" "+ userInt0 +" "+ block);
    }
}
