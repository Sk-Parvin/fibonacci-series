import java.util.Scanner;
public class FibonacciSeries {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of terms in the Fibonacci series: ");
        int numTerms = scanner.nextInt();
        System.out.println("Fibonacci Series up to " + numTerms + " terms:");
        printFibonacci(numTerms);
        scanner.close();
    }
    private static void printFibonacci(int numTerms) {
        if (numTerms <= 0) {
            return;
        }
        int first = 0, second = 1;
        System.out.print(first + " ");
        for (int i = 1; i < numTerms; i++) {
            System.out.print(second + " ");
            int next = first + second;
            first = second;
            second = next;
        }
    }
}
