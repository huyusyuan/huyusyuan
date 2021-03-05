### Hi there 👋

## 第一個程式
```C
#include<stdio.h>
int main()
{
 int n1=10,n2=20,n3=30;
 printf("n1:%d n2:%d n3=%d\n", n1, n2, n3);

 int *p = &n1;
  *p = 200;
   printf("n1:%d n2:%d n3=%d\n", n1, n2, n3);
```
因為 P= &n1 的關係 所以要把200框起來然後指向N1的地方

## 第二個程式
```C
#include<stdio.h>
int main()
{
 int n1=10,n2=20,n3=30;
 printf("n1:%d n2:%d n3=%d\n", n1, n2, n3);

 int *p = &n1;
  *p = 200;
   printf("n1:%d n2:%d n3=%d\n", n1, n2, n3);
   
 int *p2 = &n3;
  *p2 = 300;
   printf("n1:%d n2:%d n3=%d\n", n1, n2, n3);
   
   return0;
 }
```

## 第三個程式

```C
#include<stdio.h>
int main()
{
  int n[3]={10,20,30};
  printf("n[0]:%d n[1]:%d n[2]:%d\n", n[0],n[1],n[2]);

  int *p= & n[0];
  *p=200;
  printf("n[0]:%d n[1]:%d n[2]:%d\n", n[0],n[1],n[2]);

  int *p2= &n[2];
  *p2=300;
  printf("n[0]:%d n[1]:%d n[2]:%d\n", n[0],n[1],n[2]);

  p2=p;
  *p2=400;
  printf("n[0]:%d n[1]:%d n[2]:%d\n", n[0],n[1],n[2]);

  return 0;
```
}

