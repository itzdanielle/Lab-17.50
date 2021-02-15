# Lab-17.50
#include <iostream>
using namespace std;

double kilometers (int num) {
  double result;
  result = 1.61 * num;
  return result;
  
}
double milesToKilo (int num) {
  double result;
  result = .621 * num;
  return result;
  
}

int main() {
  cout << "Please input" << endl;
  cout << "1 Convert miles to kilometers" << endl;
  cout << "2 Convert kilometers to miles" << endl;
  int num;
  cin >> num;
  if (num == 1) 
  {
    int miles;
    cout << "Please input the miles to be converted" << endl; 
    cin >> miles;
    int kilo = kilometers (miles);
    cout << miles << " Miles = " << kilo << " Kilometers" << endl;

  }
  if (num == 2) 
  {
    int kilometers;
    cout << "Please input the kilometers to be converted" << endl;
    cin >> kilometers;
    int miles = milesToKilo (kilometers); 
  cout << kilometers << " Kilometers = " << miles << " Miles" << endl;
  }
}
