# CALCULATOR
#include<stdio.h>

int main()
{
    int n1,n2;
    char sy;
    printf("Enter the symbole\n");
    scanf("%c",&sy);
    printf("Enter the Numbers\n");
    scanf("%d%d",&n1,&n2);
    switch(sy){
        case '+':
        printf("Sum is = %d",n1+n2);
        break;
        case '-':
        if (n1>n2)
        {
            printf("Minus is = %d",n1-n2);
        }
        else{
        printf("Minus is = %d",n2-n1);
        }
        break;
        case '/':
              if (n1>n2)
        {
            printf("Division is = %d",n1/n2);
        }
        else{
        printf("Divisiom is = %d",n2/n1);
        }
        break;
        case '*':
        printf("Product is %d",n1*n2);
        break;
        case '%':
        if (n1>n2)
        {
            printf("Reminder is = %d",n1%n2);
        }
        else{        
        printf("Reminder is = %d ",n1%n2);
        }
        break;
        default:
        printf("Invalid Symbol");
    }
    return 0;
}
