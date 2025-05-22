# EX-16-LEFT-SHIFT-OPERATION AND RIGHT-SHIFT-OPERATION
## AIM
Write a C program to perform the basic left and right shift operation.  

## ALGORITHM

1.Start the program.
2.Input an integer value from the user and store it in variable a.
3.Perform a left shift operation on a by 2 bits (a << 2) and display the result.
4.Perform a right shift operation on a by 2 bits (a >> 2) and display the result.
5.End the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    printf("After Left Shift Operation value of a is:%d\n",a<<2);
    printf("After Right Shift Operation value of a is:%d\n",a>>2);
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/034eb037-4077-428d-a7d3-5cb699da5ccf)


## RESULT
Thus the program to perform the basic left shift operation  and right shift operation has been executed successfully.




 
 


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
```
#include <stdio.h>

int main()
{
    int num1,num2;
    
    scanf("%d %d", &num1,&num2);
    

    if(num1== num2)
    {
        printf("Numbers are Equal");
    }
    if(num1!= num2)
    {
        printf("Numbers are not Equal");
    }
    

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/22a1fb2f-9826-4f53-a8ac-f5924d8e0ea8)

           
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
```
#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main() {
    char Str[100];

    
    fgets(Str, sizeof(Str), stdin);


    Str[strcspn(Str, "\n")] = '\0';

    
    for (int i = 0; Str[i]; i++) {
        Str[i] = tolower(Str[i]);
    }

    printf("Lower case String is:%s\n", Str);

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/9eea66c6-8f08-4792-b5a7-385ee881a4d8)



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully.
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using for loop.

## ALGORITHM

1.Start the program and declare a string s.
2.Read a full line of text into s.
3.Initialize count = 0.
4.Loop through s and increment count when a new word starts.
5.Print count and end the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
    char s[100];
    scanf("%[^\n]",s);
    int i,count=0;
    for(i=0;s[i]!='\0';i++)
    {
        if((s[i-1]==' '&&s[i]!=' ')||(i==0 && s[i]!=' '))
        count++;
    }
    printf("%d",count);
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/73646cde-5d17-4ee5-ad7c-8c22cf379db6)



## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM

1.Start the program and declare two character arrays (str1, str2).
2.Read two strings (lines) from the user using fgets.
3.Remove newline characters from both strings using strcspn.
4.Compare characters of both strings one by one using a loop.
5.If all characters match, print "strings are same"; otherwise, print "strings are not same".


## PROGRAM
```
#include <stdio.h>
#include<string.h>
int main() {
    char str1[100], str2[100];
    int i = 0, flag = 0;

    
    fgets(str1, sizeof(str1), stdin);
    
    fgets(str2, sizeof(str2), stdin);

    
    str1[strcspn(str1, "\n")] = '\0';
    str2[strcspn(str2, "\n")] = '\0';

    
    while (str1[i] != '\0' || str2[i] != '\0') {
        if (str1[i] != str2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if (flag == 0)
        printf("strings are same\n");
    else
        printf("strings are not same\n");

    return 0;
}
```

## OUTPUT
 
![image](https://github.com/user-attachments/assets/630dc19c-5005-4baa-b53f-3ec066ea1dac)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

