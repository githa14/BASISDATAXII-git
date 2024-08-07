# Membuat Database
1. Pertama,  buatlah database pada cmd.
	 Code :
	 ```mysql
	 CREATE DATABASE company_githa;
	 ```

	![[asset/1.JPG]]

	Analisa :
	- `CREATE DATABASE company_githa;` : digunakan membuat database baru bernama "company_githa"

2. Kedua, gunakanlah database tersebut untuk membuat tabel didalam database tersebut.
	 Code :
	 ```mysql
	 USE company_githa;
	 ```

	![[asset/2.JPG]]

	Analisa :
	- `USE company_githa;` : digunakan untuk membuat kita berpindah ke dalam database "company_githa" untuk melakukan operasi-operasi selanjutnya.
# Membuat table
 Code :
```mysql
	 CREATE TABLE pegawai ( 
	 NIP int (255) PRIMARY KEY, 
	 NDep varchar (255) NOT NULL, 
	 NBlk varchar (255), 
	 JK enum ('Laki-laki','Perempuan') NOT NULL, 
	 Alamat text (255) NOT NULL, 
	 Telp varchar (255) NOT NULL, 
	 Jabatan enum ('Manajer','Staf','Sales'), 
	 Gaji BIGINT (255) NOT NULL, 
	 NoCab varchar (255) NOT NULL 
	 );
```

![[asset/3.JPG]]

Analisa :
- `CREATE TABLE pegawai ( ` : digunakan untuk membuat sebuah tabel baru bernama "pegawai".
- `NIP int (255) PRIMARY KEY` : Ini adalah nomor unik yang digunakan untuk mengidentifikasi setiap pegawai. Setiap pegawai memiliki NIP yang berbeda. 
-  `NDep varchar (255) NOT NULL` : Kolom ini menyimpan nama depan pegawai. Nama-nama seperti 'Emya', 'Diah', 'Dian', dll.
-  `NBlk varchar (255)` :  Kolom ini menyimpan nama belakang pegawai. Nama-nama seperti 'Salsalina', 'Wahyuni', 'Anggraini', dll.
-  `JK enum ('Laki-laki','Perempuan') NOT NULL` : Kolom ini menyimpan jenis kelamin pegawai yaitu "Laki-laki" atau "Perempuan".
-  `Alamat text (255) NOT NULL` : Kolom ini menyimpan alamat lengkap pegawai. Data alamat seperti 'Jl.Suci 78 Bandung', dll., menunjukkan format teks yang panjang, sesuai dengan kebutuhan penyimpanan informasi alamat.
-  `Telp varchar (255) NOT NULL` : digunakan untuk membuat sebuah tabel baru bernama "pegawai".
-  `Jabatan enum ('Manajer','Staf','Sales')` : digunakan untuk membuat sebuah tabel baru bernama "pegawai".
-  `Gaji BIGINT (255) NOT NULL` : digunakan untuk membuat sebuah tabel baru bernama "pegawai".
-  `NoCab varchar (255) NOT NULL` : digunakan untuk membuat sebuah tabel baru bernama "pegawai".

# Menampilkan table
# Memasukkan data dan Menampilkan Hasilnya