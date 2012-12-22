Memahami File GNU/Linux
-----------------------

Pada sebuah komputer, seluruh informasi yang tersimpan di dalam media
penyimpanan seperti hardisk, disket, flash drive, dll adalah sebuah file. Pada
GNU/Linux, seluruh program, dokumen, konfigurasi sistem-seluruhnya
tersimpan di dalam file-file, sehingga di dalam hardisk anda dapat tersimpan
ratusan atau bahkan ribuan file. Semuanya terorganisasi dalam sebuah sistem
file (filesystem) GNU/Linux. Sistem file GNU/Linux berbeda dengan sistem file
yang digunakan oleh sistem operasi lain seperti MS Windows atau Macintosh.

Seluruh perangkat hard drive anda dipandang sebagai sebuah file. GNU/Linux
menggunakan 3 tipe utama dari objek sebagai media penyimpanan informasi,
yaitu:

**Files:** File-file yang menjalankan program disebut dengan file executable atau
file biner. File biner biasanya diletakkan pada direktori /bin (singkatan dari
binary), atau di direktori /sbin (singkatan dari system binaries).

**Links:** Penunjuk ke file lain.

**Directories:** Kumpulan file, links dan direktori lain.


Memahami Nama File yang Digunakan GNU/Linux
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Penamaan file, links, dan direktori GNU/Linux mengikuti aturan berikut:

#. Tidak boleh lebih dari 256 karakter, dan nama path/direktori tidak boleh lebih
   dari 4096.
#. Case sensitive, GNU/Linux membedakan karakter huruf besar dan kecil.
   Misalkan: \`askari` akan berbeda dengan \`ASKARI`.
#. Dapat menggunakan huruf maupun angka. Namun, untuk menghindari
   kesalahan penulisan sebaiknya tidak menggunakan karakter \`#` karena kalimat
   setelah karakter tersebut akan dianggap sebagai komentar.
#. Menggunakan slash forward (/) untuk identifikasi sebuah direktori.

Memahami Ekstensi File GNU/Linux
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

GNU/Linux dapat membaca ekstensi file dari sistem operasi lain seperti \*.jpg
untuk file gambar, \*.html untuk file web, \*.doc untuk word processor Microsoft
Windows, dll. Ekstensi File yang digunakan debian GNU/Linux:


**.bz2**
	File kompresi dengan menggunakan kompresi bzip2.

**.gz**
	File kompresi dengan menggunakan kompresi gzip.

**.c**
	File yang ditulis dalam bahasa C.

**.conf**
	File konfigurasi GNU/Linux.

**.deb**
	Paket instalasi debian GNU/Linux.

**.lock**
	File yang terkunci demi untuk menghindari pemakaian oleh file lain.

**.so**
	Objek share (pustaka atau modul).

**.src**
	File source code. Yang ditulis dalam plain text, file tersebut harus 
	dikompilasi terlebih dahulu sebelum menggunakannya.

**.tar**
	File yang berisi bundelan/kumpulan file lain yang dijadikan satu.

**.tar.gz**
	File bundelan yang terkompresi dalam format .gz.
	

Pada GNU/Linux, terdapat beberapa tipe file seperti executable file, system data
file, dan user data file. Beberapa perbedaan yang ada antara lain:

**Executable file:** file-file ini berisi instruksi program untuk dijalankan oleh
sistem. Program dan script merupakan executable file.

**system data file:** file-file ini berisi informasi yang digunakan oleh program atau
script. Biasanya digunakan oleh administrator dan para programmer untuk
menjalankan program secara berlainan.

**user data file:** file-file ini berisi teks dan data yang dibuat oleh user.
Secara default GNU/Linux dapat mengenali secara otomatis seluruh tipe file
sehingga anda tidak perlu lagi bersusah payah dengan tipe filenya.

Hidden File
~~~~~~~~~~~

Beberapa file yang ada pada GNU/Linux terkadang tidak tampak atau tidak
dapat diakses oleh user lain. Sebagai contoh, terdapat banyak file konfigurasi
sistem yang hanya dapat diakses oleh root dan biasanya oleh sistem dibuat
tersembunyi (hidden), sehingga tidak dapat dilihat/diakses oleh user lain.

Namun, sebagai user biasa pun anda dapat membuat file tersembunyi. File
tersembunyi pada GNU/Linux biasanya diawali dengan karakter titik (.). Anda
dapat melihat beberapa file tersembunyi yang ada pada direktori home.

::

	kari@debian:~$ ls -al
	
	total 2348
	drwxr-xr-x 79 kari kari   12288 Des 20 23:52 .
	drwxr-xr-x  3 root root    4096 Sep 18 08:06 ..
	drwx------  4 kari kari    4096 Okt 14 01:02 .adobe
	-rw-rw-r--  1 kari kari     239 Sep 21 09:59 .apport-ignore.xml
	drwx------  2 kari kari    4096 Des 19 00:50 .aptitude
	drwxr-xr-x  3 kari kari    4096 Okt 27 18:30 .ardour2
	drwxrwxr-x  4 kari kari    4096 Des  4 11:58 .audacity-data

Untuk membuat sebuah hidden file dapat menggunakan perintah berikut::

	kari@debian:~$ cat > .datarahasiaku

Catatan:

Pembuatan *hidden file* selalu diawali dengan karakter titik (.)
