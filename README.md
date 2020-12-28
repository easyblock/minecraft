# minecraft
personal exercise
//p1152
#include<stdio.h>
#include<math.h>
int main()
{
	int a[10000000], n, k = 0;
	scanf("%d", &n);
	for (int i = 1; i <= n; i++)
		scanf("%d", &a[i]);
	for (int i = 1; i <= abs(n-1); i++)
	{
		int m = 0;
		for (int j = 1; j <= n; j++)
		{
			if (i == a[j])break;
			else m++;
		}
		if (m == n)k = 1;
	}
	if (k == 1)printf("Not jolly");
	else printf("Jolly");
	return 0;
  }
 //only 60 point
