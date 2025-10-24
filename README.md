
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

int main() {
    char a,b,c;
	scanf("%c %c %c",&a,&b,&c);
	printf("%c %c %c",c,b,a);
	return 0;
}


## OUTPUT:
<img width="1811" height="481" alt="image" src="https://github.com/user-attachments/assets/f83b0111-de54-436f-b1ce-bae74429c15c" />


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
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a>0)
    printf("%d is Positive",a);
    else if(a==0)
    printf("%d is neither Positive nor Negative",a);
    else
    printf("%d is Negative",a);
    return 0;
}

# OUTPUT:
<img width="1813" height="677" alt="image" src="https://github.com/user-attachments/assets/8f9550cb-7df1-4c21-8f46-941967651117" />
<img width="1813" height="682" alt="image" src="https://github.com/user-attachments/assets/36d7d06a-bf5f-4929-a4b2-04fa93597e50" />
<img width="1814" height="686" alt="image" src="https://github.com/user-attachments/assets/bcf44348-c312-4417-89d6-eb7699370c3b" />


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
#include<stdio.h>
int main()
{
    printf("Enter the first fraction\n");
    float a,b;
    scanf("%f/%f",&a,&b);
    float x=a/b;
    printf("Enter the second fraction\n");
    float c,d;
    scanf("%f/%f",&c,&d);
    float y=c/d;
    float min=x<y?x:y;
    printf("%f",min);
    return 0;
}

## OUTPUT:
<img width="1816" height="716" alt="image" src="https://github.com/user-attachments/assets/33dd7bb1-03a8-4860-834a-4ff15c75948e" />


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
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a==1)
    printf("%d is equal to 1",a);
    else
    printf("%d is not equal to 1",a);
    return 0;
}

## OUTPUT:
<img width="1812" height="564" alt="image" src="https://github.com/user-attachments/assets/64d07a62-d883-45be-befc-9351ff0e3ebe" />
<img width="1814" height="605" alt="image" src="https://github.com/user-attachments/assets/55d36211-5c74-44e5-b858-1e831733d430" />


## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully




# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 

## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determine the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.

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
11.	
## PROGRAM:
#include<stdio.h>
int main()
{
    int m1,m2,m3;
    float total, per;
    scanf("%d %d %d",&m1,&m2,&m3);
    total=m1+m2+m3;
    per=total/3;
    printf("Total marks = %.0f\nPercentage = %.2f\n",total,per);
    if(m1>=40&&m2>=40&&m3>=40)
    {
        if(per>=60)
        printf("Division = First");
        else if(per>=48)
        printf("Division = Second");
        else if(per>=36)
        printf("Division = pass");
        else
        printf("Division = Fail");
    }
    return 0;
}

## OUTPUT:
<img width="1812" height="432" alt="image" src="https://github.com/user-attachments/assets/9499d527-059a-49cf-b46a-5f207f6eb1e0" />
<img width="1813" height="509" alt="image" src="https://github.com/user-attachments/assets/4cd00f59-7bae-4dc1-992b-8c7a74096d2f" />
<img width="1815" height="455" alt="image" src="https://github.com/user-attachments/assets/9668d9a8-d121-41b4-8564-943f5c65a9bd" />
<img width="1816" height="475" alt="image" src="https://github.com/user-attachments/assets/1c95456a-91f9-483a-9496-465e7c57d5db" />

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

