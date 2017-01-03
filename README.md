#include <iostream>
using namespace std;
float celsius,fahrenheit,kelvin,rankine;
void convert_Celsius()
{
    fahrenheit = (celsius * 9 / 5) + 32;
    kelvin=celsius+273.15;
    rankine=(celsius+273.15)*9/5;
}
void convert_Fahrenheit()
{
    celsius = (fahrenheit - 32) * 5 / 9;
    kelvin = (fahrenheit +459.67) *5/9;
    rankine = fahrenheit +459.67;
}
void  convert_Kelvin()
{
    celsius=kelvin-273.15;
    fahrenheit=kelvin*9/5 - 459.67;
    rankine=kelvin*9/5;
}
void convert_Rankine()
{
    celsius=(rankine-491.67)* 5/9;
    kelvin=rankine *5/9;
    fahrenheit=rankine-459.67;
}


int main()
{
    unsigned short n,x;
    cout<<"Alege 1 pentru a converta temperatura."<<"\n"<<"Alege 2 pentru a converta lungimea."<<"\n"<<"Alege 3 pentru a converta aria."<<"\n"<<"Alege 4 pentru a converta volum."<<"\n"<<"Alege 5 pentru a converta viteza."<<"\n"<<"Alege 6 pentru a converta greutate."<<"\n"<<"Alege 7 pentru a converta presiune."<<endl;
    cin>>x;
    if(x==1)
    {
        cout<<"Alege 1 pentru a converta grade Celsius." <<"\n"<<"Alege 2 pentru a converta grade Fahrenheit." <<"\n"<<"Alege 3 pentru a converta grade Kelvin."<<"\n"<<"Alege 4 pentru a converta grade Rankine."<<endl;
        cin >>n;
        if(n==1)
        {
            cout << "Alege temperatura in Celsius: ";
            cin >> celsius;
            convert_Celsius();
            cout << "Temperatura in Fahrenheit este: " << fahrenheit<<"\n"<< "Temperatura in Kelvin este: "<< kelvin<<"\n"<< "Temperatura in Rankine este: " << rankine<<endl;
        }
     }
     return 0;
     }
