# UNIQUE-ELEMENT-IN-ARRAY
#include <iostream>
using namespace std;

int main() {
    int n, arr[100];
    
    cout << "Enter the size of the array: ";
    cin >> n;
    
    cout << "Enter elements of the array: " << endl;
    for (int i = 0; i < n; i++) {
        cout << "Element " << i + 1 << ": ";
        cin >> arr[i];
    }
    
    int ans = 0;
    for (int i = 0; i < n; i++) {
        ans ^= arr[i]; // XOR operator
    }
    
    cout << "The unique element in the array is: " << ans << endl;

    return 0;
}
