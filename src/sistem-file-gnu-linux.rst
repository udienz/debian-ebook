=====================
Sistem File GNU/Linux
=====================

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

Pemilik, Hak Akses, dan Group
-----------------------------

GNU/Linux merupakan salah satu sistem operasi yang cukup aman (secure).
Seorang user dapat memproteksi file-filenya dan dapat menentukan user mana
saja yang dapat mengakses, membaca, dan merubah file tersebut. Saat sebuah
file dibuat dan disimpan oleh user, maka secara otomatis kepemilikannya
(owner) adalah user yang bersangkutan. Terdapat tiga macam hak akses dari
sebuah file, yaitu:

**Read:** mengizinkan user lain untuk membaca isi dari file tersebut tetapi user lain
tidak dapat melakukan perubahan isi file.

**Write:** mengizinkan kepada user lain untuk dapat membaca dan melakukan
perubahan terhadap isi file, termasuk menghapusnya.

**Execute:** mengizinkan user lain dapat mengeksekusi/menjalankan file (biasanya
berupa script atau program).

Pemberian hak akses kepada user dapat dilakukan secara individu (one by one)
oleh pemilik file. Pemberian hak akses kepada user lain seperti di atas masih
dapat dilakukan jika jumlah user masih terjangkau. Namun bagaimana halnya
jika jumlah user telah mencapai ratusan atau bahkan ribuan dalam sebuah
perusahaan. Sungguh bukan sebuah ide yang baik jika harus diberikan hak akses
satu per satu kepada user yang jumlahnya ribuan tadi. Masalah tersebut ternyata
telah terpikirkan oleh developer GNU/Linux dengan menciptakan manajemen
group yang di dalamnya dapat mencakup banyak user.

Selain hak akses yang dimiliki oleh sebuah file, sistem file GNU/linux juga
mengenal tiga buah mode akses terhadap direktori atau file. Adapun ketiga
mode akses tersebut, yaitu:

**Owner** 	: hak akses user pemilik direktori atau file.

**Group** 	: hak akses group tempat user tersebut berada.

**Other** 	: hak akses setiap user selain pemilik direktori atau file

Berikut rincian penjelasan mode akses dan hak akses terhadap sebuah file atau
direktori GNU/Linux.

.. image:: images/hak-akses.png
	:alt: Pemilik, Hak akses dan group

Hak akses terhadap file juga dapat dikonversikan ke dalam bilangan biner dan
desimal seperti yang tampak pada tabel berikut.

======	=========
Nilai	Arti
======	=========
0	\- \- \-
1	\- \- x
2	\- w \-
3	\- w x
4	r \- \-
5	r \- x
6	r w \-
7	r w x
======	=========

Berikut aturan konversi hak akses *owner, group, dan other* dari huruf ke
bilangan biner dan desimal. Konversi ini nantinya akan berguna saat manajemen
user pada bab selanjutnya.

.. image:: images/konversi-hak-akses.png

Berikut contoh kasus penerapan kepemilikan, hak akses, dan group pada sistem
file GNU/Linux.

Terdapat sebuah file dokumen keuangan pada perusahaan tertentu, sebutlah
perusahaan A. Dokumen ini dimiliki oleh salah satu karyawan divisi keuangan.
Secara otomatis file tersebut tentu saja hak kepemilikannya dimiliki oleh
karyawan yang bersangkutan. Ia berencana untuk memberikan hak akses
seluruh karyawan divisi keuangan tetapi tidak untuk karyawan divisi lain. Hak
akses yang diberikan ke divisi yang bersangkutan hanyalah akses untuk melihat
isi file dokumen saja tetapi tidak berhak untuk merubah isi dari file yang
bersangkutan. Sedangkan untuk hak execute tidak diperlukan karena filenya
bukanlah program atau script.

Bagaimana karyawan tersebut melakukan semua ini? Tentu saja bukanlah hal
yang sulit karena sistem operasi GNU/Linux menyediakan fasilitas perubahan
hak akses yang telah dijelaskan pada awal bab ini. Lebih jauh tentang perubahan
hak akses terhadap sebuah file akan dijelaskan pada bab manajemen user dan
hak akses.


Memahami direktori GNU/Linux
----------------------------

Direktori debian GNU/Linux tersusun secara hirarki. Berbeda dengan microsoft
windows yang mengelompokkan berdasarkan partisi yang ada. Debian
GNU/Linux hanya memiliki satu hirarki direktori besar yang berisi semua
partisi yang ada. Direktori teratas adalah direktori root yang ditandai dengan
forward slash (/).

Di bawah direktori root (/) berisi sub direktori */bin, /boot, /dev, /etc, /home, /lib,
/lost+found, /misc, /mnt, /proc, /root, /sbin, /tmp, /usr, /var*. Di bawah
subdirektori yang telah disebutkan di atas, masih terdapat subdirektori lagi
hingga berupa file saja.

.. image:: images/hirarki-direktori.png
	:alt: Hirakri direktori Debian GNU/Linux

Meskipun bukan sesuatu yang begitu penting untuk mengetahui isi seluruh
direktori debian GNU/Linux, tapi merupakan hal yang sangat baik jika anda
mengetahui jenis-jenis dari file yang tersimpan pada setiap direktori yang ada.

Direktori Debian GNU/Linux
~~~~~~~~~~~~~~~~~~~~~~~~~~

Struktur debian GNU/Linux dan varian GNU/Linux lain berdasarkan pada
sistem operasi UNIX. Keuntungan dari sistem direktori ini adalah anda dapat
memposisikan sebuah partisi sebagai sebuah file pada sistem. Berikut ini
struktur direktori/file debian GNU/Linux:
























