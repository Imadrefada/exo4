# exo4
#include<stdio.h>
#include<stdlib.h>
#include<string.h>

struct temps{
 int h;
 int m;
 int s;
};
struct temps lecture(struct temps *T){

 printf("entre t1 h(0-24):m(0-59):s(0-59)");
 scanf("%d",&(T ->h));
 scanf("%d",&(T ->m));
 scanf("%d",&(T ->s));}

 void print(struct temps *t){

  printf(" the time is :%02d:%02d:%02d\n",t->h,t->m,t->s);
}



struct temps diff(struct temps*tstart,struct temps *tend){
  int s1,s2 s3;
  struct temps sdff;
 s1=(tstart->h*3600+tstart->m*60+htstart->s);
 s2=(tend->h*3600+tend->m*60+hend->s);
 s3=s1-s2;
   if(s3<0){
   s3=s3*(-1);
 }
  sdff->h=s3%3600;
  sdff->m=mod(s3,3600);
  sdff->s=mod(m,60);
  printf(" the deff  btw the start time and end time is : %d:%d:%d\n",sdff->h,sdff->m,sdff->s);
}
//variabels:// 
struct  temps t1;
struct  temps t2;
struct  temps T ;
struct temps tend,start;
 struct temps sdff;
int main(){
 
 lecture(&t1);
 print(&t1);
 lecture(&t2);
 print(&t2);
 diff(&t1,&t2);
 return 0;}
