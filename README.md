#include <iostream>
#include <cstdlib>   
#include <ctime>     

using namespace std;
int main() {
    srand(time(0));  
    int rastgeleSayi = rand() % 100 + 1; 
    int tahmin;
    int denemeSayisi = 0;

    cout << "_SAYI_TAHMIN_OYUNU_" << endl;
    cout << "1 ile 100 arasinda bir sayi tuttum. Tahmin et bakalim!" << endl;

    while (true) {
        cout << "Tahminini gir: ";
        cin >> tahmin;
        denemeSayisi++;

        if (tahmin < rastgeleSayi) {
            cout << "Daha buyuk bir sayi gir." << endl;
        } 
        else if (tahmin > rastgeleSayi) {
            cout << "Daha kucuk bir sayi gir." << endl;
        } 
        else {
            cout << " Tebrikler " << denemeSayisi << "denemede bildin. " << endl;
            break;
        }
    }
}

        




















