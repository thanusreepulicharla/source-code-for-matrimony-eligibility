# source-code-for-matrimony-eligibility
import java.util.Scanner;

public class Matrimony {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the Gender (M/F):");
        char a = sc.next().charAt(0);
        System.out.println("Enter the Age:");
        int age = sc.nextInt();

        if (a == 'M' || a == 'F') {
            if (a == 'M') {
                if (age >= 21) {
                    System.out.println("Eligible");
                } else {
                    System.out.println("Not Eligible");
                }
            } else {
                if (age >= 18) {
                    System.out.println("Eligible");
                } else {
                    System.out.println("Not Eligible");
                }
            }
        } else {
            System.out.println("Invalid input");
        }
    }
}
