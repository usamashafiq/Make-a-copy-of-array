#include<iostream>
#include<conio.h>
using namespace std;

void cpy(float[], float[], int, int=0);
void main() {
	int b; float a[99], c[99];
	cout << "Enter a size of array : ";
	cin >> b;
	cout << "Enter a first array : ";
	for (int i = 0; i < b; i++) {
		cin >> a[i];
	}cout << endl;
	cout << "Enter a second array : ";
	for (int j = 0; j < b; j++) {
		cin >> c[j];
	}
	char q;
	cout << "If you want a copy portion of array  (Y/N)   ";
	cin >> q;
	if (q == 'y' || q == 'Y') {
		int w;
		cout << "Enter a number where you start copy : ";
		cin >> w;
		cout << "Enter a number end of copy : ";
		cin >> b;
		cpy(a, c,b, w);
	}
	else {
		cpy(a, c,b);
	}
	_getch();
}
