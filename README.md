# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int a = 44, b = 3;
    int result = a << b;
    printf("%d\n", result);
    return 0;
}
```
## OUTPUT
<img width="1632" height="778" alt="C-16" src="https://github.com/user-attachments/assets/8fec09b8-e3fc-4112-9415-811d0bc9ddf9" />









## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int a, b;
    scanf("%d %d", &a, &b);
    if (a == b)
        printf("Both are equal\n");
    else
        printf("Both are not equal\n");
    return 0;
}
```
## OUTPUT
 <img width="1632" height="780" alt="C-17" src="https://github.com/user-attachments/assets/b85b9574-0f9e-46b7-9c19-704ef5a4db56" />
          
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];
    int i = 0;
    fgets(str, sizeof(str), stdin);
    while (str[i]) {
        str[i] = tolower(str[i]);
        i++;
    }
    printf("%s", str);
    return 0;
}
```
## OUTPUT
<img width="1635" height="787" alt="C-18" src="https://github.com/user-attachments/assets/bb1745f8-7536-47bd-abbe-27b709e94b02" />




## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    char str[100];
    int count = 0, i;
    fgets(str, sizeof(str), stdin);
    for (i = 0; str[i] != '\0'; i++) {
        if (str[i] == ' ')
            count++;
    }
    printf("%d\n", count);
    return 0;
}
```
## OUTPUT
<img width="1632" height="782" alt="C-19" src="https://github.com/user-attachments/assets/044b8480-06c8-410f-a6df-16b56e489611" />





## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int flag = 0, i = 0;
    scanf("%[^\n]", c1);
    getchar(); 
    scanf("%s", c2);
    while (c1[i] != '\0' && c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }
    if (flag == 0 && c1[i] == '\0' && c2[i] == '\0')
        printf("strings are same\n");
    else
        printf("strings are not same\n");
    return 0;
}
```
## OUTPUT
 <img width="1630" height="782" alt="C-20" src="https://github.com/user-attachments/assets/ff074bff-f49f-441b-ae20-07332d05e2f9" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

