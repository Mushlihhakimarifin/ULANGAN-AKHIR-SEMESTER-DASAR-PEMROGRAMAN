# Ujian Akhir Semester 
<br>Mata Kuliah 	: DASAR PEMROGRAMAN 
<br> Nama		: MUSHLIH HAKIM ARIFIN
<br>NIM		:	1227050098
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

dalam uas kali ini kita diberi tugas seperti dibawah tugas yang pertama kita diharuskan membuat kolom dan baris serta sebaliknya dalam uas kali ini dengan menggunakan c++ matriks 2 dimensi,lalu kita diberi tugas untuk menginputkan nilai pada kolom dan baris tersebut yang nanti akan muncul pada outputnya tugas yang kedua kita menginputkan nilai berapa saja lalu dibagi habis dengan bilangan prima(3,5,7),setelah nilainya di inputkan maka nanti akan muncul angka yang diinputkan dan bisa dibagi habis dengan bilangan prima tersebut.

## Source Code

Tugas [1]

#include <iostream>
#include <iomanip>

using namespace std;

int main()
{
	cout<<"=========================================="<<endl;
  cout << "     Program Input Matriks 2 Dimensi " << endl;
  cout << "==========================================" << endl;
  cout << endl;

  int matriks[100][100];
  int trans[100][100];
  int jum_baris, jum_kolom, i, j;

  cout << "Input jumlah baris matriks: ";
  cin >> jum_baris;

  cout << "Input jumlah kolom matriks: ";
  cin >> jum_kolom;
  cout << endl;

  for(i = 0; i < jum_baris ; i++){
    for(j = 0; j < jum_kolom; j++){
      cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
      cin >> matriks[i][j];
    }
    cout << endl;
  }

  cout << "Hasil matriks: " << endl;

  for(i = 0; i < jum_baris ; i++){
    for(j = 0; j < jum_kolom; j++){
      cout << setw(3) << matriks[i][j] << " ";
    }
    cout << endl;
  }

  for(i = 0; i < jum_baris ; i++){
    for(j = 0; j < jum_kolom; j++){
      trans[j][i]=matriks[i][j];
    }
    cout << endl;
  }
  cout<<"Hasil transpose:"<<endl;
  for(i = 0; i < jum_kolom ; i++){
    for(j = 0; j < jum_baris; j++){
      cout<<trans[i][j]<<"\t";
    }
    cout<<endl;
}

  return 0;
}

Tugas [2]

#include <iostream>
#include <iomanip>

using namespace std;

int main()
{
	cout<<"=========================================="<<endl;
  cout << "         MUSHLIH HAKIM ARIFIN " << endl;
  cout << "==========================================" << endl;
  cout << endl;

  int matr[100][100];
  int y, x, i, j;

  cout << "Input jumlah baris matriks: ";
  cin >> y;

  cout << "Input jumlah kolom matriks: ";
  cin >> x;
  cout << endl;

  for(i = 0; i < y ; i++){
    for(j = 0; j < x; j++){
      cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
      cin >> matr[i][j];
    }
    cout << endl;
  }

cout<<"Nilai Dibagi 3"<<endl;

for (i=0; i<y;i++)
{
	for (j=0;j<x;j++)
	{
		if(matr[i][j]%3==0){
				cout<<" "<<matr[i][j];
		}
		
	}

 } 
 cout<<endl;
 cout<<"Nilai Dibagi 5"<<endl;

for (i=0; i<y;i++)
{
	for (j=0;j<x;j++)
	{
		if(matr[i][j]%5==0){
				cout<<" "<<matr[i][j];
		}
		
	}

 } 
 cout<<endl;
 cout<<"Nilai Dibagi 7"<<endl;

for (i=0; i<y;i++)
{
	for (j=0;j<x;j++)
	{
		if(matr[i][j]%7==0){
				cout<<" "<<matr[i][j];
		}
		
	}

 } 
 cout<<endl;
  return 0;
}
## Output
