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
                              # loop question
#  badhiya question Q .1 write a program in c++ to find a prime number within a range .

#include<iostream>
#include<math.h>
using namespace std;
int m ,n;
int a=0 ,b=0;
int main(){
    cout<<"find prime number within a range";
    cout<<"----------------------------";
    cout<<"input number for starting range";
    cin>>m; // reading the starting range entered by the range 
    cout<<"input number for ending range ";
    cin>>n;// reading the ending range entered by the range 
    cout<<"the prime numbers between"<<m<<"and"<<n<<"are"<<endl;//display a message 
    // indicating the range of numbers
for(int i = m; i<=n; i++ )
{
    for(int j = 2 ; j<=sqrt(i);j++)
    {

if (i%j==0)// checking if the number is divisible by j 
b++;// incrementing b if i is divisible by j 
    }
    if (b== 0 && i!=1)// checking if b is zeroo and i not equal to 1 
    //prime number should not be 1
   {
      a++ ; // incrementing a as prime number is found
    cout<<i<<" "; // display the prime number 
   }  
   b = 0; // resetting b to zero for the next iteration
}
cout<<"the total number of prime numbers between "<<m<<"to"<<n<<"is "
<<a<<endl;//display the total cout of prime numbers found 
    
    return 0;
}
# Q.2  Write a program in c++ to find the sum of the digits of a given number.
//c++ exercise find the sum of digit of a given number
#include<iostream>
using namespace std;
int num1,num2,r,sum=0;//decleration of integer variable 
int main(){
// display a message to find the sum of digits of a given number
cout<<"find the sum of digits of a given number";
cout<<"___________________________";

// the user to input a number
cout<<"input a number"<<endl;
cin>>num1;//reading the number enter by the user 
num2 = num1; // store the original number in num2 for display letter
// loop to extract each digit and calculate their sum 
while (num1>0)

{
    r =  num1%10;//extract the rightmost digit of num1;
    num1 = num1/10;//remove the rightmost digit of num1;
    sum = sum +r;//add the extracted digit to the sum variable

}
// display the sum of digit of the original number 'num2'
cout<<"the sum of the digit "<<num2<<"is"<<sum<<endl;
return 0;   
}

# Q.3 write a program in c++ to find the factorial of a number
#include<iostream>
using namespace std;
int n ,factorial= 1;
int main(){
cout<<"find the factorial of a number ";//display a message indicate a purpose
cout<<"________________________";
cout<<"input a number to find the factorial ";//promoting the user to input a number 
cin>>n;//reading the number enter by the user
for(int i = 1;i<=n;i++)//loop calculate the factorial 
{
    factorial = factorial*i;
}
cout<<"the factorial of a number "<<factorial<<endl;
    return 0;

  # Q. 4  write a program in c++ to display cube of the number up to an integer
#include<iostream>
using namespace std;

int main(){
int n,b,cube;
cout<<"enter your number ";
cin>>b;
for(int i=1;i<=b;i++)
{
 cube = i*i*i;
    cout<<"number is :"<<i<<"and the cube "<<cube<<endl;//display the number and its cube 

}

    return 0;
}









  
 



