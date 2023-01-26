   # Program Menghitung Luas Bangun Datar

Just copy the lines below and paste it into a new C++ Source File

It's As easy as that. :coffee: 





        #include <conio.h>
        #include <stdio.h>

        main(void) { //deklarasi variabel
	int pilih;//inisialisasi variabel inputan pemilihan switch case 
	char ulang;//inisialisasi variabel inputan pengulangan goto 
	float jari, panjang, lebar, sisi, alas, tinggi;//inisialisasi variabel inputan 
	float luasling, luasperpan, luasper, luasjar, luasseg;//inisialisasi variabel proses 
	
	//judul program 
	printf("================MENU================\n"); 
	printf("\nProgram Menghitung Luas Bangun Datar\n");
	menu://program pengulangan goto
	
	printf("------------------------------------\n");
	printf("1. Menghitung luas lingkaran \n");
	printf("2. Menghitung luas persegi panjang \n");
	printf("3. Menghitung luas persegi \n");
	printf("4. Menghitung luas genjang \n");
	printf("5. Menghitung luas segitiga \n");
	printf("------------------------------------\n");
	printf("Masukkan pilihan [0/1/2/3/4/5]:");
	
	scanf ("%i",&pilih);//pemilihan switch case
	
	switch(pilih)
		{
			case 0:
				break;
				case 1:
				printf ("\nMenghitung Luas Lingkaran \n");
				printf ("----------------------------------\n");
				printf ("Masukkan jari-jari lingkaran cm = ");
				scanf ("%f",&jari);//input
				luasling = 3.14 * jari * jari;//proses
				printf ("Luas lingkaran = %2.2f cm2\n",luasling);//output
				break;
			case 2:
				printf ("\nMenghitung Luas Persegi Panjang \n");
				printf ("----------------------------------\n");
				printf ("Masukkan nilai panjang cm = ");
				scanf ("%f",&panjang);//input
				printf ("Masukkan nilai lebar cm = ");
				scanf ("%f",&lebar);//input
				luasperpan = panjang * lebar;//proses
				printf ("Luas persegi panjang = %2.2f cm2\n",luasperpan);//output
				break;
			case 3:
				printf ("\nMenghitung Luas Persegi \n");
				printf ("----------------------------------\n");
				printf ("Masukkan nilai sisi cm = ");
				scanf ("%f",&sisi);//input
				printf ("Masukkan nilai sisi cm = ");
				scanf ("%f",&sisi);//input
				luasper = sisi * sisi;//proses
				printf ("Luas persegi panjang : %2.2f cm2\n",luasper);//output
				break;
			case 4:
				printf ("\nMenghitung Luas Jajar Genjang \n"); 
				printf ("----------------------------------\n");
				printf ("Masukkan nilai panjang cm = ");
				scanf ("%f",&panjang);//input
				printf ("Masukkan nilai tinggi cm = ");
				scanf ("%f",&tinggi);//input
				luasjar = panjang * tinggi;//proses
				printf ("Luas jajar genjang : %2.2f. cm2\n",luasjar);//output
				break;
			case 5:
				printf ("\nMenghitung Luas Segitiga \n");
				printf ("----------------------------------\n");
				printf ("Masukkan alas segitiga cm = ");
				scanf ("%f",&alas);//input
				printf("Masukkan tinggi segitiga cm = " );
				scanf ("%f",&tinggi);//input
				luasseg = alas * tinggi / 2;//proses
				printf ("Luas segitiga : %2.2f cm2 \n",luasseg);//output
				break; 
			}
				
			//input perulangan goto
				
		printf ("\n\nApakah akan menghitung lagi? [Y/T] ");
		ulang = getch();
		if (ulang == 'Y' || ulang == 'y')//pemilihan untuk melanjutkan 
			{printf ("\n\n"); goto menu; }
		if (ulang == 'T' || ulang == 't')//pemilihan untuk tudak melanjutkan
			{printf ("\nTERIMA KASIH"); }
		getch();
		}
