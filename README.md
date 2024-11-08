# question.practice
 Q.1    c++ program to find largest number among three numbers
#include<iostream>
using namespace std;<br>
 
int main(){
 int n,b,m;
cout<<"enter your number "<<endl;
cin>>n>>b>>m;
// check if n largest number:
if(n>=b && n>=m){
    cout<<"largest number"<<n;

}
else if (b>=n && b>=m){
    cout<<"largest number"<<b;

}
// if neither n and b are the largest , m is the largest
else
cout<<"largest number"<<m;
    return 0;
}
