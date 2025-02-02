#include <iostream>

int main() {
    double a, b;  
    char c;
    std::cout << "Մուտքագրեք առաջին թիվը: ";
    std::cin >> a;
    std::cout << "Մուտքագրեք երկրորդ թիվը: ";
    std::cin >> b;
    std::cout << "Մուտքագրեք գործողության նշանը (+, -, *, /): ";
    std::cin >> c;
    if (c == '-') {
        std::cout << "a = " << a - b << "\n";
    } else if (c == '+') {
        std::cout << "b = " << a + b << "\n";
    } else if (c == '*') {
        std::cout << "b = " << a * b << "\n";
    } else if (c == '/') {
        if (b != 0) {
            std::cout << "b = " << a / b << "\n";
        } else {
            std::cout << "Սխալ: Զրոյի վրա բաժանում չի թույլատրվում!\n";
        }
    } else {
        std::cout << "Սխալ նշան: Ներմուծեք +, -, * կամ / \n";
    }
    switch (c) {
        case '-':
            std::cout << "a = " << a - b << "\n";
            break;
        case '+':
            std::cout << "a = " << a + b << "\n";
            break;
        case '*':
            std::cout << "a = " << a * b << "\n";
            break;
        case '/':
            if (b != 0) {
                std::cout << "a = " << a / b << "\n";
            } else {
                std::cout << "Սխալ: Զրոյի վրա բաժանում չի թույլատրվում!\n";
            }
            break;
        default:
            std::cout << "Սխալ նշան: Ներմուծեք +, -, * կամ / \n";
    }

    return 0;
}
