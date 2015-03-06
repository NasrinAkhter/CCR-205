# CCR-205

5.2  Write a program to find the number of and sum of all integers greater than 200 that are divisible by 7.       
C code:  
 #include<stdio.h>
int main(){
    int i,sum;
  	for(i=112;i<=200;i=i+7){
    sum=sum%7;
    printf("%d\n",i);
}
}

Output :
112
119
126
133
140
147
154
161
168
175
182
189
196	


5.12    An electricity board charges the following rates for the  use of electricity:
For the first 200 units: 80 P per unit
For the next 100 units: 90 P per unit
Beyond 300 units: Rs 1.00 per unit
All users are charged a minimum of Rs. 100 as meter charge. If total amount is more than Rs. 400, then the additional surcharge of 15 % of total amount is charged. Write a program to read the names of users and number of units consumed and print out the names.


C Code :
#include<stdio.h>
int main() {
    char name[20];
    float units;
    printf("Enter consumer's name: ");
    scanf("%s",name);
    printf("Enter the amount of units consumed : ");
    scanf("%f",&units);
    if(units<=200.00)
    printf("%s has to pay $%f\n",name,100+units*0.80);
    else if(units<=300.00)
    printf("%s has to pay $%f\n",name,100+0.90*units);
    else
    printf("%s has to pay $%f\n",name,units+units*0.15+100);
    return 0;
 }
 
Output:
Enter consumer's name: Nasrin
Enter the amount of units consumed : 345
Nasrin has to pay $496.75



 5.13 Write a program to compute and display the sum of all integers that are divisible by 6 but not divisible by 4 and lie between 0 and 100. The program should also count and display the number of such values.

 
C code:
#include<stdio.h>
int main(){
    int i,count=0;
    for(i=0;i<=100;i++){
    if(i%6==0&&i%4!=0){
    printf("%d\n",i);
    count=count+1;
    }
    }
    printf("count=%d\n",count);
}


Output:
6
18
30
42
54
66
78
90
count=8

