#include<stdio.h>
int main()
{
    int n,a[10],i,j,t;

    printf("enter n:");
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    scanf("%d",&a[i]);
    for(int i=0;i<n;i++)
    {
        for(j=i+1;j<n;j++)
        {
            if(a[j]>a[j+1])
            {
                t=a[i];
                a[i]=a[j];
                a[j]=t;
            }
            
        }
    }
    printf("sort");
    for(i=0;i<n;i++)
    printf("%d\n",a[i]);
    return 0;
}
output:
enter n:3
6
5
2
sort:2
5
6
