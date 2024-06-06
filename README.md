# Wave-array
Make a wave array sequence where a1>=a2&lt;=a3>=a4&lt;=a5
#include<iostream>
#include<bits/stdc++.h>
using namespace std;

int main(){
	int n;
	cout<<"Enter the size: ";
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];
	}
	sort(arr,arr+n);
	for(int i=0;i<n;i++){
		cout<<arr[i]<<" ";
	}
	for(int i=0;i<n;i+2){
		int temp=arr[i];
		arr[i]=arr[i+1];
		arr[i+1]=temp;
	}
	for(int i=0;i<n;i++){
		cout<<arr[i]<<" ";
	}
	
}
