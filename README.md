#include <iostream>
using namespace std;
int main()
{
    int bil[5], n, i, j, temp;
    cout<<"Masukkan Bilangan yang ingin diurutkan "<<endl;
    cin>>n;
    
    
    for (n=1; n<=4; n++){
        cin >> bil[n];
    }
    cout<<endl;
    cout << "Hasil pengurutan bilangan secara ascending : " <<endl;
    for (i=1; i<=4; i++){
        for (j=1; j<=4; j++){
            if (bil[i] < bil[j]){
                temp = bil[i];
                bil[i] = bil[j];
                bil[j] = temp;
            }
        }
    }
    for (i=1; i<=4; i++){
        cout << bil[i] << ", ";
    }
    return 0;
}
