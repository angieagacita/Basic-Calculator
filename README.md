#include <iostream>
using namespace std;

int main() {
    float firstNum, secondNum, answer;
    char operation;

    cout << "=== Basic Calculator ===" << endl;

    // Input first value
    cout << "Input first number: ";
    cin >> firstNum;

    // Input operator
    cout << "Choose operation (+, -, *, /): ";
    cin >> operation;

    // Input second value
    cout << "Input second number: ";
    cin >> secondNum;

    // Perform calculation
    if (operation == '+') {
        answer = firstNum + secondNum;
        cout << "Answer: " << answer;
    }
    else if (operation == '-') {
        answer = firstNum - secondNum;
        cout << "Answer: " << answer;
    }
    else if (operation == '*') {
        answer = firstNum * secondNum;
        cout << "Answer: " << answer;
    }
    else if (operation == '/') {
        if (secondNum != 0) {
            answer = firstNum / secondNum;
            cout << "Answer: " << answer;
        }
        else {
            cout << "Cannot divide by zero!";
        }
    }
    else {
        cout << "Invalid operation entered.";
    }

    return 0;
}

