#include <iostream>
using namespace std;

int main() {
    char operation;
    double num1, num2, result;

    cout << "Введіть операцію (+, -, *, /): ";
    cin >> operation;

    cout << "Введіть два числа: ";
    cin >> num1 >> num2;

    switch (operation) {
        case '+':
            result = num1 + num2;
            cout << "Результат: " << result << endl;
            break;
        case '-':
            result = num1 - num2;
            cout << "Результат: " << result << endl;
            break;
        case '*':
            result = num1 * num2;
            cout << "Результат: " << result << endl;
            break;
        case '/':
            if (num2 != 0) {
                result = num1 / num2;
                cout << "Результат: " << result << endl;
            } else {
                cout << "Помилка: ділення на нуль!" << endl;
            }
            break;
        default:
            cout << "Невідома операція!" << endl;
    }

    return 0;
}
