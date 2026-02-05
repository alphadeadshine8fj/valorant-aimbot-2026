#include <iostream>
#include <thread>
#include <chrono>
#include <random>

using namespace std;

int main() {
    random_device rd;
    mt19937 gen(rd());
    uniform_int_distribution<> dis(1, 100);

    cout << "Запускаю генератор эпичности...\n\n";

    this_thread::sleep_for(chrono::milliseconds(800));

    for (int i = 0; i < 12; ++i) {
        int power = dis(gen);
        
        cout << "Уровень крутости: ";
        
        if (power >= 95) {
            cout << "\033[1;31m" << power << " 🔥 БОГ МОДА ВКЛЮЧЁН 🔥\033[0m\n";
        }
        else if (power >= 80) {
            cout << "\033[1;33m" << power << " ✦ легенда на районе ✦\033[0m\n";
        }
        else if (power >= 60) {
            cout << "\033[1;32m" << power << " норм заходит\n";
        }
        else if (power >= 40) {
            cout << power << " среднячок\n";
        }
        else {
            cout << "\033[90m" << power << " сегодня не твой день, бро...\033[0m\n";
        }

        this_thread::sleep_for(chrono::milliseconds(400 + dis(gen) * 5));
    }

    cout << "\nФинальный вердикт: ";

    int final = dis(gen) + dis(gen) + dis(gen);
    
    if (final > 220) {
        cout << "ТЫ НЕПобедимый АЛЬФА-ТИТАН 2026 ГОДА 🗿💀\n";
    } else if (final > 180) {
        cout << "очень даже мощный чел\n";
    } else if (final > 140) {
        cout << "ну такой... жить можно\n";
    } else {
        cout << "пора качаться, братан 😭\n";
    }

    cout << "\nПовторить судьбу? (ctrl+c чтобы сбежать)\n";
    
    return 0;
}
