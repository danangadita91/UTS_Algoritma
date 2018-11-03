# UTS_Algoritma

```
Soal 1 : Soal 1-Program Perulangan-while
Alur Algoritma :
1. Mendeklarasikan int a, b, x, y;
	dimana a, b sebagai variable input
	dan x, y sebagai penampung nilai input dari variable a, b
2. Menggunakan Pembanding pertama sebagai pencari nilai yang sama
	(x!=y)= Penjelasan jika nilai x=y => False (End)
3. Menggunakan pembanding ke dua sebagai perulangan
	(x<y) {
	x= x+a
	y= y+b }
	Penjelasan: menggunakan perbandingan (x<y) dengan ketentuan perulangan
	x= x+a, y= y+b
4. Pertanyaan A.  jika a=2 dan b=4 maka hasilnya adalah :
	True, maka = 4 Kali Perulangan

5. Pertanyaan B. jika a=4 dan b=7 maka hasilnya adalah :
	True, maka = 28 Kali Perulangan

6. Rumus ini akan berulang sampai x=y
```
Berikut kodenya :
```c++
int main()
{
    int x,y,a,b,progres;
    cout<< " Masukan Nilai A :";
    cin>> a;
    cout<< " Masukan Nilai B :";
    cin>> b;
    progres= true;
    x=a;
    y=b;

    while (progres){
        if (x!=y){
            if (x<y)
            {
                x=x+a;
            }
            else
            {
                y=y+b;
            }
        }
        else
            progres=false;
    }
    cout<< x<< " Kali Perulangan";
}
```
Berikut Hasilnya :
![img](https://raw.githubusercontent.com/danangadita91/UTS_Algoritma/master/Soal1/kondisi%20a%3D2%20b%3D4.png)
![img](https://raw.githubusercontent.com/danangadita91/UTS_Algoritma/master/Soal1/kondisi%20a%3D4%20b%3D7.png)


```
Soal 2 - Perulangan dengan Input nim sebagai batas
Alur Algoritma : 
1. Mendeklarasikan int n, x, t, batas;
	int n = variable input
	x = variable input (konstanta)
	t = penampung nilai variable input n
	batas = untuk menentukan batas/perbandingan
2. Masukan nilai input n = “sesuai 2 digit trakhir NIM”(55)
3. Menentukan batas
	(t=<=batas)
	t= t+ x;
	x= x+ 10;
4. Hasilnya adalah : 195
```
Berikut Kodenya :
```c++
int main()
{
    int n, x, t, batas;
    cout<<"Masukan nilai n : ";
    cin>>n;
    batas= n+ 100;
    x= 20;
    t= n;
    while (t<=batas)
    {
        t= t+ x;
        x= x+ 10;
    }
    cout<<t;
    return 0;
}
```
Berikut hasilnya :
![img](https://raw.githubusercontent.com/danangadita91/UTS_Algoritma/master/Soal2/Perulangan%20dengan%20NIM.png)
