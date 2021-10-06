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
 ### Task 2
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
 
 
# Lesson 8
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
### Task 2
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
# Lesson 9
### Task 1
//Calculator
``` c++
#include <iostream>
using namespace std;
int main(){
   
   float a,b;
   char k;
   int n;
  while(true){
  	 cout<<"Enter the  number : ";
  	 cin>>a>>k>>b;
   switch(k){
   	
   	case '+' : cout<<"Javob :"<<a+b<<endl; break;
   	case '-' : cout<<"Javob :"<<a-b<<endl; break;
   	case '*' : cout<<"Javob :"<<a*b<<endl; break;
   	case '/' : cout<<"Javob :"<<a/b<<endl; break;
   	default : cout<<"Bunday amal yo'q"<<endl; break;	
   }
  }	}
```

# Lesson 10
### Task 1
// Valyuta o'zgartirish
``` c++
#include <iostream>
using namespace std;
int main(){
   
   string currency,curren; 
   float value;

  	 cout<<"Enter Currency : "; cin>>currency;
  	 cout<<"Enter the Value : "; cin>>value;
     cout<<"Qaysi valyutaga otmoqchisiz ?  "; cin>>curren;
    if(currency=="euro") // start
    {
           if(curren=="cad"){
		   cout<<value*554.92/875.85<<endl;
   	cout<<value*554.92<< " usd"<<endl;
}
else if(curren=="aud"){
		   cout<<value*554.92/1105.95<<endl;
   	cout<<value*554.92<< " usd"<<endl;
} else if(curren=="inr"){
		   cout<<value*554.92/34754.84<<endl;
   	cout<<value*554.92<< " usd"<<endl;         
}}
	else if(currency=="usd") // start
  cout<<value*1<<" usd"<<endl;
  
	else if(currency=="funt"){ //start
 if(curren=="cad"){
		   cout<<value*554.92/875.85<<endl;
   	cout<<value*554.92<< " usd"<<endl;
}
else if(curren=="aud"){
		   cout<<value*554.92/1105.95<<endl;
   	cout<<value*554.92<< " usd"<<endl;
} else if(curren=="inr"){
		   cout<<value*554.92/34754.84<<endl;
   	cout<<value*554.92<< " usd"<<endl;
}	
}
else if(currency=="cad") //start
  {   	if(curren=="euro"){
		   cout<<value*875.85/554.92<<endl;
   	cout<<value*554.92<< " usd"<<endl;     
}
else if(curren=="aud"){
		   cout<<value*875.85/1105.95<<endl;
   	cout<<value*554.92<< " usd"<<endl;
          
} else if(curren=="inr"){
		   cout<<value*875.85/34754.84<<endl;
   	cout<<value*554.92<< " usd"<<endl;
}
  } 
	else if(currency=="inr"){ //start
	if(curren=="cad"){
		   cout<<value*554.92/875.85<<endl;
   	cout<<value*554.92<< " usd"<<endl;
          
}
else if(curren=="aud"){
		   cout<<value*554.92/1105.95<<endl;
   	cout<<value*554.92<< " usd"<<endl;
          
} else if(curren=="euro"){
		   cout<<value*34754.84/554.92<<endl;
   	cout<<value*554.92<< " usd"<<endl;
}
   }}
   
```
### Task 2
// Kiritilgan sonning, kiritilgan oraliqdagi darajalari yigindisi
``` c++

#include <iostream>
using namespace std;

int main(){
	
int n,sum=0,i;
int k; 
cout<<"Oraliq kiriting : "; cin>>n;
cout<<"Nechining darajasi kerak : "; cin>>i;
k=i;

 while(n>=i){
	
	sum=sum+i;
	i=i*k;
}
cout<<sum;
}

```
### Task 3
// Tub son topish

``` c++
#include <iostream>
using namespace std;

int main(){
	int n,sum=0;
	cin>>n;
	
	for(int i=2; i<n; i++){
		
		if(n%i==0)
	    sum+=1;	 	   
}   
     if(sum==0)
    cout<<"Tub son ";
    else cout<<"Tub son emas";
}
```
### Task

/// Kiritilgan son 2 ning darajasi yoki yo'q tekshirish

``` c++
#include <iostream>
using namespace std;

int main(){
	
int n,sum=0,i=2;
int k; 
cout<<"Oraliq kiriting : "; cin>>n;
k=i;

 while(n>i){
	i=i*k;
}

if(n==i)
cout<<"True"<<endl;
else cout<<"False"<<endl;

main();
}
```
# Lesson 11
### Task 1
//Berilgan satrda nechta katta harf, nechta kichik harf borligini aniqlovchi dastur tuzing

``` c++
#include <iostream>
#include <ctype.h>

using namespace std;

int main(){
	int sumUpper=0, sumLower=0;
	string satr;
	cin>>satr;
	
	for(int i=0; i<=satr.length(); i++){
		
		if(isupper(satr[i]))
		sumUpper++;
		
		else if(islower(satr[i]))sumLower++;
		
	}	
	
	cout<<"Katta harf :"<<sumUpper<<endl;
	cout<<"Kichik harf :"<<sumLower;
	
} 
```

### Task 2
/// Password

``` c++
#include <iostream>
#include <ctype.h>

using namespace std;

int main(){
	int sumUp=0,sumLow=0, sumDig=0;
	string satr;
	cin>>satr;
	
	for(int i=0; i<=satr.length(); i++){
		
		if(isupper(satr[i]))
		 
		 sumUp++; 

		if(islower(satr[i]))
		 
		 sumLow++; 

        if(isdigit(satr[i]))
		 
		 sumDig++; 
		  }	
		  
		if(sumUp !=0 && sumLow!=0 && sumDig!=0 && satr.length() >= 8)
		
		  	cout<<"Yaroqli parol "<<endl;
		  	
		  	else cout<<"Yaroqsiz parol"<<endl;
}
```
### Task 3

// Ekub topish

``` c++
#include <iostream>

using namespace std;

    int ekub(int a, int b){
    	
    	 while(a!=b){
    	 	
    	 	if(a>b)
    	 	a=a-b;
    	 	else if
			 (a<b)
    	 	b=b-a;
    	 		
		 }
		 return a;
        	
	}
   
int main(){
	
	
	int a,b;
	cin>>a>>b;
	
	cout<<"Ekub : "<<ekub(a,b);
	
}

```

# Lesson 16
// Linear qidiruv

### Task 1
``` c++
#include <iostream>
#include <time.h>
#include <stdlib.h>

using namespace std;

   void func (float arr[], int size,int k){
   	      int m;
		  for(int i=0; i<size; i++){
		  	
		  	cout<<arr[i]<<" ";
		  	
		if(arr[i]==k)
		  	m=i;
		  }
		  cout<<endl<<"Indeksi: "<<m;
   }

int main(){
	
       int size,k; cout<< "n= "; cin>>size;
       
       float arr[size];
        
        for(int i=0; i<size; i++){
             
			 cin>>arr[i];	
        	
		}
       
       cout<<"Son kiriting :"; cin>>k;
       
       func(arr,size,k);
}
```

# Lesson 17
### Task 1 
// ikki olchovli arrayda olchovi toq kirtilganda, ikki chekkasi hamda orta liniyadagi elementlar summasi
``` c++
#include <iostream>

using namespace std;


int main(){
	
     int n,m,sum=0;
     cout<<"Olcham kiriting : "; cin>>n>>m;
     
     int arr[n][m];
     
     for(int i=0; i<n; i++){
     	
     	for(int j=0; j<m; j++){
     		cout<<i+1<<"."<<j+1<<" element : ";
     		cin>>arr[i][j];
     		
		 }	
	 }
     cout<<endl;
     for(int i=0; i<n; i++){
     	for(int j=0; j<m; j++){
     		
     		cout<<arr[i][j]<<"  ";
     		
     		
     		if(j==0 || j==m-1 || i==(n-1)/2)
     		sum=sum+arr[i][j];
			 
			 	 
			 	 }
		 cout<<endl;
	 }
	        
     	cout<<endl<<"Sum : "<<sum;
}
```
### Task 2
// S1 va S2 satrlari berilgan. S1 satrida birinchi uchragan S2 satrini o’chirib tashlovchi dastur tuzing. Agar S1 satrida S2 satri uchramasa S1 o’zgarishsiz qolsin

``` c++
#include <iostream>

using namespace std;

int main(){
	
    	string str1,str2,text="";
    	getline(cin,str1);
    	getline(cin,str2);
    	
    	for(int i=0; i<str1.length(); i++){
    		
    		if(str1[i] == str2[0]){
    			text.assign(str1,i,str2.length());
    			if(text==str2){
    				
    			str1.erase(i,str2.length());
					break;
				}
			}
		}
		cout<<str1;
}
```
### Task 3
// S1, S2 va S3 satrlari berilgan. S1 satrida birinchi uchragan S2 satrini S3 satriga o’zgartiruvchi dastur tuzing.

```c++
#include <iostream>

using namespace std;

int main(){
	
    	string str1,str2,str3,text="";
    	getline(cin,str1);
    	getline(cin,str2);
    	getline(cin,str3);
    	
    	for(int i=0; i<str1.length(); i++){
    		
    		if(str1[i] == str2[0]){
    			text.assign(str1,i,str2.length());
    			if(text==str2){
    				
    				str1.replace(i,str2.length(),str3);
    				
				}
			}
		}
		cout<<str1;
}
```
### Task 4

//  S satr berilgan. Agar satrning uzunligi toq bo'lsa, eng
o'rtadagi bitta belgisidan, agar juft bo'lsa, eng
o'rtadagi 2 ta belgisidan iborat satrni ajratib oling.
Masalan:
1) s="hovli" => javob: result="v"
2) s="antiqa" => javob: result ="ti"

``` c++
#include <iostream>

using namespace std;

int main(){
      string str;
      cout<<"Satrni kiriting : ";
      cin>>str;
      
      for(int i=0; i<str.length(); i++){
      	
      	if(str.length()%2!=0){
      		
      		if(i==str.length()/2){
      			cout<<str[i]<<endl;	
			  }
		  }
		  else {
		  	if(i==str.length()/2-1)

		  	cout<<str[i]<<str[i+1];
		  }
	  }
}
```
