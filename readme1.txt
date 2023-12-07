//squaring array element and palced in accending order
#include <iostream>

using namespace std;

int main()
{
    int j,temp, n,i,a[10],b[20];
    cout<<"enter the number\n";
    cin>>n;
    cout<<"enter the array elements:\n";
    for(i=0;i<n;i++)
    cin>>a[i];
    for(i=0;i<n;i++)
    
    {
    b[i]=a[i]*a[i];
    }
    for(i=0;i<n;i++)
    for(j=0;j<n-1;j++)
    
    if (b[j]>b[j+1])
    {
    temp=b[j];
       b[j]=b[j+1];
     b[j+1]=temp;
   }
    cout<<"squares\n";
    for(i=0;i<n;i++)
cout<<b[i]<<"\n";
    return 0;
}
