# question.practice for loop  and if else 
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
# Q. 5 write a program in c++ to find the LCM of any two numbers using HCF 
#include<iostream>
using namespace std;
int i,n1,n2,j,hcf=1 ,lcm;
int main(){
cout<<"LCM of two number ";//display a message on the consol
cout<<"-------------";
cout<<"enter your first number"<<endl;//asking the user fist number 
cin>>n1;
cout<<"enter your second number"<<endl;//asking the user second number 
cin>>n2;
j= (n1<n2)?n1 :n2;//determining the smaller of the two numbers
for(i=1;i<=j;i++){//loop to find the highest common factor 
   if(n1%i==0 && n2%i ==0 ){
    hcf = i;//updating the hcf when 'i' is a common factor 
   }
}
/* multiploication of HCf and LCM = the multiplication of these two numbers .*/
lcm= (n1*n2)/hcf;// calculate the least common multiplication lcm using the formula lcm *hcf = product of the number 
cout<<"the LCM of " <<n1<<"and"<<n2<<"is"<<lcm<<endl;//displaying the calculation LCM

    return 0;
   }
# Q .6 write a program in c++ to find the sum of the series 1+1/2^2+1/3^3.........1/n^n.
#include<cmath>
#include<iostream>
using namespace std;

int main(){
double sum = 0,a;// double variable 
int n,i; // decleration of integer variable 
cout<<"find the sum of the series 1/1^1+2/2^2......n";
cout<<"_______________________________";
cout<<"enter your number"<<endl;
cin>>n;
for(i=1;i<=n;i++){
a = 1/pow(i,i);
cout<<"1/"<<i<<"^"<<i<<"="<<a<<endl;//display the current term
sum = sum+a;
}
//display the tottal sum of the series 
cout<<"the sum of the series is"<<sum<<endl;

    return 0;
# Q .7 display the pattern right angle triangle using an asterisk 
#include<iostream>
using namespace std;

int main(){
int i,j,row;
cout<<"now we find  a right angle triangle using as asterisk";
cout<<"_________________________________";
cout<<"input number of row"<<endl;
cin>>row;
for(i=1;i<=row;i++)
{
    for(j=1;j<=i;j++)
    {
        cout<<"*";
    //print an asterisk
    }
    cout<<endl;
} 
    return 0;
}
# Q.8  display the n term of odd number and their sum 
#include<iostream>
using namespace std;

int main(){
    int i,n,m=0;
    cout<<"enter your number "<<endl;
    cin>>n;
    for(i=1;i<=n;++i)
    {
     cout<<i*2-1<<endl;
     m=m+i;// add the odd number to the sum variable 

    }
     cout<<"sum of odd number "<<m<<endl;
    
    return 0;
}

# today is my test my mark 1 out of 10
# Q .9 recurssion method use in this question but some doubt ? 
#include<iostream>
using namespace std;
int fab(int n)
{
    if(n<=2){
        return 1;
    }
    return fab(n-2)+fab(n-1);
}

int main(){
    int n;
    cout<<"enter your number"<<endl;
    cin>>n;
    cout<<"the number is  "<<fab(n)<<endl;
    return 0;
}
# Q . 10  We use or , and together and we find easily a to z vowel or consonant
#include<iostream>
#include<string>
using namespace std;

int main(){
string input;
int countvowel = 0;
int countconsonant = 0;
cout<<"enter your choice "<<endl;
getline(cin , input );
for (int  i = 0; i <input.length(); i++)
{
    char c =  input[i];
    
    if((c=='a'||c=='e'||c=='o'||c=='i'||c=='u'||
c=='A'||c=='E'||c=='O'||c=='I'||c=='U')){
    countvowel++;
    
}
     
else if (c>'a'&& c <= 'z' || c <= 'Z' && c >='A' )
{
    countconsonant++;
}

        
    }
    
cout<<"kya ho sakta hai "<<countconsonant<<endl;
cout<<"kya ho sakta hai "<<countvowel<<endl;

    return 0;
}




  
 



