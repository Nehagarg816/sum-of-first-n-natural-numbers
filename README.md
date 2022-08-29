# sum-of-first-n-natural-numbers
This is a program of finding sum of first n natural numbers using recursion in functions.
#include<stdio.h>
#include<conio.h>
int average(int a);

void main()
{
	int a,s;
	printf("Enter one number a:");
	scanf("%d",&a);
	s=average(a);
	printf("Sum of first a numbers is %d",s);
}
int average(int x)
{
	int sum;
	if(x==1)
	{
		return 1;
	}
	else
	{
		sum=x+average(x-1);
	}
	return(sum);
}
