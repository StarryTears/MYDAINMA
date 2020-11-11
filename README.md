##include <stdio.h>
int iswanshu(int x);
void main()
{
	int i;
	for(i=1;i<=1000;i++)
	{
		if(iswanshu(i)==1 /*调用iswanshu函数判断是否是完数(1)*/ )
			printf("%d ",i);
	}
}
//iswanshu函数判断某个数是不是完数
int iswanshu(int x)
{
	int i,sum=0;
	for(i=1;i<6/*(2)*/;i++)
	{
		if(x%i==0)
			sum += i;
	}
	if(x==sum /*(3)*/)
		return 1;
	else
		return 0;
}
