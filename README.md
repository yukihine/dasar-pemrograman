# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar pemrograman 
<br>Nama	 	: Muqtada Hasby Abdalla
<br>NIM		        :	1227050097
<br>Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
program kali ini adalah 1. membuat array 2 dimensi kemudian di transpose  dan 2. membuat matriks 2 dimensi (nilai di inputkan), dan menampilkan nilai yang
habis dibagi 3,5 dan 7.

NO 1. membuat array 2 dimensi kemudian di transpose. pada program ini index array di buat yaitu [50] untuk baris dan [50] untuk kolom. kemudian banyaknya baris dan kolom akan di inputkan setelah diinputkan akan di masukkan pada mengulangan dan diinputkan nilai dari masing masing baris dan kolom. setelah di masukkan nilai akan di tampilkan dalam bentuk matriks dan dimasukkan ke pengulangan untuk ditranpose. kemudian akan di tampilkan nilai dari tranpose-nya.

NO 2. membuat matriks 2 dimensi (nilai di inputkan),dan menampilkan nilai yang habis dibagi 3,5 dan 7. pada program ini index array di buat yaitu [50] untuk baris dan [50] untuk kolom. kemudian banyaknya baris dan kolom akan di inputkan setelah diinputkan akan di masukkan pada mengulangan dan diinputkan nilai dari masing masing baris dan kolom. kemudian nilai tersebut akan masuk pada kondisi IF ELSE yaitu jika nilai dapat dibagi 3,5,dan 7 maka jika kondisi tersebut true maka nilai akan di tampilkan dan jika false maka akan memasuki kondisi nilai tidak dapat dibagi 3,5, dan 7. setelah itu nilai akan ditampilkan. 
## Source Code
#include <iostream>
using namespace std;

int main(){
	string nama="Muqtada Masby Abdalla";
	int nim='1227050097';
	string matkul="Dasar pemrograman";
	string jurusan="[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/)";
	int matriks [50][50],transpose[50][50];
	int baris, kolom;
	int a,k,b,c,d;
	
	cout <<"ujian akhir semester "<<endl;
	cout <<"Mata kuliah :"<<matkul<<endl;
	cout <<"Nama :"<<nama<<endl;
	cout <<"Jurusan :"<<jurusan<<endl;
	cout <<"=========================================================="<<endl;
	cout <<"1. Buatlah array 2 dimensi kemudian di transpose"<<endl;
	cout <<"2. Buatlah matriks 2 dimensi (nilai di inputkan), kemudian nilainya habis 3,5 dan 7"<<endl;
	cout <<"apa yang ingin anda cari?";
	cin >>a;
	
	if (a==1){
	    cout <<"Buatlah array 2 dimensi kemudian di transpose"<<endl;
            cout << "Masukkan jumlah baris : ";
	    cin >> baris;
	    cout << "Masukkan jumlah kolom : ";
	    cin >> kolom;
	    
	    //pengulangan matriks
	    //input matriks
	    for (b=1;b<=baris;b++){
	    	for (k=1;k<=kolom;k++){
	    		cout <<"baris ke-"<<b<<" kolom ke-"<<k<<":";
	    		cin >>matriks[b][k];
			}
		}
		cout <<endl;
		
		//tampilan matriks
		cout<<endl<<"tampilan matriks "<<endl<<endl;
	    for (b=1;b<=baris;b++){ 
	        for (k=1;k<=kolom;k++){ 
	                cout<<matriks[b][k]<<"  ";
	            }
	        cout<<endl;
	    }
	    
		//transpose 
		for (b=1;b<=baris;b++){
			for(k=1;k<=kolom;k++){
				transpose [b][k]=matriks[b][k];
			}
		}
		
		//tampilan setelah di transpose 
		cout <<"hasil transpose ="<<endl;
		 for (b=1;b<=baris;b++){
		 	for(k=1;k<=kolom;k++){
		 		cout <<transpose [k][b]<<"  ";
			 }
			cout <<endl;
		 }
	}
		
	else if (a==2){
	    cout << "Masukkan jumlah baris : ";
	    cin >> baris;
	    cout << "Masukkan jumlah kolom : ";
	    cin >> kolom;
	    
	    //pengulangan matriks
	    //input matriks
	    for (b=1;b<=baris;b++){
	    	for (k=1;k<=kolom;k++){
	    		cout <<"baris ke-"<<b<<" kolom ke-"<<k<<":";
	    		cin >>matriks[b][k];
			}
		}
		cout <<endl;
		
		//tampilan matriks
		cout<<endl<<"tampilan matriks "<<endl<<endl;
	    for (b=1;b<=baris;b++){ 
	        for (k=1;k<=kolom;k++){ 
	                cout<<matriks[b][k]<<"  ";
	            }
	        cout<<endl;
	    }
	    	
		cout <<"bilangan yang dapat dibagi 3,5 dan 7"<<endl;
		cout <<"===================================="<<endl;
		for (b=1;b<=baris;b++){
			for (k=1;k<=kolom;k++){
				if (matriks [b][k] %3 ==0 && matriks[b][k] %5==0 && matriks [b][k] %7 ==0){
					cout <<matriks [b][k]<<"  " <<" dapat dibagi 3,5,7"<<endl;
				}
				else {
					cout <<matriks [b][k]<<" tidak habis dibagi 3,5,7"<<endl;
				}
			}
		}
	}
	return 0;
}	
## Output
NO 1.	
<img width="626" alt="Screenshot 2022-12-31 195227" src="https://user-images.githubusercontent.com/118992045/210137393-ae6ac0a9-be02-4dba-94d3-e3fe83d2588a.png">

NO 2.
<img width="624" alt="Screenshot 2022-12-31 195314" src="https://user-images.githubusercontent.com/118992045/210137412-b587e237-e34a-4f78-b12a-6fd5f3a29c42.png">
	
