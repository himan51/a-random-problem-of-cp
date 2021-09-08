//# hello-world
//getting started with github
#include<bits/stdc++.h>
using namespace std;
void fun ()
{
	int a;
	cin>>a;
	if (a==1)
	{
		cout<<1<<" "<<1<<"\n";
	}
	if (a==2)
	{
		cout<<1<<" "<<2<<"\n";
	}
	for (int i=2;i<a;i++)
	{
		if ((i*i-i+1)<=a&&i*i>=a)
		{
			cout<<i<<" "<<i*i-a+1<<"\n";
			return;
		}
		if (a<i*i-i+1&&a>=i*i-i+1-i+1)
		{
			cout<<i-(i*i-i+1-a)<<" "<<i<<"\n";
			return;
		}
 	}
}
int main()
{
	ios_base::sync_with_stdio(0);cin.tie(0);
	int t;
	cin>>t;
	while(t--)
	{
		fun();
	}
}
