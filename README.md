# Lesson 5
### Task 1
```c++

#include <iostream>
using namespace std;

int main(){
	
	int sec,hour,min;
	cout<<"Sekund kiriting : ";
	cin>>sec; //3670  1 soat 1 min 10 sec 
    	hour= sec/3600;
	
	min=sec%3600/60;
	sec= sec%3600%60;
	
	cout<<hour<<":"<<min<<":"<<sec;
	
	
}

 ```
 
 # Lesson 6
 ## Task 1
 //Uchta tanga berilgan. Ulardan biri soxta va og'ir. Tortish uchun
ikki pallali tarozi o'lchov toshlarisiz berilgan. Soxta tangani
aniqlang.

 ``` c++
 #include <iostream>
using namespace std;
int main(){
	
	int a,b,c;
	
	cout<<"Birinchi tanga : "; cin>>a;
	cout<<"Ikkinchi tanga : "; cin>>b;
	cout<<"Uchinchi tanga : "; cin>>c;
	
	
	if(a>b && a>c ){
   cout<<"1 - tanga soxta"<<endl;
	}
	else if( b>a && b>c){
		
		cout<<"2- tanga soxta"<<endl;
		
	}
	else if(c>a && c>b){
		cout<<"3 - tanga soxta"<<endl;
	}
	else cout<<"???";
	
}

 ```
 ## Task 2
 //Foydalanuvchi tomonidan kiritilgan uch xonali natural sonning chapdan oqiganda ham, ongdan oqiganda ham
bir xil" ekanligini tekshiring.

 ``` c++
 
 #include <iostream>
using namespace std;
int main(){
	
	int n,a,b,c;
	cin>>n;
	
	a=n/100;
	b=n%100/10;
	c=n%10;
	
	if(a==c){
		cout<<"True"<<endl;
	}
	else cout<<"False"<<endl;
	
	
main();	
}

 ```
 
 
# Lesson 7
### Task 1
//Berilgan 3 ta sonni o'sish tartibida chiqaring

```c++
#include <iostream>
using namespace std;
int main(){
  int a,b,c;
   cin>>a>>b>>c;
   
   if(a>b && a>c){
   	if(b>c){
   		cout<<c<<" "<<b<<" "<<a<<endl;
	   }
	   else if(c>b){
	   cout<<b<<" "<<c<<" "<<a<<endl;	
	   }
   }
   if(b>a && b>c){
   	if(a>c){
   		cout<<c<<" "<<a<<" "<<b<<endl;
	   }
	   else if(c>a){
	   cout<<a<<" "<<c<<" "<<b<<endl;
	   	 } }
  
    if(c>a && c>b){
   	if(a>b){
   		cout<<b<<" "<<a<<" "<<c<<endl;
	   }
	   else if(b>a){
	   cout<<a<<" "<<b<<" "<<c<<endl;  	
   }
   }	
}
```
## Task 2
// Uchta sonning kattasini topish
``` c++
#include <iostream>
using namespace std;
int main(){
	
	int a,b,c;
	
	cout<<"Birinchi son : "; cin>>a;
	cout<<"Ikkinchi son : "; cin>>b;
	cout<<"Uchinchi son : "; cin>>c;
	
	
	if(a>b && a>c ){
   cout<<"Katta son : "<<a<<endl;
	}
	else if( b>a && b>c){
		
		cout<<"Katta son : "<<b<<endl;
		
	}
	else
		cout<<"Katta son : "<<c<<endl;
}

```
