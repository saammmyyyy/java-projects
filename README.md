# java-projects- student grades
This is a simple project that calculates the grades when scores are entered
//source code
import java.util.Scanner;
public class StudGrade{
    public static void main(String[] args) 
    {

    
    Scanner scanner = new Scanner(System.in);
    System.out.println("Enter the number of Grades:");
    int numGrades = scanner.nextInt();
    int[] grades = new int[numGrades];
    for(int i=0;i<numGrades;i++)
    {
        System.out.println("Enter the Grade: " + (i+1) + ": ");
        grades[i]=scanner.nextInt();
}
scanner.close();
int total=0;
for(int i=0;i<numGrades;i++)
{
    total+=grades[i];

}
double average = (double)total/numGrades;
System.out.println("The average is: " + average);


    }
}
