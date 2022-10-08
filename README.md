# 7
试题



//从大到小输入三个数
int main()
{
	int a = 0;
	int b = 0;
	int c = 0;
	scanf("%d,%d,%d", &a, &b, &c);//%d之间有，则输入也要有，
	//算法实现
	//a放最大值
	//b次之
	//c放最小值
	if (a < b)
	{
		int tmp = a;
		a = b;
		b = tmp;
	}
	if (a < c)
	{
		int tmp = a;
		a = c;
		c = tmp;
	}
	if (b < c)
	{
		int tmp = b;
		b = c;
		c = tmp;
	}
	printf("%d%d%d\n", a, b, c);
	return 0;
}


//打印3的倍数
int main()
{
	int i = 0;
	for (i = 1; i <= 100; i++)
	{
		if (i % 3 == 0)
			printf("%d",i);
	}
	return 0;
}





//求公倍数
int main()
{
	int m = 0;
	int n = 0;
	int r = 0;
	scanf("%d%d", &m, &n);
	while (m % n)
	{
		r = m % n;
		m = n;
		n = r;
	}
	printf("%d\n", n);
	return 0;
}
