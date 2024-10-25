# EX-NO-6-Pseudo-Random-Number

## AIM : -
To implement Pseudorandom Number Generation using Standard Library.

## ALGORITHM : -

Step 1: Get the number of random numbers to generate from the user.<br>
Step 2: Read the minimum and maximum values for the random number range.<br>
Step 3: Initialize the random seed using the current time.<br>
Step 4: Generate a random number by calculating the remainder of division with the range
(max - min + 1) and adding the minimum value.<br>
Step 5: Repeat the random number generation for the specified count.<br>
Step 6: Print each generated random number.<br>
Step 7: End the program.<br>

## PROGRAM : -

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main()
{
 int count, min, max;
 printf("Enter the number of random numbers to generate: ");
 scanf("%d", &count);
 printf("Enter the minimum value: ");
 scanf("%d", &min);
 printf("Enter the maximum value: ");
 scanf("%d", &max);
 srand(time(NULL));
 printf("Pseudorandom numbers:\n");

 for (int i = 0; i < count; i++)
 {
 int random_number = (rand() % (max - min + 1)) + min;
 printf("%d\n", random_number);
 }
 return 0;
}

```
## OUTPUT : -
![Screenshot 2024-10-09 155210](https://github.com/user-attachments/assets/af951326-192d-4203-b2a9-582b75ed3e24)

## RESULT : -
The program for Pseudorandom Number Generation is executed successfully.


