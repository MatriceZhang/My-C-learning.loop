My-C-learning
==================

//learning
#include <iostream>
#include <iomanip>   //for setw
using namespace std;

int main(){
    const unsigned long limit=4294967295u;
    unsigned long next=0;
    unsigned long last=1;
    while (next<limit/2)  //don't let the result get too big
    {
        cout<<last<<" ";
        long sum=next+last;
        next=last;
        last=sum;
        
    }
    cout<<endl;
    return 0;
    
    
}

