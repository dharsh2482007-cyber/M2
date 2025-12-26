# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int M, N, i;
    scanf("%d %d", &M, &N);
    for (i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }
    return 0;
}
```

## OUTPUT:

<img width="452" height="210" alt="image" src="https://github.com/user-attachments/assets/ce6d7ec9-1b6f-4574-bc2e-c8e5fecc6b12" />











## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int i, j, n;

    // Read number of rows
    scanf("%d", &n);

    // Print triangular pattern
    for (i = 1; i <= n; i++) {
        for (j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```


## OUTPUT:

<img width="485" height="291" alt="image" src="https://github.com/user-attachments/assets/2f807966-a80d-4518-838f-aae42bfec2a4" />





## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:

```
#include <stdio.h>

// Function declaration
void add(int a, int b);
void sub(int a, int b);

int main() {
    int x, y;
    scanf("%d %d", &x, &y);
    add(x, y);
    sub(x, y);

    return 0;
}
void add(int a, int b) {
    printf("Addition = %d\n", a + b);
}
void sub(int a, int b) {
    printf("Subtraction = %d\n", a - b);
}
```


## OUTPUT:

<img width="457" height="276" alt="image" src="https://github.com/user-attachments/assets/458cbd54-b908-4ddd-805a-8890ccf8c517" />







## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int n, digit, sum = 0;

    // Read the number
    scanf("%d", &n);

    // Find sum of odd digits
    for (; n != 0; n /= 10) {
        digit = n % 10;
        if (digit % 2 != 0) {
            sum += digit;
        }
    }

    // Print the result
    printf("Sum of odd digits = %d", sum);

    return 0;
}
```


## OUTPUT:

<img width="528" height="192" alt="image" src="https://github.com/user-attachments/assets/a0bb8760-809b-4e93-b310-73761e654640" />




## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:

```
#include <stdio.h>

// Function declaration
long long factorial(int n);

int main() {
    int num;
    long long result;

    // Read the number
    scanf("%d", &num);

    // Function call
    result = factorial(num);

    // Print result
    printf("Factorial = %lld", result);

    return 0;
}

// User-defined function to find factorial
long long factorial(int n) {
    long long fact = 1;
    int i;

    for (i = 1; i <= n; i++) {
        fact *= i;
    }

    return fact;
}
```


## OUTPUT:

<img width="387" height="201" alt="image" src="https://github.com/user-attachments/assets/f13b1505-2a76-4b40-a608-5b5b95a6fbfc" />


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
