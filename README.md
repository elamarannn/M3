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
~~~
#include <stdio.h>
#include <math.h> 
float calculateEMI(float principal, float annualRate, int tenureMonths) {
    float monthlyRate = annualRate / (12 * 100);
    float emi = (principal * monthlyRate * pow(1 + monthlyRate, tenureMonths)) / (pow(1 + monthlyRate, tenureMonths) - 1);
    return emi;
}
int main() {
    float principal, annualRate;
    int tenureMonths;
    scanf("%f", &principal);
    scanf("%f", &annualRate);
    scanf("%d", &tenureMonths);

    if (principal <= 0 || annualRate <= 0 || tenureMonths <= 0) {
        printf("Invalid input. Please enter positive values.\n");
        return 1;
    }
    float emi = calculateEMI(principal, annualRate, tenureMonths);
    printf("Your EMI is: %.2f\n", emi);
    return 0;
}

~~~

## OUTPUT

![image](https://github.com/user-attachments/assets/4d00b356-3c03-426a-9079-091caa32e675)




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
~~~
#include <stdio.h>
int fibonacci(int n)
{
    int a=0,b=1,c,i;
    for (i=1;i<=n;++i){
        printf("%d ",a);
        c=a+b;
        a=b;
        b=c;
    }
    return 0;
}
int main()
{
    int n;
    scanf("%d",&n);
    fibonacci(n);
    return 0;
}
~~~
## OUTPUT


![image](https://github.com/user-attachments/assets/7482f0c3-40b6-48bb-9edf-eee1c87ad050)






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
~~~
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The Last Element of the array is %d\n", arr[n-1]);
    return 0;
}
~~~
## OUTPUT
![image](https://github.com/user-attachments/assets/c3cd16ab-111a-4de6-bbee-675dfb37643c)









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
~~~
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i=0;i<n;i++){
        if (arr[i]>0){
            printf("The positive array are : %d",arr[i]);
        }
    }
    return 0;
}
~~~

## OUTPUT

![image](https://github.com/user-attachments/assets/62e40c71-9a5c-4baf-b0e7-db8be567c47f)




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
~~~
#include <stdio.h>
int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The replaced array are : ");
    for (int i=0;i<n;i++){
        if (arr[i]%2==0){
            printf("E ");
        }else{
            printf("%d ",arr[i]);
        }
    }
    return 0;
}
~~~
## Output:
 
![image](https://github.com/user-attachments/assets/36a1346b-38e8-43c1-8f38-b9014a3ddef4)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



