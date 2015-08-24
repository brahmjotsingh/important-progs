# important-progs
#include<iostream>

using namespace std;

int main()
{
	int i,j,k,m;
	long long arr[100][100];
	cin>>k;
	for(i=0;i<k;i++)
	{
			for(m=0;m<(k)-i;m++)
				cout<<" ";
			for(j=0;j<=i;j++)
			{
				
				if(j==0 || i==j)
					arr[i][j]=1;
				else
					arr[i][j] = arr[i-1][j]+arr[i-1][j-1];
				cout<<arr[i][j]<<" ";
			}
		cout<<endl;
	}
}
