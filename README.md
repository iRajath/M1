
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:

```c
#include <stdio.h>
int main(void)
{
    char ch1, ch2, ch3;
	printf("Enter three characters: ");
    scanf("%c %c %c", &ch1, &ch2, &ch3);
    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);
    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/70c5869c-71d8-48b2-be6b-8ced557016ca)
















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:

```c
#include <stdio.h>

int main(void)
{
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);
    if (n >= 0)
    {
        printf("Number is positive.\n");
    }
    else
    {
        printf("Number is negative.\n");
    }
    return 0;
}
```
# OUTPUT:

![image](https://github.com/user-attachments/assets/2c98a996-6dc6-4f12-a491-8a7aad9d485e)










# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:

```c
#include <stdio.h>

int main(void)
{
    float num1, num2, min;

    printf("Enter two fractional numbers: ");
    scanf("%f %f", &num1, &num2);

    min = (num1 < num2) ? num1 : num2;
    printf("Minimum of %.2f and %.2f is %.2f\n", num1, num2, min);

    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/56dada92-63a2-4418-a6be-fc5483574a22)








## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:

```c
#include <stdio.h>

int main(void)
{
    int value;
    printf("Enter a value: ");
    scanf("%d", &value);
    if (value == 1)
    {
        printf("The value is equal to 1.\n");
    }
    else
    {
        printf("The value is not equal to 1.\n");
    }

    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/097ec241-3edc-4752-8f6a-e9718f993243)








	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:

```c
#include <stdio.h>

int main(void)
{
    float marks1, marks2, marks3;
    float total, percentage;

    printf("Enter marks for subject 1 (out of 100): ");
    scanf("%f", &marks1);

    printf("Enter marks for subject 2 (out of 100): ");
    scanf("%f", &marks2);

    printf("Enter marks for subject 3 (out of 100): ");
    scanf("%f", &marks3);

    if (marks1 < 0 || marks1 > 100 || marks2 < 0 || marks2 > 100 || marks3 < 0 || marks3 > 100)
    {
        printf("Invalid marks entered! Marks should be between 0 and 100.\n");
        return 1;
    }

    total = marks1 + marks2 + marks3;
    percentage = (total / 300) * 100;

    printf("\nResults:\n");
    printf("Total marks: %.2f\n", total);
    printf("Percentage: %.2f%%\n", percentage);

    if (marks1 < 40 || marks2 < 40 || marks3 < 40)
    {
        printf("Division: Fail (One or more subjects below passing marks)\n");
    }
    else if (percentage >= 60)
    {
        printf("Division: First Division\n");
    }
    else if (percentage >= 50)
    {
        printf("Division: Second Division\n");
    }
    else if (percentage >= 40)
    {
        printf("Division: Pass\n");
    }
    else
    {
        printf("Division: Fail\n");
    }

    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/c015d126-2a16-4a25-8a3d-69174f981abe)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

