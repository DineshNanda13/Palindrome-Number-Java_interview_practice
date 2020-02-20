# Palindrome-Number-Java_interview_practice
Java Program to determine whether the given number is palindrome or not
package number_palindrome;

import java.util.*;

/**
 *
 * @author Dinesh Nanda
 */
public class PalindromeNumber {

    public static void main(String[] args) {

        Scanner s = new Scanner(System.in);
        System.out.println("Enter a number");
        int number = s.nextInt();
        int temp = number;
        int new_num = 0;
        
        while (number > 0) {
            int last = number % 10;
            new_num  = (new_num * 10) + last;
            number = number / 10;
        }
        if(new_num == temp){
            System.out.println("Palindrome Number");
        }else{
            System.out.println("Not a Palindrome Number");
        }
    }
}

