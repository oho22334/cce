# cce 0312

##錯誤
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

##計算陣列平方值

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
