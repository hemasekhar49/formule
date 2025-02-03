#include <stdio.h>

int main()
{
    int r,num,h;
    float volume,csa,tsa,l;
    printf("select shape \n1.cylinder\n2.cube\n3.cone\n4.sphere\n");
    scanf("%d",&num);
    switch(num){
        case 1:printf("enter the radius and height of cylinder:\n");
                scanf("%d%d",&r,&h);
                volume=3.14*r*r*h;
                csa=2*3.14*r*h;
                tsa=2*3.14*r*(r+h);
                printf("volume of cylinder=%f\n",volume);
                printf("curved surface area of cylinder=%f\n",csa);
                printf("total surface area of cylinder=%f\n",tsa);
                break;
        case 2: printf("enter the length of cube=\n");
                scanf("%d",&h);
                volume=h*h*h;
                printf("volume of cube=%f",volume);
                break;
        case 3:printf("enter the radius and height of the cone:\n");
               scanf("%d%d",&r,&h);
               volume=0.33*3.14*r*r*h;
               l=sqrt(r*r*h*h);
               tsa=3.14*r*(r+l);
               csa=3.14*r*l;
               printf("volume of cone=%f\n",volume);
               printf("curved surface area cone=%f\n",csa);
               printf("total surface area of cone=%f\n",tsa);
               break;
        case 4:printf("enter the radius of the sphere:\n");
               scanf("%d",&r);
               volume=0.33*3.14*r*r*r;
               tsa=4*3.14*r*r;
               printf("volume of sphere=%f\n",volume);
               printf("surface area cone=%f\n",tsa);
               break;
        defualt:printf("select a valid shape");
        printf("THE END");
    }

    return 0;
}
