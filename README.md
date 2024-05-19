#include <iostream>
using namespace std;

int main() {
    // Задаем размер массива NxN
    const int N = 5; // Может быть любым числом

    // Объявляем двумерный массив
    int arr[N][N];

    // Заполняем массив значениями
    for (int i = 0; i < N; i++) {
        for (int j = 0; j < N; j++) {
            // Например, заполним массив числами от 1 до N^2
            arr[i][j] = i * N + j + 1;
        }
    }

    // Выводим массив на экран
    cout << "Двумерный массив размером " << N << "x" << N << ":" << endl;
    for (int i = 0; i < N; i++) {
        for (int j = 0; j < N; j++) {
            cout << arr[i][j] << "\t";
        }
        cout << endl;
    }

    return 0;
