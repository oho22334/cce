# cce 0312

## 錯誤
```C
#include <stdio.h>
int main ()
{
    int a[5]={ 0,10,20,30,40};
    int*p = &a[2];
    *p = 222;
    for(int i=0;i<5;i++)
    printf(" %d",a[i]);printf("\n");
    printf("p心理的小紙條記的值是:%d\n",p);

    p = p+2;
    *p=666;
    for(int i=0;i<5;i++)
    printf(" %d",a[i]);printf("\n");
    printf("p心理的小紙條記的值是:%d\n",p);
    p--;
    *p=555;
    for(int i=0;i<5;i++)
    printf(" %d",a[i]);printf("\n");
    printf("p心理的小紙條記的值是:%d\n",p);
}
```

##
```C
#include <stdio.h>
int main ()
{
    int a[5]={ 0,10,20,30,40};
    int*p = &a[2];
    *p = 222;
    for(int i=0;i<5;i++)
    printf(" %d",a[i]);printf("\n");

    p = p+2;
    *p=666;
    for(int i=0;i<5;i++)
    printf(" %d",a[i]);printf("\n");
    
    p--;
    *p=555;
    for(int i=0;i<5;i++)
    printf(" %d",a[i]);printf("\n");
    
}
```

## 計算陣列平方值

```C
#include <stdio.h>
int main ()
{
	int a[10];int n;
	scanf("%d",&n);
	for(int i=0;i<n;i++){
	scanf("%d",&a[i]);
		printf("%d,",a[i]*a[i]);}
		printf("\n");
		
}
```

## 大小寫轉換 
```C
#include <stdio.h>
int main ()
{
 char a[10];
 scanf("%s",&a);
 for(int i=0;i<10;i++){
 	if(a[i]>='0'&&a[i]<='9')printf("%c",a[i]);
 	else if (a[i]>='A'&&a[i]<='Z')printf("%c",a[i]+32);
 	else if (a[i]>='a'&&a[i]<='z')printf("%c",a[i]-32);
 	else if (a[i]=='\0') break;
 	}
 	printf("\n");
 	}
```
## 計算幾週與幾天 


```C
#include <stdio.h>
int main ()
{
	int n;
	scanf("%d",&n);
	printf("%d %d\n",n/7,n%7);
}
```
## 計程車資計算
```C
#include <stdio.h>
int main ()
{
	int n;
	scanf("%d",&n);
	if(n<=2000)
	printf("100\n");
	else if (n>2000)
	printf("%d\n",((n-2499)/500)*5+100);
}
```
## 整數間最大距離
```C
#include <stdio.h>
int main ()
{
	int a,b,c;
	scanf("%d%d%d",&a,&b,&c);
	if(a>b&&b>c)printf("%d\n",a-c);
	else if(a>c&&c>b)printf("%d\n",a-b);
	else if(b>a&&a>c)printf("%d\n",b-c);
	else if(b>c&&c>a)printf("%d\n",b-a);
	else if(c>b&&b>a)printf("%d\n",c-a);
	else if(c>a&&a>b)printf("%d\n",c-b);
}
```
## 兩數間可被5整除的整數
```C
#include <stdio.h>
int main ()
{
	int x,y ,temp;
	scanf("%d%d",&x,&y);
	if(x>y)
	{
		temp=x;
		x=y;
		y=temp;
	}
	for (int i=x;i<=y;i++)
		if(i%5==0) printf("%d\n",i);
}
```
