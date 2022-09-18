//# third
//create a class name weather report that tours Daily Weather report with data members for data member day of month ,high temperature, low temperature, amount of rain, amount of snow. The constructor initialise the field with default values sunday for day of month, 999 for high and low temperature , the amount of rain and snow is 0.  

#include<iostream>
using namespace std;

class weather_report
{
	int high_temp,low_temp,a_rain,a_snow;
	string day_of_month;
	public:
	void data();
	void display();
	
	weather_report() //constructor
	{
		day_of_month="sunday"; //default
		high_temp=999;
		low_temp=999;
		a_rain=0;//amount of rain
		a_snow=0;
			
	}
};

void weather_report::data()
{
	cout<<"Enter the day of month :";
	cin>>day_of_month;
	cout<<"Enter the high temp : ";
	cin>>high_temp;
	//cout<<"Enter the low temp : ";
	//cin>>low_temp;
	cout<<"Enter the amount of rain : ";
	cin>>a_rain;
	cout<<"Enter the amount of snow : ";
	cin>>a_snow;
	cout<<endl;
}
void weather_report::display()
{
	cout<<"The day of month : "<<day_of_month<<endl;
	cout<<"The high temp is :"<<high_temp<<endl;
	cout<<"The low temp is :"<<low_temp<<endl;
	cout<<"The amount of rain : "<<a_rain<<endl;
	cout<<"The amount of snow : "<<a_snow<<endl;
}
int main()
{
	 weather_report obj;
	 obj.data();
	 obj.display();
	 return 0;
}
