#include<iostream>
#include<cmath>
using namespace std;

int main() 
{
	float sqm, total, len, wid, dia, rad, area;
	float pie = 3.14;
	float Cembag = 4;
	int boxes;
	int cement;
	bool answer;
	cout << " Is it a circle, square/rectangle :" << endl;
	cout << " For circle press 1 and for a square and rectangle press 0:";
	cin >> answer;
	if (answer == true)
	{
		cout << " Diameter:";
		cin >> dia;
		cout << " Radius:";
		cin >> rad;
		cout << " Square meter per box";
		cin >> sqm;
		area = pie * pow(rad,2);
		boxes = area / sqm;
		cement = Cembag * area;
		cout << " You will need " << boxes << " boxes to cover that circle with tiles" << endl;
		cout << " You will need " << cement << " bags of tile cement to cover that area " << endl;
	}
	else 
	{
		cout << "Lenght:";
		cin >> len;
		cout << "Width:";
		cin >> wid;
		cout << " Square meter per box:";
		cin >> sqm;
		area = len * wid;
		boxes = area / sqm;
  		cement = Cembag * area;
		cout << " You will need " << boxes << " boxes to cover that sqaure/rectangle with tiles" << endl;
		cout << " You will need " << cement << " bags of tile cement to cover that area " << endl;
	}
}
	
