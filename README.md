# java
public class Main {
public static void main(String[] args) {


class Shape {
public double calculateArea() {
return 0; // Default implementation returns 0
}
}
class Circle extends Shape {
private double radius;


public Circle(double radius) {
this.radius = radius;
}


@Override
public double calculateArea() {
return Math.PI * radius * radius;
}
}
class Rectangle extends Shape {
private double width;
private double height;


public Rectangle(double width, double height) {
this.width = width;
this.height = height;
}


@Override
public double calculateArea() {
return width * height; // Calculate area of rectangle
}
}
class Triangle extends Shape {
private double base;
private double height;


public Triangle(double base, double height) {
this.base = base;
this.height = height;
}


@Override
public double calculateArea() {
return 0.5 * base * height; // Calculate area of triangle
}
}




Circle circle = new Circle(4);
System.out.println("Area of Circle: " + circle.calculateArea());
Rectangle rectangle = new Rectangle(5, 4);


System.out.println("\nArea of Rectangle: " + rectangle.calculateArea());


Triangle triangle = new Triangle(2, 6);
System.out.println("\nArea of Triangle: " + triangle.calculateArea());




}
}
