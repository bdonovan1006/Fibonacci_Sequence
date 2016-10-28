# Fibonacci_Sequence
Program asks user for amount of Fibonacci numbers to be printed and then prints that amount.


/**
 * Brian Donovan
 * Brian1006@comcast.net
 * This program will allow 2 users to play the mathematical game Nim 
 */
 
 import java.util.Scanner;

class Fibonacci {

    Scanner keyboard = new Scanner(System.in);
    public int i = 3;

    public void sequence() {
        long x = 0;
        long y = 1;
        long z = 0;
        System.out.print("How many Fibonacci numbers would you like printed?: ");
        long max = keyboard.nextLong();
        int count = 0;

        while (count < max) {
            z = x + y;
            x = y;
            y = z;
            System.out.println(z);
            count++;
        }
    }
}

public class FibonacciSequence {

    public static void main(String[] args) {
        Fibonacci fib = new Fibonacci();
        fib.sequence();
    }

}
