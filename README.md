# leftrotate
#include <stdio.h>
int main()
{ 
   int n,num,a[100],i,j,r,k=0; 
   scanf("%d\n%d",&num,&n); 
   while(num>0) 
   { 
      r=num%10; 
      a[k++]=r; 
      num=num/10;
      j=k;
   }
   for(i=j-n-1;i>=0;i--)
   { 
      printf("%d",a[i]);
   } 
   for(i=j-1;i>=j-n;i--) 
   { 
      printf("%d",a[i]); 
   } 
}
