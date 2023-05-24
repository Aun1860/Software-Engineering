# Software Engineering
 Software Engineering Assignment 
 sir i have created electricity bill program  myslef i can any thing from it but my build file is not working  i dont know how but here is my code 
 import java.util.Scanner;


public class ElectricityBill {
    public static void main(String[] args) {
        Scanner program2= new Scanner(System.in);
        System.out.print("Enter Your Units Consumed:");
        int unitsConsumed= program2.nextInt();
        int billAmount;

        if (unitsConsumed <= 100) {
            billAmount = unitsConsumed ;
        } else if (unitsConsumed <= 200) {
            billAmount = 100 + ((unitsConsumed - 100) * 3);
        } else if (unitsConsumed <= 300) {
            billAmount = 400 + ((unitsConsumed - 200) * 5);
        } else if (unitsConsumed<=400) {
            billAmount = 900 + ((unitsConsumed - 300) * 7);

        } else {
            billAmount = 1600 + ((unitsConsumed - 400) * 9);
        }

        System.out.println(" Your Electricity Bill Amount is " + billAmount+" Rupees");
        System.out.println("Thank you for using Our Service");
    }
}

