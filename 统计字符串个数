#include<stdio.h>
#include<string.h>
int main()
{
	char ch[1000],a[10];
	char *pa;
	pa=a;
	int x,y,i,z=0;
	printf("请输入一个句子\n");
	fgets(ch,1000,stdin);//得到英文句子 
	printf("请输入要计数的单词\n");
	fgets(a,10,stdin);//待需要统计的字符串 
	strlwr(ch);
	
	for(i=0;i<strlen(ch)-1;i++) 
	{
		if(ch[i]==a[0])
		{
			for(x=1,y=1; x<strlen(a)-1 && ch[i+x]==*(pa+x); x++)
			{
				y++;
			}
			if(y==strlen(a)-1)
			{
				z++;
				i+=strlen(a)-2; 
			}
		}
	}
	printf("有%d个\n",z);
	return 0;
}
