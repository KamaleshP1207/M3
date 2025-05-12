# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h> // For pow function

// Function to calculate and display EMI (without return type, with arguments)
void calculateEMI(float principal, float rate, int months) {
    float monthlyRate = rate / (12 * 100); // Converting annual rate to monthly rate
    float emi = (principal * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);

    // Displaying the EMI result
    printf("\nEMI for the given details is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;

    // Reading principal, rate of interest, and number of months
    printf("Enter the Principal amount: ");
    scanf("%f", &principal);

    printf("Enter the Rate of Interest (annual in percentage): ");
    scanf("%f", &rate);

    printf("Enter the Number of Months: ");
    scanf("%d", &months);

    // Calling the EMI calculation function
    calculateEMI(principal, rate, months);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/39c6d873-365d-45b7-a646-27680b5de8ff)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n = 6, first = 0, second = 1, next;

    // Displaying Fibonacci series
    printf("Fibonacci Series for %d terms: \n", n);

    for (int i = 1; i <= n; i++) {
        if (i == 1) {
            printf("%d ", first);
            continue;
        }
        if (i == 2) {
            printf("%d ", second);
            continue;
        }

        next = first + second;
        first = second;
        second = next;

        printf("%d ", next);
    }

    printf("\n");

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/84842bc3-1eea-4766-84cf-eaa472a03302)








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;

    // Reading the number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    // Declaring an array
    int arr[n];

    // Reading array elements
    printf("Enter %d elements: \n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Displaying the last element
    printf("The last element of the array is: %d\n", arr[n - 1]);

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/2eefd470-b592-45fe-bf03-d0b2ca4f04cc)









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, count = 0;

    // Reading the number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    // Declaring an array
    int arr[n];

    // Reading array elements
    printf("Enter %d elements: \n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        // Checking if the element is positive
        if (arr[i] > 0) {
            count++;
        }
    }

    // Displaying the result
    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/6488efa8-e3ed-4ed5-b625-ad4efc7c0150)





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;

    // Reading the number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    // Declaring an array
    int arr[n];

    // Reading array elements
    printf("Enter %d elements: \n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Replacing even elements with 'E'
    printf("\nUpdated Array: \n");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");

    return 0;
}
```
## Output:
![image](https://github.com/user-attachments/assets/b5acfdfb-29e4-4e62-9d6a-25f346c5d9cd)
 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



