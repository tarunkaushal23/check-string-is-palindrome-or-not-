#include<iostream>
using namespace std;
int main()
{
	string str="abc";
	int n=str.length();
	bool s;
	char arr[n];
	int j=0;
	for(int i=str.length()-1;i>=0;i--)
	{
		arr[j]=str[i];
		j++;
	}
	
	for(int i=0;i<str.length();i++)
	{
		if(str[i]==arr[i])
		{
			s=true;
		}
		else
		{
			s=false;
			break;
		}
	}
	if(s==true)
	{
		cout<<"String is a Palindrome";
	}
	else{
		cout<<"String is not a palindrome";
	}
}
