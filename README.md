# C---assignment-for-attendance-on-02.05.2026

## Execute the following programs and create a  document in github with question, code and output and then upload the pdf file generated from github and also give the github link in the submission.

### 1. Write a c program to print all prime numbers between two limits.

PROGRAM:
```
#include <stdio.h>
int main() 
{
    int a,b,i,j,x;
    scanf("%d%d", &a,&b);
    printf("Prime numbers between %d and %d are:\n",a,b);

    for(i=a; i<=b; i++) {
        if(i<2)
            continue;
        x=1;

        for(j=2; j<=i/2; j++) {
            if(i%j==0) {
                x = 0;
                break;
            }
        }
        if(x)
            printf("%d ", i);
    }
    return 0;
}
```

OUTPUT:

<img width="1203" height="703" alt="image" src="https://github.com/user-attachments/assets/6d8f89ed-66d4-421d-997a-20058caefd11" />


### 2. Write a c program to count the number of digits in a number.

PROGRAM:
```
#include <stdio.h>
int main() 
{
    int num,count=0;
    scanf("%d",&num);

    if(num==0)
        count=1;

    while(num!=0) {
        num=num/10;
        count++;
    }
    printf("Number of digits = %d", count);
    return 0;
}
```

OUTPUT:

<img width="1185" height="512" alt="image" src="https://github.com/user-attachments/assets/11b1445c-956f-4953-9d39-7b1f2877ed2b" />


### 3. Write a c program to print the alphabet S in n x n matrix.

PROGRAM:
```
#include <stdio.h>
int main() 
{
    int n,i,j;
    scanf("%d", &n);

    for(i=0; i<n; i++) {
        for(j=0; j<n; j++) {
            if(i==0 || i==n/2 || i==n-1)
                printf("*");

            else if(i<n/2 && j==0)
                printf("*");

            else if(i>n/2 && j==n-1)
                printf("*");

            else
                printf(" ");
        }
        printf("\n");
    }
    return 0;
}
```

OUTPUT:

<img width="1179" height="729" alt="image" src="https://github.com/user-attachments/assets/8494abfb-32c5-493e-abe8-eca4ca56bd87" />


### 4. Write a c program to print the pyramid pattern.
```
   *

  ***

 *****

*******
```

PROGRAM:
```
#include <stdio.h>
int main() 
{
    int i,j,n;
    scanf("%d", &n);

    for(i=1; i<=n; i++) {
        for(j=1; j<=n-i; j++) {
            printf(" ");
        }
        for(j=1; j<=(2*i-1); j++) {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}
```

OUTPUT:

<img width="1182" height="534" alt="image" src="https://github.com/user-attachments/assets/9b7790e2-0724-4f94-93c3-9e32d1571a20" />


### 5. Write a c program to find GCD of two numbers using loop.

PROGRAM:
```
#include <stdio.h>
int main() 
{
    int a,b,i,gcd;
    scanf("%d%d",&a,&b);

    for(i=1; i<=a && i<=b; i++) {
        if(a%i==0 && b%i==0) {
            gcd=i;
        }
    }
    printf("GCD = %d",gcd);
    return 0;
}
```

OUTPUT:

<img width="1174" height="453" alt="image" src="https://github.com/user-attachments/assets/42f08376-fcc4-4707-8870-fed63b91e53b" />
