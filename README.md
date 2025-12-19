# C Module -2
# PROGRAM---2

## Exp no -2(a) L1 Loops
### Name : DEEPAK PRABHAKARAANN VB
### Reference number : 25011420
### Date :  20.12.25
# Aim
Write a C program to print odd numbers ranging from M to N (including M and N values) in reverse order.
# Algorithm
- Start
- Input values: Read two integers M and N.
- Assume M ≤ N.
- If not, you can swap them or handle accordingly.
- Initialize loop variable: Set i = N.
- Loop condition: While i >= M, do the following:
- Check oddness: If i % 2 != 0, then i is odd.
- Print: Display the value of i.
- Decrement: Reduce i by 1 (i = i - 1).
- End loop when i < M.
- Stop.
## Program
```
#include<stdio.h>
int main()
{
    int n1,n2,a;
    scanf("%d %d",&n1,&n2);
    for(a=n2;a>n1;a--)
    {
        if(a%2!=0)
        {
        printf("%d ",a);
        }
    }
    return 0;
}
```
## Output
<img width="1181" height="261" alt="image" src="https://github.com/user-attachments/assets/fe346ed6-5828-4227-a4bf-00e9bc8c0091" />
# Result
Thus the program to print odd numbers ranging from M to N (including M and N) in reverse order has been successfully executed.


## Exp no -2(b) Nested Loops
### Nmae : DEEPAK PRABHAKARAANN VB
### Reference number : 25011420
### Date : 20.12.25
# Aim
Write a C program for the following pattern:

            %

             % %

               % % %

                 % % % %

               % % %

             % %

           %
# Algorithm
- Start
- Input: No input required (pattern size is fixed here as 4 rows up and 3 rows down).
- Define structure:
- The pattern has two parts:
- Upper half (increasing): 1 to 4 % symbols.
- Lower half (decreasing): 3 down to 1 % symbols.
- Each line has leading spaces to align the % symbols diagonally.
- Process upper half:
- For i = 1 to 4 (row counter):
- Print (i-1) spaces.
- Print i % symbols separated by a space.
- Move to next line.
- Process lower half:
- For i = 3 down to 1:
- Print (i-1) spaces (but aligned to continue the diagonal).
- Print i % symbols separated by a space.
- Move to next line.
- Stop
## Program 
```
#include<stdio.h>
int main()
{
    int i,j;
   for(i=1;i<5;i++)
   {
       printf(" ");
       for(j=0;j<=i+3;j++){
           printf("  ");
       }
       
       
       for(j=1;j<=i;j++)
       {
           
           printf("%% ");
       }
       printf("\n");
      
   }
   
   for(i=3;i>=1;i--){
      printf(" "); 
       for(j=i+3;j>=0;j--){
           printf("  ");
       }
       
       
       for(j=i;j>=1;j--){
           printf("%% ");
       }
       printf("\n");
      
   }
}
```
## Output
<img width="1182" height="410" alt="image" src="https://github.com/user-attachments/assets/acd5b99c-045d-49c1-8e32-dc35845eecf2" />
# Result
Thus the program to display the pyramid‑shaped pattern of % symbols has been successfully executed.


## Exp no -2(c) Functions in C
### Name : DEEAPK PRABHAKARAANN VB
### Reference number : 25011420
### Date ; 20.12.25
# Aim
Write a C program to perform addition and subtraction of two numbers using function (without argument and without return type.
# Algorithm
- Start
- Declare functions:
- void add(); → performs addition.
- void subtract(); → performs subtraction.
(Both functions will not take arguments and will not return values.)
- Inside main():
- Call the add() function.
- Call the subtract() function.
- In add() function:
- Declare two integer variables a and b.
- Input values for a and b from the user.
- Compute sum = a + b.
- Print the result.
- In subtract() function:
- Declare two integer variables x and y.
- Input values for x and y from the user.
- Compute diff = x - y.
- Print the result.
- End program.
## Program 
```
#include<stdio.h>
void add();
void sub();
int main()
{
    add();
    sub();
}
void add()
{
    int n,m;
    scanf("%d %d",&n,&m);
    printf("Addition: %d\n",n+m);
}
void sub()
{
    int k,l;
    scanf("%d %d",&k,&l);
    printf("Subtraction: %d",k-l);
}
```
## Output
<img width="1177" height="267" alt="image" src="https://github.com/user-attachments/assets/d7f11899-958c-4e4e-8bf8-791f0ed7e051" />
# Result
Thus the program to perform addition and subtraction of two numbers using functions without arguments and without return type has been successfully executed.


## Exp no -2(d) Loops
### Name : DEEPAK PRABHAKARAANN VB
### Reference number : 25011420
### Date : 20.12.25
# Aim
Write a c program to find the sum of digits using while loop without using modulus operator
# Algorithm
- Start
- Input: Read an integer num.
- Initialize: Set sum = 0.
- Loop condition: While num > 0, do the following:
- Extract last digit without %:
- Use integer division and multiplication.
- digit = num - (num / 10) * 10
(This effectively gives the remainder when divided by 10, but without %.)
- Add digit to sum: sum = sum + digit.
- Remove last digit: num = num / 10.
- End loop when num == 0.
- Output: Print the value of sum.
- Stop.
## Program
```
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    i=n;
    int sum=0;
    while(i>0)
    {
        sum+=i-(i/10*10);
        i/=10;
    }
    printf("%d",sum);
}
```
## Output
<img width="1180" height="295" alt="image" src="https://github.com/user-attachments/assets/b76948a2-1e36-4c37-a3e9-82446763f8a6" />
# Result 
Thus the program to find the sum of digits of a number using a while loop without using the modulus operator has been successfully executed.


## Exp no -2(e) Functions im C
### Name : DEEPAK PRABHAKARAANN VB 
### Refernce number : 25011420
### Date : 20.12.25
# Aim
Write a C program to perform addition and subtraction of two numbers using function (without argument and without return type).
# Algorithm 
- Start
- Declare functions:
- void add(); → performs addition.
- void subtract(); → performs subtraction.
(Both functions will not take arguments and will not return values.)
- Inside main():
- Call the add() function.
- Call the subtract() function.
- In add() function:
- Declare two integer variables a and b.
- Input values for a and b from the user.
- Compute sum = a + b.
- Print the result.
- In subtract() function:
- Declare two integer variables x and y.
- Input values for x and y from the user.
- Compute diff = x - y.
- Print the result.
- End program.
## Program
```
#include<stdio.h>
void add();
void sub();
int main()
{
    add();
    sub();
}
void add()
{
    int n,m;
    scanf("%d %d",&n,&m);
    printf("Addition: %d\n",n+m);
}
void sub()
{
    int k,l;
    scanf("%d %d",&k,&l);
    printf("Subtraction: %d",k-l);
}
```
## Output
<img width="1210" height="278" alt="image" src="https://github.com/user-attachments/assets/5c7192c8-ae6a-4655-bd94-c50b943c932f" />
# Result 
Thus the program to perform addition and subtraction of two numbers using functions without arguments and without return type has been successfully executed.









           
           

