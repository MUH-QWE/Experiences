#include <iostream>
using namespace std;
class Book
{
    public:
    double width;
    double height;
    double p()
    {
    return width *height;
    }
    double q()
    {
    return width /height;
    }
    double r()
    {
    return width +height;
    }
    double s()
    {
    return width -height;
    }
   
};

int main()
{
Book x;
cout<<"enter width:    "<<endl;
cin>>x.width;
cout<<"enter height:    "<<endl;
cin>>x.height;
char w;
cout<<"choice (+,-,*,/)"<<endl;
cin>>w;
if(w=='+'){
    cout<<x.r()<<endl;
}
else if(w=='-'){
    cout<<x.s()<<endl;
}
else if(w=='/'){
    cout<<x.q()<<endl;
}
else if(w=='*'){
    cout<<x.p()<<endl;
}

else{
    cout<<"error"<<endl;
}



    return 0;
}
