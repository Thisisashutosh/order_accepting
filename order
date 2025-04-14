import java.util.Scanner;

public class OrderSystem {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String[] items = {"Burger", "Pizza", "Pasta", "Soda", "Fries"};
        double[] prices = {5.99, 8.99, 7.49, 1.99, 2.99};

        double totalAmount = 0.0;
        int choice;

        do {
            System.out.println("===== Menu =====");
            for (int i = 0; i < items.length; i++) {
                System.out.printf("%d. %s - $%.2f\n", i + 1, items[i], prices[i]);
            }
            System.out.println("6. Display Total and Exit");
            System.out.print("Enter your choice: ");
            choice = scanner.nextInt();

            if (choice >= 1 && choice <= 5) {
                totalAmount += prices[choice - 1];
                System.out.printf("%s added to order. Current total: $%.2f\n", items[choice - 1], totalAmount);
            } else if (choice != 6) {
                System.out.println("Invalid choice. Please try again.");
            }
        } while (choice != 6);

        System.out.printf("Final Total Amount: $%.2f\n", totalAmount);
    }
}
