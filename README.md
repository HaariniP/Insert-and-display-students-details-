# Insert-and-display-students-details-
import java.util.Scanner;
class Student {
    String name;
    int age;
    String grade;
    void displayDetails() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Grade: " + grade);
    }
}
public class StudentDetails {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Student student = new Student();
        System.out.print("Enter student name: ");
        student.name = scanner.nextLine();
        System.out.print("Enter student age: ");
        student.age = scanner.nextInt();
        scanner.nextLine();  // Consume leftover newline
        System.out.print("Enter student grade: ");
        student.grade = scanner.nextLine();
        System.out.println("\nStudent Details:");
        student.displayDetails();
        scanner.close();
    }
}

Output 
Student Details:
Name: Alice
Age: 20
Grade: A
