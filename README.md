# CSC-7200-Assignment-1-README-file

Sahil Prajapati 

CSC 7200

Student ID - @01410508

Email - sprajapa@student.fitchburgstate.edu

QUESTION 1 ANSWER

1.	SOURCE CODE

package two;

import java.util.Scanner;

public class one {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the first integer: ");
        int integer1 = scanner.nextInt();

        System.out.print("Enter the second integer: ");
        int integer2 = scanner.nextInt();

        System.out.print("Enter the third integer: ");
        int integer3 = scanner.nextInt();

        // Calculating sum
        int sum = integer1 + integer2 + integer3;

        // Calculating average
        double average = (double) sum / 3;

        // Calculating product
        int product = integer1 * integer2 * integer3;

        // Finding the smallest integer
        int smallest = Math.min(Math.min(integer1, integer2), integer3);

        // Finding the largest integer
        int largest = Math.max(Math.max(integer1, integer2), integer3);

        // Displaying the results
        System.out.println("Sum: " + sum);
        System.out.printf("Average: %.2f%n", average);
        System.out.println("Product: " + product);
        System.out.println("Smallest integer: " + smallest);
        System.out.println("Largest integer: " + largest);
    }
}




QUESTION 2 ANSWER 


SOURCE CODE;

package futureInvestmentValue;

import java.util.Scanner;

public class futureInvestment {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the investment amount: ");
        double investmentAmount = scanner.nextDouble();

        System.out.print("Enter the annual interest rate (%): ");
        double annualInterestRate = scanner.nextDouble();

        double monthlyInterestRate = annualInterestRate / 12 / 100;

        System.out.println("Years\t\tFuture Value");

        for (int years = 1; years <= 10; years++) {
            double futureValue = futureInvestmentValue(investmentAmount, monthlyInterestRate, years);
            System.out.printf("%d\t\t$%.2f%n", years, futureValue);
        }
    }

    public static double futureInvestmentValue(double investmentAmount, double monthlyInterestRate, int years) {
        double futureValue = investmentAmount * Math.pow(1 + monthlyInterestRate, years * 12);
        return futureValue;
    }
}



























