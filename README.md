# Calculator Script

Just copy the lines below and paste it into a new C++ Source File
as easy as that. :coffee:





    #include <iostream>
     using namespace std;

    int main() {
    int a, b, hasil, menu;
    float c, d, hasilbagi;

    cout << "====================================" << endl;
    cout << "Program Kalkulator Sederhana" << endl;
    cout << "====================================" << endl << endl;

    cout << "\tMenu:" << endl;
    cout << "\t1. Penjumlahan" << endl;
    cout << "\t2. Pengurangan" << endl;
    cout << "\t3. Perkalian" << endl;
    cout << "\t4. Pembagian" << endl;
    cout << "Pilih menu: ";
    cin >> menu;
    cout << "-------------------------------" << endl;

    switch (menu) {
        case 1:
            cout << "\n1. Penjumlahan:" << endl;
            cout << "Masukan bilangan pertama: ";
            cin >> a;
            cout << "Masukan bilangan kedua: ";
            cin >> b;
            hasil = a + b;
            cout << "-------------------------------+" << endl;
            cout << "Hasil:\t\t\t" << hasil << endl;
            break;
        case 2:
            cout << "\n2. Pengurangan:" << endl;
            cout << "Masukan bilangan pertama: ";
            cin >> a;
            cout << "Masukan bilangan kedua: ";
            cin >> b;
            hasil = a - b;
            cout << "--------------------------------" << endl;
            cout << "Hasil:\t\t\t" << hasil << endl;
            break;
        case 3:
            cout << "\n3. Perkalian:" << endl;
            cout << "Masukan bilangan pertama: ";
            cin >> a;
            cout << "Masukan bilangan kedua: ";
            cin >> b;
            hasil = a * b;
            cout << "-------------------------------x" << endl;
            cout << "Hasil:\t\t\t" << hasil << endl;
            break;
        case 4:
            cout << "\n4. Pembagian:" << endl;
            cout << "Masukan bilangan pertama: ";
            cin >> c;
            cout << "Masukan bilangan kedua: ";
            cin >> d;
            hasilbagi = c / d;
            cout << "-------------------------------:" << endl;
            cout << "Hasil:\t\t\t"  << hasilbagi << endl;
            break;
        default:
            cout << "Kamu salah memilih menu." << endl;
            break;
    }

    return 0;
    }
