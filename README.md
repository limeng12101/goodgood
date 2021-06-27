# goodgood
just for test


#include  <iostream>
using namespace std;


void TestRef(int &a ,int &b)
{
	int temp;
	temp = a;
	b = a;
	a = temp;
}


int main()
{
	int x = 10;
	int y = 20;
	cout << "交换前x=" << x << "交换前y=" << y << endl;
	TestRef(x , y);

	cout << "交换后x=" << x << "交换后y=" << y << endl;

	system("pause");

	return 0;

}
