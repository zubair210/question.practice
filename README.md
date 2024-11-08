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

# Q .3 // when you campare number which number are large , small and middle ;; 
#include <iostream>
using namespace std;

int main() {
    int num1, num2, num3;
    
    // User input for three numbers
    cout << "Enter three numbers: "<<endl;
    cin >> num1 >> num2 >> num3;
    
    int largest, middle, smallest;
    
    // Check for the largest number
    if (num1 >= num2 && num1 >= num3) {
        largest = num1;
        if (num2 >= num3) {
            middle = num2;
            smallest = num3;
        } else {
            middle = num3;
            smallest = num2;
        }
    } else if (num2 >= num1 && num2 >= num3) {
        largest = num2;
        if (num1 >= num3) {
            middle = num1;
            smallest = num3;
        } else {
            middle = num3;
            smallest = num1;
        }
    } else {
        largest = num3;
        if (num1 >= num2) {
            middle = num1;
            smallest = num2;
        } else {
            middle = num2;
            smallest = num1;
        }
    }
    
    // Output the results
    cout << "this team is gold medalist : " << largest << endl;
    cout << "this team achieve a silver medal: " << middle << endl;
    cout << "good game this team is achieve bronze medal : " << smallest << endl;
    
    return 0;
}

 



