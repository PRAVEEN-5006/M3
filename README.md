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
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float rate, int months) {
    float emi;
    float r = rate / (12 * 100);
    emi = (principal * r * pow(1 + r, months)) / (pow(1 + r, months) - 1);
    printf("The EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;
    printf("Enter the principal amount: ");
    scanf("%f", &principal);

    printf("Enter the annual rate of interest: ");
    scanf("%f", &rate);

    printf("Enter the number of months: ");
    scanf("%d", &months);

    calculateEMI(principal, rate, months);

    return 0;
}


## OUTPUT
![Screenshot 2025-04-28 204245](https://github.com/user-attachments/assets/fed85b1f-7e97-458c-8d20-7de5b1f1cf26)






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
#include <stdio.h>

int main() {
    int n = 6; 
    int first = 0, second = 1, next, i;

    printf("Fibonacci Series for %d terms:\n", n);

    for (i = 0; i < n; i++) {
        if (i == 0) {
            printf("%d ", first);
            continue;
        }
        if (i == 1) {
            printf("%d ", second);
            continue;
        }
        next = first + second;
        printf("%d ", next);
        first = second;
        second = next;
    }

    return 0;
}

## OUTPUT

![Screenshot 2025-04-28 204430](https://github.com/user-attachments/assets/1cba2d94-291d-4b68-a1f9-d8273bc90928)







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
#include <stdio.h>

int main() {
    int n, i;
    
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    int arr[n]; 
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n-1]);

    return 0;
}

## OUTPUT

![Screenshot 2025-04-28 204626](https://github.com/user-attachments/assets/1e35cb62-38b1-4b76-8616-11d610c196ba)








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
#include <stdio.h>

int main() {
    int n, i, count = 0;
    
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    int arr[n]; 
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements: %d\n", count);

    return 0;
}


## OUTPUT

![Screenshot 2025-04-28 204825](https://github.com/user-attachments/assets/c05044aa-82ba-496a-afbc-bbb2d5742366)




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
#include <stdio.h>

int main() {
    int n, i, num;
    char arr[100]; 

    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &num); 
        if (num % 2 == 0) {
            arr[i] = 'E'; 
        } else {
            arr[i] = num; 
        }
    }

    printf("Updated array:\n");
    for (i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("%c ", arr[i]); 
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}

## Output:
![Screenshot 2025-04-28 205059](https://github.com/user-attachments/assets/17d67a9e-ab22-436a-9edd-f02a8c2a0ef2)

 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



