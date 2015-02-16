//Decreasing order
#include <iostream>
using namespace std;

void insertion_sort(int arr[],int n)
{
  int key,i;
  for(int j=1;j<n;j++)
  {
	 // set key as the current element
	 key=arr[j];
	 i=j-1;
	 //compare the previous element with key 
	//if key is smaller than arr[i] push the elements one step right
	 while(i>=0 && arr[i]<key)
	 {

		arr[i+1]=arr[i];
		 i=i-1;
	 }
	 //store the key in the appropriate place
	 arr[i+1]=key;
  }
  //return arr[i];
}

// Controls operation of the program
void main () 
{
	int A[5]={100,105,96,154,0};
	int s=5;
	insertion_sort(A,s);
	for(int j=0;j<5;j++)
		{
			cout<<A[j]<<"\n";
		}
	//return 0;
	system("pause");
}
