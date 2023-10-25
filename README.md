# Menu_driven_distance
#include<stdio.h>
#include<math.h>

void main()
{
int x1,y1,x2,y2,m,d,d1,n;
printf("Enter x1 and y1 coordinates of first point");
scanf("%d %d",&x1,&y1);

printf("Enter x2 and y2 coordinates of second point");
scanf("%d %d",&x2,&y2);

do
{
printf("1.Distance\n");
printf("2.Slope\n");
printf("3.Quadrant\n");
printf("4.Exit\n");
printf("Enter your choice ");
scanf("%d",&n);

switch(n)
{
case 1:
d=(x2-x1)*(x2-x1)+(y2-y1)*(y2-y1);
d1=sqrt(d);
printf("The distance between two points = %f\n",(float )d1);
break;

case 2:
m=((y2-y1)/(x2-x1));
printf("The slope = %d\n",m);
break;

case 3:
if(x1>0 && y1>0  && x2>0 && y2>0 )
printf("Points lies in same quadrant  \n");

else if(x1<0 && y1<0  && x2<0 && y2<0 )
printf("Points lies in same quadrant  \n");

else
printf("Points lies in different quadrant \n");
break;
}
}
while(n!=4);
}
