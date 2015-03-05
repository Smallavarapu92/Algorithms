
#include<iostream>
using namespace std;
int main()
{
	int n=0,i=0;
	cout<<"\nEnter the size of the array\n";
	cin>>n;
	int *A= new int[n];
	cout<<"\n Please enter a list of postive values:\n";
	while(i<n)
	{
		cin>>A[i];
		i++;
	}
	cout<<"\nEnd of the array";
	cout<<"\n Entered array is: ";
	for(int i=0;i<n;i++)
		cout<<"\t"<<A[i];






	system("pause");
}
