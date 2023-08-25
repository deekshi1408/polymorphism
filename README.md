# polymorphism
class Shape {
    void draw() {
        System.out.println("Drawing a shape.");
    }
}
class Circle extends Shape {
    @Override
    void draw() {
        System.out.println("Drawing a circle.");
    }
}
class Square extends Shape {
    @Override
    void draw() {
        System.out.println("Drawing a square.");
    }
}
public class PolymorphismExample {
    public static void main(String[] args) {
        Shape[] shapes = new Shape[2];
        shapes[0] = new Circle();
        shapes[1] = new Square();
        for (Shape shape : shapes) {
            shape.draw();
        }
    }
}
