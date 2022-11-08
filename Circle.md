#include<stdio.h>
//#include<maths.h>

//Declaring pie
const int pie =3.14;

void all()
{
float k;
printf("Give Input :");
scanf("%f",&k);

printf("Circumference : %.2fcm \nArea : %.2fcm",k*2*pie ,pie*k*k);
}


void basic()
{
 float k;
printf("Give Input :");
scanf("%f",&k);

float h= k/(2*pie);
printf("Radius : %.2fcm \nArea : %.2fcm",h ,pie*h*h);
}

int main()
{
    //Variable Declaration
int opt;    
    
    //Taking Case 
 printf("What You know about the Circle :\n");
 printf("[1 for Radius,2 for Circumference]\n");
 scanf("%d",&opt);
 
 //Applying Cases
 switch(opt)
 {
     case 1:
        all();
        break;
    
    case 2:
        basic();
        break;
    default:
    printf("Provide Right Input \n");
     }
return 0;    
}
