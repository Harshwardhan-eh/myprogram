*/ write a program to find out the given sentence is a snowball or not.*/
#include<stdio.h>
#include<conio.h>
#include<string.h>
void main()
{
int i,f,ac1=0,ac2=0,I,flag;
char str[40];
clrscr();
printf("Enter the string :");
gets(str);
I=strlen(str);
for(i=0;i<I;i++){
if(str[i]!=32){
ac1=ac1+1;
continue;
}
else{
if(ac1>=ac2+1){
ac2=ac1;
ac1=0;
continue;
}
else{
flag=1;
break;
}
}
}
printf("\n Output: \n");
if(flag==1)
printf("\nSentence is not a snowball sentence",str);
else
printf("\nSENTENCE is a snowball sentence",str);
getch();
}
