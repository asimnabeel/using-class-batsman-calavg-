# using-class-batsman-calavg-
using class batsman calavg using class batsman find its bat avg in #C++
#include<iostream>
#include<string>
using namespace std;
class Batsman
{
string batsman_name;
int Batcode,Total_innings,n_out_innings, runs, bestscore;
float bat_avg;
public:
float calavg()
{
bat_avg = runs / Total_innings;
return runs / Total_innings;
}
void read_data()
{
cout << "Enter batsman name:" << endl;
cin.ignore();
getline(cin, batsman_name);
cout << "Enter Batcode:" << endl;
cin >> Batcode;
cout << "Enter Total innings:" << endl;
cin >> Total_innings;
cout << "Enter Not out innings:" << endl;
cin >> n_out_innings;
cout << "Enter runs:" << endl;
cin >> runs;
cout << "Enter bestscore:" << endl;
cin >> bestscore;
calavg();
}
void display()
{
cout << "Batsman name:" << batsman_name << endl;
cout << "Bat code:" <<Batcode << endl;
cout << "Total innings:" << Total_innings << endl;
cout << "Not out innings:" << n_out_innings << endl;
cout << "Runs:" << runs << endl;
cout << "Best score:" << bestscore << endl;
cout << "bat avg:" << bat_avg << endl;
calavg();
}
};
int main()
{
Batsman b1;
b1.read_data();
b1.display();
}
