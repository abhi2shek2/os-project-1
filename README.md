#include<stdio.h>
#include<stdlib.h>
int main()
{
  double a,b,c,d, e,f,g,h;

  printf("\ntime taken to service a page fault if an empty page is available in milliseconds");
  scanf("%lf",&b);
  printf("\time taken to  modify page in milliseconds ");
  scanf("%lf",&a);
  printf("\n  access time in nanoseconds");
  scanf("%lf",&c);
  printf("\nthe page is modified in percentage");
  scanf("%lf",&g);
  e=(g/100);
  f=(1-e);
  printf("\n access time");
  scanf("%lf",&d);
  printf("\n  acess time is" );
  printf("\n eft: (1- Page Fault)* Memory time+p*modifed*time to service page fault+p*(1-modifed)service time for no page fault");
  h=(d-c)/((e*a*1000000)+(f*b*1000000)-c);
  printf("\n maximum acceptable page-fault rate is %lf",h);
}
