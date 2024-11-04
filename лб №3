#include <iostream>
#include <cmath>  // для функції sqrt і M_PI

using namespace std;

// Завдання 1: Перетворення числа
void task_if1() {
    int num;
    cout << "Введіть ціле число: ";
    cin >> num;
    if (num > 0) num -= 8;
    cout << "Результат: " << num << endl;
}

// Завдання 2: Перевірка точки в кольоровій області
void task_geom1() {
    float x, y, r;
    cout << "Введіть радіус r: ";
    cin >> r;
    cout << "Введіть координати точки (x, y): ";
    cin >> x >> y;

    // Перевіряємо належність до області (умовно для 4 варіантів)
    if (x >= 0 && y >= 0 && sqrt(x*x + y*y) <= r)
        cout << "Точка в червоній області (33 варіант)" << endl;
    else if (x >= 0 && y <= 0 && sqrt(x*x + y*y) <= r)
        cout << "Точка в зеленій області (34 варіант)" << endl;
    else if (x <= 0 && y >= 0 && sqrt(x*x + y*y) <= r)
        cout << "Точка в жовтій області (35 варіант)" << endl;
    else if (x >= 0 && y <= 0 && sqrt(x*x + y*y) <= r)
        cout << "Точка в світло-зеленій області (36 варіант)" << endl;
    else
        cout << "Точка поза областю" << endl;
}

// Завдання 3: Площа і периметр півкола
void task_area_perimeter() {
    float r;
    cout << "Введіть радіус r: ";
    cin >> r;
    float area = (M_PI * r * r) / 2;
    float perimeter = M_PI * r + 2 * r;
    cout << "Площа півкола: " << area << endl;
    cout << "Периметр півкола: " << perimeter << endl;
}

// Завдання 4: Меню
void menu() {
    int choice;
    cout << "\n1. Перетворення числа\n2. Перевірка точки\n3. Площа і периметр\n0. Вихід\n";
    cout << "Виберіть завдання: ";
    cin >> choice;

    switch (choice) {
        case 1: task_if1(); break;
        case 2: task_geom1(); break;
        case 3: task_area_perimeter(); break;
        case 0: cout << "Вихід з програми.\n"; break;
        default: cout << "Невірний вибір!" << endl;
    }
}

int main() {
    menu();  // Запуск меню
    return 0;
}
