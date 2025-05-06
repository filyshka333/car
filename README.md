#include <iostream> 
using namespace std; 
class Car 
{ 
private: 
  string color; 
  string type; 
  int year; 
 public: 
  void setColor(string color){ 
  this->color = color; 
 } 
  void setType(string type){ 
  this->type = type; 
 } 
  void setYear(int year){ 
  this->year = year; 
 } 
 string getColor(){ 
  return this->color; 
 } 
 string getType(){ 
  return this->type; 
 } 
 int getYear(){ 
  return this->year;  
 } 
  
 void startCar(){ 
  cout << "Аввтомобиль заведен" << endl; 
 } 
 void stopCar(){ 
  cout << "Автомобиль заглушен"<< endl; 
 }  
 void msgColor(){ 
  cout << "Цвет автомобиля "<< getColor() << endl; 
 } 
     
}; 
 int main() 
{ 
setlocale (LC_ALL, "Russian"); 
 Car car; 
  
 car.setColor("Green"); 
 car.setType("Bus"); 
 car.setYear(1960); 
  
 car.startCar(); 
 car.stopCar(); 
 car.msgColor(); 
 cout << "Тип автомобиля: " << car.getType()<<endl; 
 cout << "Год выпуска: " << car.getYear()<<endl; 
 return 0; 
}
