# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar pemrograman 
<br>Nama		      : Muqtada Hasby Abdalla
<br>NIM		        :	1227050097
<br>Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Pada ujian kali ini saya membuat program yang menampilkan arrray 2 dimensi kemudian men-transpose nya. Pertama disini dimulai dari membuat index array dengan barisnya [50]dan kolom nya[50], kemudian nanti akan di input oleh pengguna untuk baris dan kolomnya 
dan akan ada inputan yang tadi telah diinput akan dilooping kemudian akan ditampilkan matriks dari yang sudah di inputkan, kemudian nilai yang telah di munculkan akan dilooping kembali untuk kemudian di transpose dengan mengganti antara kolom dan baris pada array.
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
	int k,b,c,d;
	
	cout <<"#ujian akhir semester "<<endl;
	cout <<"Mata kuliah :"<<matkul<<endl;
	cout <<"Nama :"<<nama<<endl;
	cout <<"Jurusan :"<<jurusan<<endl;
	cout <<"=========================================================="<<endl;
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
## Output
  <img width="665" alt="Screenshot 2022-12-27 210027" src="https://user-images.githubusercontent.com/118992045/209677381-873cbb91-cb19-4a37-8130-574681ba2ccd.png">
