# lab-7 , question 2 and 3
/*lab 7-function, ms 79,23 oct
name: nurafiqah binti khosni
class: biti s1g2
title: question 2 */

#include <iostream>
using namespace std;

void swap(int &x, int &y); //function declaration /prototype

 
int main()
{
    int x=10, y=79;
    cout<<"The original value of x: "<<x<< endl;
    cout<<"The original value of y: "<<y<< endl;
    swap(x,y);
    cout<<"The swap value of x in main: "<<x<< endl;
    cout<<"The swap value of y in main: "<<y<< endl;
    return 0;
}

void swap(int &x, int &y) //define the function

{
    int temp=x;
    x=y;
    y=temp;
    cout<<"The swap value of x in swap: "<<x<< endl;
    cout<<"The swap value of y in swap: "<<y<< endl;
}

/*lab 7-function, ms 79,23 oct
name: nurafiqah binti khosni
class: biti s1g2
title: question 3 */

#include <iostream>
using namespace std;

double total(double, double); //function declaration-prototype
const double gall=0.264179;

int main()
{
    double litre, km;
    cout<<"Please enter number of litres of petrol consumes:"<<endl;
    cin>>litre;
    cout<<"Please enter number of kilometres travelled:"<<endl;
    cin>>km;
    cout<<"The number of kilometres per gallon your car used is:" << total(litre,km)<< endl;
    return 0;
}

double total(double x, double y) //define function
{
     double ans;
     
     ans=y/(gall*x);
     return ans;
}
