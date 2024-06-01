- 👋 Hi, I’m @Rohit-athi
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Rohit-athi/Rohit-athi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--
#include<stdio.h>

#include<conio.h>

#include<stdlib.h>

void main()

{

FILE *fp1,*fp2;

int i,n,num;

clrscr();

fp1=fopen("even.txt","w");

fp2=fopen("odd.txt","w");

printf("enter the no of element:");

scanf("%d",&n);

printf("\n enter %d number:",n);

for(i=0;i<n;i++)

{

 scanf("%d",&num);

 if(num%2==0)

 putw(num,fp1);

 else

 putw(num,fp2); }

 fclose(fp1);

 fclose(fp2);

 fp1=fopen("even.txt","r");

 fp2=fopen("odd.txt","r");

 printf("\n contents of even numbes file:\n");

 while((num=getw(fp1))!=EOF)

 {

 printf("%d\n",num);

 }

printf("\n contents of odd numbers file:\n");

while((num=getw(fp2))!=EOF)

{

 printf("%d\n",num);

}

 fclose(fp1);

 fclose(fp2);

 getch();

}
