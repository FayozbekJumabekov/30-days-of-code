# Lesson 5
description
/* Kun boshidan boshlab N sekund o’tdi. Kun
boshidan boshlab qancha soat, minut, sekund
o’tganini hisoblovchi dastur tuzing.
*/

#include <iostream>
using namespace std;


void func(int sec);


int main(){
	
	int sec;
	cin>>sec; //3670  1 soat 1 min 10 sec 
    func(sec);
	
}

 void func(int sec){
 	
 int hour,min;
 	
 		hour= sec/3600;
	
	min=sec%3600/60;
	sec= sec%3600%60;
	
	cout<<hour<<"  "<<min<<"  "<<sec;
	
 	
 	
 }


