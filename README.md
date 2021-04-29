# PZ-3-Baza
#include <iostream>
using namespace std;

int main()
{
    cout << "Enter values" << endl;
    int mas[10];
    for (int i = 0; i < 10; i++) {
        cin >> mas[i];
        //cout << mas[i] << " ";
    }
    cout << "massive before sorting" << endl;
    for (int i = 0; i < 10; i++) {
        cout << mas[i] << " ";
    }
    cout << endl;
    for (int i = 0; i < 10; i++) {
        for (int j = 0; j < 10 - 1 - i; j++) {
            if (mas[j] > mas[j + 1]) {
                swap(mas[j], mas[j + 1]);
            }
        }
    }
    cout << "massive after sorting" << endl;
    for (int i = 0; i < 10; i++) {
        cout << mas[i] << " ";
    }
}
