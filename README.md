# linear-search
#include<stdio.h>
#define max 50
int main()
{
    int a[max],i,x,n,flag;
    flag=0;
    printf("How many elements?");
    scanf("%d",&n);
    printf("Enter array elements:\n");
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("\nEnter element to search: ");
    scanf("%d",&x);
    for(i=0;i<n;i++)
    {
        if(a[i]==x)
            flag=1;
            break;
    }
    if(flag==1)
    {
        printf("Element %d is found\n",x);
    }
    else
    {
        printf("Element %d is not found\n",x);
    }
}

OUTPUT:
How many elements?5
Enter array elements:
1
5
9
7
3

Enter element to search: 3
Element 3 is not found
