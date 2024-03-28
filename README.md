# Student-grade-calculator-
import java.util.Scanner;

public class StudentGradeCalculator {
    public static void main(String[] args) {
        float[] marks = new float[8];
        float sum = 0, avg;
        Scanner scan = new Scanner(System.in);

        System.out.print("Enter Marks Obtained in 8 Subjects: ");
        for (int i = 0; i < 8; i++) {
            marks[i] = scan.nextFloat();
            sum += marks[i];
        }

        avg = sum / 8;

        System.out.print("\nGrade = ");
        if (avg >= 94)
            System.out.println("A");
        else if (avg >= 90 && avg < 94)
            System.out.println("A-");
        else if (avg >= 87 && avg < 90)
            System.out.println("B+");
        else if (avg >= 83 && avg < 87)
            System.out.println("B");
        else if (avg >= 80 && avg < 83)
            System.out.println("B-");
        else if (avg >= 77 && avg < 80)
            System.out.println("C+");
        else if (avg >= 73 && avg < 77)
            System.out.println("C");
        else if (avg >= 70 && avg < 73)
            System.out.println("C-");
        else if (avg >= 67 && avg < 70)
            System.out.println("D+");
        else if (avg >= 63 && avg < 67)
            System.out.println("D");
        else if (avg >= 60 && avg < 63)
            System.out.println("D-");
        else
            System.out.println("F");
    }
}

Here’s how the program works:

It prompts the user to input marks obtained in 8 subjects.
The program calculates the total marks by summing up the individual subject marks.
The average percentage is computed by dividing the total marks by 8 (the number of subjects).
Based on the average percentage, the corresponding grade is assigned according to the table you provided.
Feel free to input the marks and see the grade calculated! 📊
