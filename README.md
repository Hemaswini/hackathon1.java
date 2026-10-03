# hackathon1.java
import java.util.Scanner;
public class CollectionWaste {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int vehicleNumber = 209;
        double wasteCollected = 29.3;
        int collectionPoints = 13;
        char vehicleStatus = 'L';
System.out.println("Vehicle Number: " + vehicleNumber);
        System.out.println("Waste Collected: " + wasteCollected + " kg");
        System.out.println("Collection Points: " + collectionPoints);
        System.out.println("Vehicle Status: " + vehicleStatus);
        System.out.print("Enter waste collected in kilograms: ");
        double waste = sc.nextDouble();
        if (waste >= 100) {
            System.out.println("Collection Target Achieved");
        } else {
            System.out.println("More Waste Collection Required");
        }
        System.out.print("Enter waste collected at Point 1: ");
        double point1Waste = sc.nextDouble();
        System.out.print("Enter waste collected at Point 2: ");
        double point2Waste = sc.nextDouble();
        double totalWaste = calculateTotalWaste(point1Waste, point2Waste);
        System.out.println("Total Waste Collected: " + totalWaste + " kg");
        sc.close();
}
public static double calculateTotalWaste(double point1Waste, double point2Waste) {
        return point1Waste + point2Waste;
    }
}
