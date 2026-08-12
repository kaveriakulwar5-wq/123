import java.util.Scanner;

public class MultiplicationTable {
    public static void main(String[] args) {
        // Create a Scanner object to read user input
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Enter a number to print its multiplication table: ");
        int num = scanner.nextInt();
        
        System.out.println("\nMultiplication Table for " + num + ":");
        System.out.println("---------------------------------");
        
        // Loop from 1 to 10 to generate the table
        for (int i = 1; i <= 10; i++) {
            // Using printf for structured, well-aligned output
            System.out.printf("%d x %d = %d\n", num, i, num * i);
        }
        
        // Close the scanner to prevent resource leaks
        scanner.close();
    }
}
