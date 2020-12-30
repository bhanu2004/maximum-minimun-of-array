//maximum-minimun-of-array
#include <iostream>
#include <algorithm>

using namespace std;



int maximum(int arr[],int n){
     int maxm=-999;
    for(int i=0;i<n;i++){
       
        maxm=max(maxm,arr[i]);
    }
    return maxm;
}

int minimum(int *arr,int n){
    int minm=9988;
    for(int i;i<n;i++){
        minm=min(minm,arr[i]);
    }
    return minm;
}
int main()
{
int n;
cin>>n;
int arr[n];
for(int i=0;i<n;i++)cin>>arr[i];
cout<<"maximum value is "<<maximum(arr,n)<<endl;
cout<<"minimum value is "<<minimum(arr,n)<<endl;
return 0;
}
