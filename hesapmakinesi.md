#include <iostream>
using namespace std;

int main() {
    int sayi1, sayi2, islem, sonuc = 0;

    cout << "1. sayiyi giriniz: ";
    cin >> sayi1;

    cout << "2. sayiyi giriniz: ";
    cin >> sayi2;

    cout << "Toplama = 1, Cikarma = 2, Carpma = 3, Bolme = 4";
    cout << "Islem seciniz: ";
    cin >> islem;

    if (islem == 1) {
        sonuc = sayi1 + sayi2;
        cout << "Sonuc: " << sonuc;
    }
    else if (islem == 2) {
        sonuc = sayi1 - sayi2;
        cout << "Sonuc: " << sonuc;
    }
    else if (islem == 3) {
        sonuc = sayi1 * sayi2;
        cout << "Sonuc: " << sonuc;
    }
    else if (islem == 4) {
      if(sayi2 != 0)
       {sonuc = sayi1 / sayi2;}
       
        cout << "Sonuc: " << sonuc;
    }
 
    return 0;
}
