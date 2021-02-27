# employee
details of the employee
#include <stdio.h>

 
typedef struct{
 
    char name[30];
    int phone_no;
    int age;
    int salary;
 
}Employee;
 
int main()
{
    int i, n=3;
 
    Employee employees[n];
 
    //Taking each employee detail as input
 
    printf("Enter %d Employee Details \n \n",n);
    for(i=0; i<n; i++){
 
        printf("Employee %d:- \n",i+1);
        //Name
        printf("Name: ");
        scanf("%s",employees[i].name);
        //phone_no
        printf("phone_no: ");
        scanf("%d",&employees[i].phone_no);
        //age
        printf("age:");
        scanf("%d",&employees[i].age);
        //Salary
        printf("Salary: ");
        scanf("%d",&employees[i].salary);
 
        printf("\n");
    }
 
    //Displaying Employee details
 
    printf("All Employees Details \n");
 
    for(i=0; i<n; i++){
 
        printf("Name \t: ");
        printf("%s \n",employees[i].name);
 
        printf("phone_no \t: ");
        printf("%d \n",employees[i].phone_no);
        printf("age \t: ");
        printf("%d \n",employees[i].age);
 
        printf("Salary \t: ");
        printf("%d \n",employees[i].salary);
 
        printf("\n");
    }
 
    return 0;
 
}
