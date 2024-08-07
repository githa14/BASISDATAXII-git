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
# Membuat Table
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
-  `Telp varchar (255) NOT NULL` : Kolom ini menyimpan nomor telepon pegawai. Data di sini adalah unik karena memiliki kunci unik (`UNI`), yang memastikan tidak ada dua pegawai dengan nomor telepon yang sama.
-  `Jabatan enum ('Manajer','Staf','Sales')` : Kolom ini menyimpan jabatan pegawai. Nilai yang ada seperti 'Manajer', 'Sales', dan 'Staf'. Adapun satu baris yang memiliki nilai kosong, yang menunjukkan bahwa jabatan untuk pegawai tersebut belum ditentukan.
-  `Gaji BIGINT (255) NOT NULL` : Kolom ini menyimpan gaji pegawai dengan kapasitas yang besar, sesuai dengan nilai-nilai yang ada misalnya, 5250000, 2500000, dll.
-  `NoCab varchar (255) NOT NULL` : Kolom ini menyimpan nomor cabang tempat para pegawai bekerja. Nilai seperti 'C101', 'C103', dan 'C104' menunjukkan bahwa pegawai tersebut dikelompokkan berdasarkan cabang, dan adapun beberapa pegawai yang memiliki cabang yang sama.

# Menampilkan Table
Code :
```mysql
	DESC pegawai;
```

![[asset/4.JPG]]

Analisa :
- `DESC pegawai;` : digunakan untuk menampilkan deskripsi atau informasi rinci tentang struktur tabel database yang berisi data pegawai.
# Memasukkan Data
Code :
```mysql
	DESC pegawai;
```

![[asset/4.JPG]]

Analisa :
- `DESC pegawai;` : digunakan untuk menampilkan deskripsi atau informasi rinci tentang struktur tabel database yang berisi data pegawai.
# Menampilkan Hasil Penginputan Data
Code :
```mysql
	SELECT * FROM Pegawai;
```

![[asset/6.JPG]]

Analisa :
- `SELECT * FROM Pegawai;` : digunakan untuk mengambil semua data dari tabel `pegawai`. Artinya, query ini akan menampilkan semua kolom dan baris yang ada di dalam tabel `pegawai`.
