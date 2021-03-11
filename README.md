# cce



```
## 第十一題 均標與前標計算
```c
#include <stdio.h>
int main()
{
	int N;
	scanf("%d",&N);
	
	int sum=0;
	int a[1000];
	for(int i=0;i<N;i++){
		scanf("%d",&a[i]);
		sum+=a[i];
		}
	float average;
	average=(float)sum/N;
	float r=0;
	float sumTop=0;
	for(int i=0;i<N;i++){
		if(a[i]>=average){
			sumTop+=a[i];
			r++;
			}
		}
	float averageTop;
	averageTop=(float)sumTop/r;
	printf("均標:%.1f\n",average);
	printf("前標:%.1f\n",averageTop);
}
	


```
