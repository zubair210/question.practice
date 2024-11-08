# question.practice
 # Q.1   c++ program to find largest number among three numbers

 
#include<iostream>
using namespace std;
 
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

# Q . 2 // c++ program to check whether a character is vowel or consonant //
#include<iostream>
using namespace std;
char n ;

int main(){
cout<<"enter your character "<<endl;
cin>>n;

if((n=='a'||n=='e'||n=='o'||n=='i'||n=='u'||
    n=='A'||n=='E'||n=='O'||n=='I'||n=='U')){
    cout<<"this alphabet is vowel"<<endl;
}
     else{
        cout<<"this alphabet is consonant"<<endl;
    }
return 0;
}



