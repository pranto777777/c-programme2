#include <stdio.h>
struct Employe
{char name[50];
int id;
char company_name[50];
float salary;
    
};
void printemploye(struct Employe [] );
int main() {
   struct Employe a[1000];
   int i;float highest;
   for(i=0;i<1000;i++)
   {
       printf("\nEnter the name:");
       scanf("%s",&a[i].name);
       printf("\nEnter the id:");
       scanf("%d",&a[i].id);
       printf("\nEnter the company name:");
       scanf("%s",&a[i].company_name);
       printf("\nEnter the salary");
       scanf("%f",&a[i].salary);
   }

for(i=0;i<1000;i++)
{
   if (a[i].salary>highest)
   highest=a[i].salary;
}
printf("\nHighest salary is %f",highest);
printemploye(a);

    return 0;
}

void printemploye(struct Employe a[])
{
 printf("%s\n",a[3].name);
 printf("\n%d",a[3].id);
 printf("\n%s",a[3].company_name);
 printf("\n%f",a[3].salary);
    
}
