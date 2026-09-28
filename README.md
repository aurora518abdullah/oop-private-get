# oop-private-get

#include<bits/stdc++.h>
using namespace std;
class Car{
private:
    string brand,model;
    double price;
public:
    Car(string brand,string model,double price)
    {
        this->brand=brand;
        this->model=model;
        this->price=price;
    }
    string getter() const
    {
        return brand;
    }
    string getter1() const
    {
        return model;
    }
    double getter2() const
    {
        return price;
    }
    void display()
    {
        cout<<"Brand: "<<brand<<" | model: "<<model<<" | price: "<<price<<endl;
    }


};


int main()
{
    Car a1("Toyota","Corolla",25000);
    Car a2("Honda","Civil",28000);
    a1.display();
    a2.display();
}
