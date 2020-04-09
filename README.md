Welcome to GitHub！
#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<string.h>
void main()
{
 int dts=0,zcj=0,*p; /* 答题数，得分 */
 int score[3]={10,7,5};
 char str[10],str1[10][20];
 while(1)
 {
	int a=0,b=0,c=0,d=0,e=0,f=-1,g=0,i=0,result;
		int m=result;
			int *mp=&m;
	char fuhao[2]={'+','-'};/*题目运算符号*/
	g++;
	while(1)
	{
		a=rand()%51;/*a取0-50之间的随机数*/
		b=rand()%51;/*b取0-50之间的随机数*/
		d=rand()%2;/*运算符号随机*/
		a+b>50||a+b<0||a-b>50||a-b<0;/*结果在0-50以内的非负数*/
	if(d==0)c=a+b;
	else c=a-b;
	if(c>=0 && c<=50)/*遇见题目相同时重新出题*/
	{
		sprintf(str,"%d %c %d = ",a,fuhao[d],b);
		strcpy(str1[dts],str);
		if(dts==0) break;
    f=-1;
	for(g=0;g++;)
	{
		if(strcmp(str,str1[i])==0)
		{
			f=1;break;
		}
	}
    for(i=0; i<dts;i++)
	{
		if(strcmp(str,str1[i])==0)
		{
			f=1;break;
		}
	}
	if(f<0)
		break;
	}
	}
	printf("%s\n",str);/*输入答案*/
	printf("输入计算结果:\n");
	while(1)
	{
		scanf("%d",&result);
		e++;
		if(result==!c)
		{
			printf("答案还是错误哦，要多加练习啊，该题答案为:\n",result);
			break;
		}
		if(result==c)
		{
			printf("恭喜你，回答正确！\n");
			zcj+=score[e-1];
			break;
		}
		else if(e>0&&e<3)
		{
			printf("答案错误，请再思考一下~:\n");
		}
		else 
		{
			printf("答案还是错误哦，要多加练习啊，该题答案为:\n",c);/*三次错误后输出答案*/
			break;
		}
	}
	dts++;
	if(dts>=10)break;
	}
	if(zcj>=90)printf("\nSMART\n");	
	else if(zcj<=90&&zcj>=80)printf("\nGOOD\n");
	else if(zcj<=80&&zcj>=70)printf("\nOK\n");
	else if(zcj<=70&&zcj>=60)printf("\nPASS\n");
	else if(zcj<=60)printf("\nTRY AGAIN\n");
	printf("你的最终成绩是：%d\n",zcj);
  getch();
}
