# sphere.java

import java.lang.Math;

class Sphere {
    private double diameter;

    public Sphere(double diameter) {
        this.diameter = diameter;
    }

    // Setter method for diameter
    public void setDiameter(double diameter) {
        this.diameter = diameter;
    }

    // Method to calculate and return the volume of the sphere
    public double calculateVolume() {
        return (4.0 / 3.0) * Math.PI * Math.pow(diameter / 2.0, 3);
    }

    // Method to calculate and return the surface area of the sphere
    public double calculateSurfaceArea() {
        return 4 * Math.PI * Math.pow(diameter / 2.0, 2);
    }

    // toString method to return a one-line description of the sphere
    public String toString() {
        return "Sphere with diameter " + diameter;
    }
}

public class MultiSphere {
    public static void main(String[] args) {
        // Instantiate and update several Sphere objects
        Sphere sphere1 = new Sphere(3.0);
        Sphere sphere2 = new Sphere(5.0);

        // Display initial descriptions
        System.out.println("Initial descriptions:");
        System.out.println(sphere1);
        System.out.println(sphere2);

        // Update the diameter of sphere1
        sphere1.setDiameter(4.0);

        // Display updated descriptions and calculated properties
        System.out.println("\nUpdated descriptions and properties:");
        System.out.println(sphere1);
        System.out.println("Volume of sphere1: " + sphere1.calculateVolume());
        System.out.println("Surface area of sphere1: " + sphere1.calculateSurfaceArea());
        System.out.println(sphere2);
        System.out.println("Volume of sphere2: " + sphere2.calculateVolume());
        System.out.println("Surface area of sphere2: " + sphere2.calculateSurfaceArea());
    }
}
Volume of sphere1: 33.510321638291124
Surface area of sphere1: 50.26548245743669
Sphere with diameter 5.0
Volume of sphere2: 65.44984694978736
Surface area of sphere2: 78.53981633974483
