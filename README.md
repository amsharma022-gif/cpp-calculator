#include <iostream>
#include <string>
using namespace std;

int main() {
    double num1, num2;
    string c;

    cout << "Enter the first digit: ";
    cin >> num1;

    cout << "Enter the second digit: ";
    cin >> num2;

    cout << "Enter '+' to add,\n"
         << "Enter '-' to subtract,\n"
         << "Enter '*' to multiply,\n"
         << "Enter '/' to divide,\n"
         << "Enter '**a' for square of first digit,\n"
         << "Enter '**b' for square of second digit:\n";
    cin >> c;

    if (c == "+") {
        cout << num1 + num2 << endl;
    } else if (c == "-") {
        cout << num1 - num2 << endl;
    } else if (c == "*") {
        cout << num1 * num2 << endl;
    } else if (c == "/") {
        if (num2 != 0) {
            cout << num1 / num2 << endl;  // integer division
        } else {
            cout << "Error: Division by zero!" << endl;
        }
    } else if (c == "**a") {
        cout << num1 * num1 << endl;
    } else if (c == "**b") {
        cout << num2 * num2 << endl;
    } else {
        cout << "Invalid input!" << endl;
    }

    return 0;
}
