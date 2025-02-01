#include <iostream> 
#define M_PI 3.14159265358979323846 
 
using namespace std; 
 
int main() { 
 
    double alpha_degrees, alpha_radians; 
    cout << "3."; 
    cout << "\nz1 = Cos a + cos 2a + cos 6a + cos 7a"; 
 
    cout << "\nz2 = 4 Cosa/2 * cos5/2 a * cos4a "; 
 
    cout << "\n\nEnter alpha in degrees: "; 
    cin >> alpha_degrees; 
 
    alpha_radians = alpha_degrees * M_PI / 180.0; 
 
    double z1 = cos(alpha_radians) + cos(2 * alpha_radians) + cos(6 * alpha_radians) 
+ cos(7 * alpha_radians); 
 
    double z2 = 4 * cos(alpha_radians / 2) * cos(5 * alpha_radians / 2) * cos(4 * 
alpha_radians); 
 
    cout << "z1 = " << z1 << endl; 
    cout << "z2 = " << z2 << endl; 
 
    if (fabs(z1 - z2) < 1e-9) { 
        cout << "z1 and z2 are approximately equal." << endl; 
    } 
    else { 
        cout << "z1 and z2 are not equal." << endl; 
    } 
 
    return 0; 
}
