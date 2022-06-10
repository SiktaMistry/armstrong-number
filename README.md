# armstrong-number
#include<stdio.h>
int main()
{
	int n; int num; 
	int remainder; int result=0;
	printf("Enter a three digit number\n");
	scanf("%d",&n);
	num=n;
	while(num!=0){
		remainder=num%10;
		result+=remainder*remainder*remainder;
		num/=10;
	}
	if(result==n){
		printf("The number is an Armstrong Number");
	}
	else{
		printf("The number is not an Armstrong Number");
	}
	return 0;
}
