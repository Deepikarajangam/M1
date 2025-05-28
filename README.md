
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```#include <stdio.h>
int main()
{
  char a,b,c;
 
  
  scanf("%c %c %c",&a, &b, &c);
  {
  printf("The reverse of %c%c%c is %c%c%c", a,b,c,c,b,a);
  }  
  return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/4c0ab224-51e1-447d-af6c-918d0ee03774)

















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
```#include <stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a>=0)
    {
        printf("a is positive number");
    }
    
 return 0;   
}
```

# OUTPUT:

![image](https://github.com/user-attachments/assets/33a81737-5afa-4e3b-97a9-32f402e33b40)










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
```#include <stdio.h>

int main() {
    
    float num1, denom1, num2, denom2;
    float frac1, frac2, result;

    
    printf("Enter numerator and denominator of first fraction: ");
    scanf("%f %f", &num1, &denom1);

    
    printf("Enter numerator and denominator of second fraction: ");
    scanf("%f %f", &num2, &denom2);

    
    frac1 = num1 / denom1;
    frac2 = num2 / denom2;


    result = (frac1 < frac2) ? frac1 : frac2;

    
    printf("The minimum of the two fractions is: %.2f\n", result);

    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/3f6615e8-4292-4a06-9698-08f230eb0fd4)









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
```#include <stdio.h>

int main() {
    int num;

   
    printf("Enter a number: ");
    scanf("%d", &num);

    
    if (num == 1) {
        printf("The number is equal to 1.\n");
    } else {
        printf("The number is not equal to 1.\n");
    }

    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/33329114-52da-4206-b41a-a7d776dbfc31)











	

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
```#include <stdio.h>

int main() {
    float marks1, marks2, marks3, total, percentage;


    
    scanf("%f", &marks1);
    
    scanf("%f", &marks2);
    
    scanf("%f", &marks3);

    
    if (marks1 < 40 || marks2 < 40 || marks3 < 40) {
        printf("Total Marks = %.0f\n", marks1 + marks2 + marks3);
        printf("Percentage = %.2f\n", (marks1 + marks2 + marks3) / 3);
        printf("Division = Fail\n");
    } else {
        
        total = marks1 + marks2 + marks3;
        percentage = (total / 300) * 100;

        
        printf("Total Marks = %.0f\n", total);
        printf("Percentage = %.2f\n", percentage);

        
        if (percentage >= 60) {
            printf("Division = First\n");
        } else if (percentage >= 48) {
            printf("Division = Second\n");
        } else if (percentage >= 36) {
            printf("Division = Pass\n");
        } else {
            printf("Division = Fail\n");
        }
    }

    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/2d559fa8-3aa1-4066-86b7-c259ccff2885)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

