#include<iostream>
using namespace std;

int wc(int a, int b)
{
    int vg;

    while(b!=0)
    {
        vg = b;
        b = a%b;
        a = vg;
    }

    return a;
}

int main()
{
    int a, b;

    cout<<"Podaj po spacji dwie liczby: ";
    cin>>a>>b;

    cout<<"NWD("<<a<<","<<b<<") = "<<wc(a,b)<<endl;



    return 0;
}
