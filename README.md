# KumkumTest
#include<stdio.h>
#include<math.h>
int main()
{
int i,n;
float a[10],mean,sd,sum,var;
float *p; // p is a pointer to float value
printf("\n Enter Number of elements :");
scanf("%d",&n);
printf("\n Enter the elements :");
p=a; // pointer p points to first element of a
for(i=0;i<n;i++)
{
scanf("%f",p);
p++; // pointer p points to the next element of the array
}
p=a; // Initialize p to the first element of the array
printf("\n input Elements are:\n");
for(i=0;i<n;i++)
{
printf("%f",*p);
p++; // Pointer p is made to point to the next element
}

p=a; // Initialize p to the first element of the array
sum=sd=mean=var=0;
// Find the sum of the array elements
for(i=0;i<n;i++)
{
sum=sum+(*p);
p++;
}
// Find the mean
mean=sum/n;
// Find variance
p=a;
for(i=0;i<n;i++)
