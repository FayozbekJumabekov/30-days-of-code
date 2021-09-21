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
	   	
	   }
   }
   
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
