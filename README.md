
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    int rem;
    rem=a%b;
    printf("Remainder of %d and %d=%d",a,b,rem);
}
```
## OUTPUT:
![Screenshot 2025-05-25 130850](https://github.com/user-attachments/assets/4af62bd1-caf7-44cf-baed-83cea9b302a5)

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
```
#include<stdio.h>
int main()
{
  char value;
  
  scanf("%c",&value);
  if(value=='P')
    printf("Present");

  return 0;
}
```
# OUTPUT:
![Screenshot 2025-05-25 130940](https://github.com/user-attachments/assets/5b37b1c5-51ea-4aff-ad9f-42cd347b678b)


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
```
#include <stdio.h>
int main()
{
    int a,b,max;
    scanf("%d%d",&a,&b);
    max = (a>b) ? a : b;
    printf("Maximum between %d and %d is %d", a, b, max);
    return 0;
}
```
## OUTPUT:
![Screenshot 2025-05-25 131019](https://github.com/user-attachments/assets/d8a94034-4bbb-41c7-97cd-76856dee733e)

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
```
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if(a== b){
        printf("Both the values are equal.");
    }
    else {
        printf("Both the values are Not equal.");
    }
}
```
## OUTPUT:

![Screenshot 2025-05-25 131300](https://github.com/user-attachments/assets/78603082-25ac-424b-a13b-b5f6b98de6e5)


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
```
#include <stdio.h>

int main() {
    int mark1, mark2, mark3;
    int total;
    float percentage;

    // Input marks
    printf("Enter marks for subject 1: ");
    scanf("%d", &mark1);

    printf("Enter marks for subject 2: ");
    scanf("%d", &mark2);

    printf("Enter marks for subject 3: ");
    scanf("%d", &mark3);

    // Check if any marks are invalid
    if (mark1 < 0 || mark2 < 0 || mark3 < 0 || mark1 > 100 || mark2 > 100 || mark3 > 100) {
        printf("Invalid marks entered. Marks should be between 0 and 100.\n");
        return 1;
    }

    // Calculate total and percentage
    total = mark1 + mark2 + mark3;
    percentage = total / 3.0;

    // Display total and percentage
    printf("Total Marks = %d\n", total);
    printf("Percentage = %.2f%%\n", percentage);

    // Determine division
    if (mark1 < 33 || mark2 < 33 || mark3 < 33 || percentage < 40) {
        printf("Division: Fail\n");
    } else if (percentage >= 60) {
        printf("Division: First\n");
    } else if (percentage >= 50) {
        printf("Division: Second\n");
    } else {
        printf("Division: Pass\n");
    }

    return 0;
}
```
## OUTPUT:
![Screenshot 2025-05-25 131503](https://github.com/user-attachments/assets/d77139f6-fa18-4d15-ba27-9930ea9f85d7)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

