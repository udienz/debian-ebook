===========
Pendahuluan
===========

Sistem Operasi
--------------

Tugas utama dari sebuah sistem operasi adalah menyediakan interface
(antarmuka) antara aplikasi user dan hardware (perangkat keras) komputer.
Aplikasi user adalah program yang ditulis untuk membantu pengguna dalam
menyelesaikan pekerjaannya seperti program akuntansi, pemrosesan data,
perangkat lunak database, manajemen sistem informasi, dll.

Sebuah sistem operasi bertanggung jawab untuk mengatur sumber daya
perangkat keras, mencegah terjadinya konflik antara program aplikasi yang ada,
dan untuk sistem operasi multiuser bertanggung jawab mencegah terjadinya
konflik diantara komputasi yang dibutuhkan oleh setiap user yang sedang login
ke komputer. Hardisk, port I/O, memori, CPU – seluruh sumber daya perangkat
keras komputer ini membutuhkan pengaturan tentang bagaimana cara
pengaksesan atau pengalamatannya.

Program-program aplikasi berjalan di level tertinggi dari sistem operasi,
sehingga program ini tidak perlu mengetahui seluk beluk perangkat keras
komputer. Selain itu, beberapa sistem operasi didesain untuk keperluan spesifik
seperti aplikasi embedded OS sehingga kustomasi software benar-benar
merupakan faktor terpenting.

GNU Software
------------

Proyek pengembangan GNU berdiri pada tahun 1984 oleh Richard Matthew
Stallman yang kesehariannya bekerja sebagai karyawan MIT. Tujuan dari
proyek GNU ini adalah untuk mengembangkan software-software dengan penuh
kebebasan (free software). Free software ini berarti kebebasan bagi setiap orang
untuk melihat source code, kebebasan untuk mempelajari, serta kebebasan
dalam mengembangkannya. Pada tahun 1989 Richard Stallman
mendeklarasikan sebuah lisensi terhadap proyek GNU yang beliau kembangkan
dalam kurung waktu 5 tahun. Richard M. Stallman mendeklarasikan GNU
Public License (GPL). Hak lisensi ini lebih tertuju kepada lisensi copyleft yang
tentu saja sangat berbeda dengan hak lisensi copyright.

Pada tahun 1991 ketika Linus B. Torvalds menciptakan kernel linux yang
dikombinasikan dengan software GNU. Kombinasi antara kernel Linux dan
software GNU ini yang kemudian menjadi cikal bakal dari free operation system
GNU/Linux.

Banyak user atau pengguna OS tersebut menginstal tool-tool GNU pada mesin-
mesin yang berbeda tipe tanpa ada masalah. Tool GNU ini menyediakan
konsistensi terhadap platform PC yang berbeda-beda.

Tool-tool GNU dikembangkan oleh GNU Project meliputi utility yang cukup
esensial seperti manajemen file GNU (The GNU File Management) dan utility
text processing GNU. Manajemen file GNU meliputi perintah-perintah dasar
yang banyak digunakan jika bermain pada lingkungan mode teks (ls, mv, mkdir,
head, sort, wc, cat, less, mtools, tar, textutils, gzip, time,wget, emacs, gcc,
gphoto, binutils, bash, awk, gtk +, aspell, gdb, gnumeric, dll).
Daftar paket software yang dikembangkan oleh GNU Project dapat dilihat di
website `GNU Project`_.

Linux kernel
------------

Awalnya Unix merupakan sistem operasi yang sangat populer karena
kemurniannya, dan ketersediaan source code program. Namun akhirnya dengan
berbagai macam alasan, hak lisensi UNIX mulai melarang penggunaan source
code untuk diajarkan di lingkungan universitas.

Linux sendiri adalah sebuah kernel yang dikembangkan oleh Linus B. Torvalds
karena terinspirasi oleh kernel MINIX buatan Andy Tanenbaum. Salah satu hal
penting yang patut untuk dicatat pada Linux adalah pengembangan arsitektur
komponen dasar yang menitipberatkan pada fasilitas sharing resource untuk
aplikasi-aplikasi yang berjalan di atas GNU/Linux. Misalnya Desktop Manager
GNOME, menggunakan Bonobo (Built on top of the international CORBA
standard) untuk sharing resource arsitektur komponen-komponen softwarenya.

Apa itu GNU/Linux
-----------------

Sebagaimana yang telah dijelaskan sebelumnya, GNU dan Linux adalah suatu
kesatuan software yang saling terintegrasi membentuk sebuah sistem operasi
yang cukup handal dan stabil. GNU/Linux merupakan sistem operasi
multitasking, dan sekaligus multiuser. Disebut multitasking karena GNU/Linux
dapat mengatur sharing CPU dari tugas-tugas yang sedang dieksekusi. Setiap
tugas (task) mendapatkan sumber daya perangkat keras yang sama. GNU/Linux
harus dapat memroses setiap tugas (task) dalam waktu yang sangat singkat.
Beberapa tugas memiliki prioritas tertinggi sehingga diperlukan juga prioritas
pemakaian sumber daya CPU ke tugas tersebut.

Salah satu keunggulan dari sistem operasi multitasking adalah kemampuan dari
sistem operasi tersebut untuk dapat menjalankan tugas-tugas yang berbeda
secara simultan.
Bagaiamana sebuah komputer dapat dikatakan multiuser?, Cukup sederhana
saja, yakni pengguna dapat menggunakan komputer yang sama pada waktu yang
bersamaan dan tetap terjadi proses pemisahan informasi antara pengguna yang
ada. Sistem operasi multiuser harus mampu mengakomodasikan koneksi lebih
dari satu user ke sistem secara simultan.

Tokoh penting GNU/Linux
------------------------

Richard Matthew Stallman
========================

Richard Matthew Stallman (RMS) lahir di Manhattan pada tanggal 16 Maret
1953 dari pasangan Alice Lippman dan Daniel Stallman. Richard Stallman
adalah tokoh sentral Free Software Foundation, pendiri Proyek GNU serta
pencetus hak lisensi copyleft dan konsep ini diabadikannya dengan lisensi
General Public License (GPL).

Proyek GNU yang diciptakan oleh Richard Stallman antara lain: teks editor
Emacs, debugger GDB, kompiler GNU (GCC) yang saat ini telah mendukung
30 macam arsitektur komputer dan 7 macam bahasa pemrograman. Software-
software buatannya merupakan bagian terpenting pada proyek GNU secara
keseluruhan.

Tahun 1960-an merupakan era Personal Computer (PC). Kesempatan pertama
yang didapatkan Stallman untuk mendalami komputer saat ia duduk di bangku
sekolah menengah pertama (junior high school). Stallman menghabiskan masa
liburannya setelah menyelesaikan sekolah menengah pertama untuk menulis
program pertamanya.

Bahasa pemrograman yang digunakan pada waktu itu adalah PL/I pada
komputer IBM 7094. Tahun 1974 Stallman meraih gelar BA pada bidang fisika
di Harvard University. Selama menjalani masa perkuliahannya di Harvard
University, Stallman juga bekerja sebagai staff hacker di laboratorium AI MIT.
Tahun 1984 Stallman mengundurkan diri dari MIT untuk mencurahkan
perhatian sepenuhnya terhadap proyek GNU sehingga akhirnya tidak dapat
menyelesaikan program doktoral yang diikutinya. Namun demikian, Stallman
telah mendapat 3 gelar Doctor Honoris Causa (HC) dari beberapa universitas di
dunia.

Selain itu, Stallman juga sempat menjabat sebagai Asisten Laboratorium
Biologi di Universitas Rockefeller. Berkat kemampuan analisis yang sangat
tinggi sehingga membuat kagum pimpinan Laboratorium tersebut. Hal lain yang
membuat pimpinan lab terkagum-kagum pada diri seorang Stallman karena latar
belakang pendidikannya selama ini bukan dalam bidang biologi melainkan
matematika dan fisika. Kemampuan lain yang dimiliki seorang Stallman adalah
dalam bidang komputer.

Beberapa penghargaan yang diperoleh Richard Matthew Stallman:
 - MacArthur Fellowship - tahun 1990
 - The Association for Computing Machinery’s Grace Hopper Award atas
   software emacs buatannya - tahun 1991
 - Doctor Honoris causa (HC) dari Sweden’s Royal Institute of Technology -
   tahun 1996
 - Electronic Frontier Foundation’s Pioneer Award - tahun 1998
 - Yuri Rubinski Memorial Award - tahun 1999
 - Doctor Honoris causa (HC) dari Universitas Glasgow - tahun 2001
 - The Takeda Techno-Entreprenourship Award - tahun 2001
 - National Academy of Engineering membership - tahun 2002
 - Doctor Honoris causa (HC) dari Vrije Universiteit Brussel - tahun 2003

Linus B. Torvalds
=================

Linus Torvalds lahir pada tanggal 28 Desember 1969 di Helsinki-Finland.
Ayahnya bernama Torvalds. Saat berusia 10 tahun Linus Torvalds sudah mulai
mencoba membuat program pada komputer Commodore VIC-20 milik sang
kakek.

Tahun 1991 Torvalds tercatat sebagai mahasiswa ilmu komputer di University
of Helsinki, Finland. Di tahun yang sama Torvalds membeli sebuah komputer
(PC) dengan MS-DOS sebagai sistem operasinya. Namun Linus Torvalds
sendiri lebih menyukai menggunakan operation system (OS) UNIX yang
digunakan di departemen ilmu komputer tempat ia menuntut ilmu.

Linus Torvalds kemudian membuat base OS (Linux - red) varian UNIX untuk
digunakan pada komputer miliknya. Setelah linux (Linus’s MINIX) rampung,
Linus Torvalds kemudian mengirim email ke internet untuk memberikan
informasi bahwa telah tersedia sebuah sistem operasi gratis beserta source
codenya.

Berkat kestabilan Linux yang jarang mengalami crash membuat para vendor
perusahaan ternama mengumumkan rencananya untuk mendukung linux sebagai
sistem operasi alternative MS-Windows.

Beberapa penghargaan yang diperoleh Linus Torvalds:
 - Nokia Foundation Award - tahun 1997
 - Lifetime Achievement Award at Uniforum Pictures - tahun 1997

Pengertian Free Software dan Open Source Software
-------------------------------------------------

Mungkin bagi kalangan linuxer tidak asing lagi dengan istilah free software dan
open source software. Pada bagian ini penulis hanya akan menjelaskan sedikit
tentang perbedaan antara free software dan open source software. Pengertian
open source adalah sebuah software dimana kode sumbernya terbuka untuk
publik sehingga semua orang dapat melihat, memodifikasi ulang. Sedangkan
free software tidak dapat diartikan sebagai freeware (gratis dalam penggunaan
produk software). Free software diartikan sebagai sebuah kebebasan dalam
menyalin, mendistribusikan, dan memodifikasi kode sumber tanpa adanya
batasan dari siapa pun juga.

.. Note::
	``Free`` disini bukan berarti hanya gratis, namun juga diartikan bebas
	
Aspek lain dari sebuah aplikasi open source adalah pengembangan dari
perangkat lunak tersebut lebih cepat dan lebih murah dalam segi pendanaannya
karena lebih banyak orang yang terlibat. Aplikasi open source memberikan
beban kerja yang tidak terlampau berat kepada para programmer disebabkan
adanya sharing tugas kepada setiap orang dalam jumlah yang banyak. Aplikasi-
aplikasi software yang mereka hasilkan juga tidak dapat dipandang sebelah mata
sebab kebanyakan hasil karya mereka benar-benar berkualitas tinggi akibat
dukungan orang-orang dengan level kemampuan yang berbeda-beda yang
bersatu dalam satu tim pengembang.

Selain itu, bug-bug aplikasi software open source biasanya lebih cepat diketahui
dibanding aplikasi close source dan penanganannya pun akan lebih cepat pula.

Free Documentation
------------------

Pada bulan maret 2000, Richard M. Stallman bersama Eben Moglen – seorang
professor dari Columbia Law School mengumumkan hak kepemilikan
dokumentasi yang berlisensi “GNU Free Documentation License (GFDL)”.
Sebuah dokumen GFDL haruslah bersifat transparan – dalam arti kata bahwa
dokumen tersebut harus tersedia dalam format yang dapat dibaca dengan
menggunakan free software seperti latex atau yang mendukung format XML.

Distribusi GNU/Linux
--------------------

Bingung? pertanyaan ini sering muncul bagi para pemula yang ingin
menggunakan sistem operasi (OS) GNU/Linux. Begitulah sedikit gambaran
tentang anggapan orang-orang karena banyak distribusi/distro Linux. Mengapa
sampai banyak varian Linux yang ada saat ini?, hal ini disebabkan karena
sifatnya yang free software-open source alias kebebasan dan kode programnya
terbuka untuk publik sehingga memungkinkan orang untuk membuat distribusi
masing-masing.

Debian GNU/Linux
----------------


Distro GNU/Linux ini berdiri pada tanggal 16 agustus 1993 yang diciptakan
oleh Ian Murdock. Nama Debian ini diambil dari penyatuan dua nama yakni
Debra dan Ian Murdock. Debra adalah istri Ian Murdock – sang pembuat distro
Debian GNU/linux.

Sistem Debian sekarang ini menggunakan kernel `Linux <http://www.kernel.org/>`_
dan kernel `FreeBSD <http://www.freebsd.org/>`_. Linux adalah bagian dari 
perangkat lunak yang dimulai oleh `Linus Torvalds <http://www.cs.helsinki.fi/u/torvalds/>`_
dan didukung oleh ribuan programmer di seluruh dunia. Sedangkan FreeBSD 
adalah sistem operasi yang termasuk kernel dan perangkat lunak lainya.

Namun Debian sedang dalam proses untuk menyediakan ke kernel lain, terutama 
untuk `Hurd <http://www.gnu.org/software/hurd/hurd.html>`_ . Hurd adalah kumpulan
server yang berjalan diatas sebuah microkernel (seperti March) yang diimplementasikan
di fitur yang berbeda. Hurd dalah perangkat lunak yang dihasilkan oleh proyek 
`GNU project`_.

Distro ini sering disebut-sebut sebagai pure GNU/Linux karena satu-satunya
distro yang sampai saat ini masih menuruti asas free software. Debian sendiri
memiliki sistem pemaketan sendiri (\*.deb). Paket-paket yang akan dipaketkan
ke dalam distro debian haruslah menuruti Debian Free Software Guidelines.

Selain itu, paket-paket tersebut harus melalui 3 fase penyeleksian paket yakni
stabel, testing, dan unstable. Untuk melewati ke tiga fase tersebut, sampai
mendapatkan predikat software stable biasanya memakan waktu yang cukup
lama. Patut untuk diketahui bahwa saat ini versi debian baru mencapai versi 3.0
padahal distro ini telah berdiri sebelum distro RedHat ataupun SuSE. Interval
waktu dari satu rilis ke rilis berikutnya biasanya memerlukan waktu sekitar
empat tahunan.

Isu yang banyak didengungkan orang terhadap distro ini adalah masalah
kestabilan, sehingga tidak mengherankan jika distro ini banyak digunakan
sebagai dasar pembuatan distro lain.

Sistem operasi universal
------------------------

Dalam perjalananya, debian merupakan satu-satunya distro yang
dapat mendukung 11 +2 arsitektur antara lain 2-bit PC / Intel 
IA-32 (i386), 64-bit PC / Intel EM64T / x86-64 (amd64), Motorola/
IBM PowerPC (powerpc), Sun/Oracle SPARC (sparc), MIPS (mips (big-
endian) and mipsel (little-endian)), Intel Itanium (ia64), IBM 
S/390 (s390), ARM EABI (armel), ARM hard float (armfh) dan s390x. 
Tambahan dua arsitektur lagi adalah kfreebsd-i386 dan kfreebsd-
amd64 yang menggunakan kernel freeBSD [#]_.

"Social contract" dengan komunitas perangkat lunak terbuka
----------------------------------------------------------

Debian mempunyai *social contract* yang dibuat oleh Ian Murdock, isi kontra sosial ini adalah:

 - Debian akan 100% terbuka
   Kami menyediakan pedoman yang kita gunakan untuk menentukan apakah suatu
   pekerjaan itu bebas terdapat dalam *Debian Free Software Guidelines*. Kami
   berjanji bahwa sistem debian dan semua komponennya akan selalu terbuka sesuai
   debian pedoman ini. Kami akan mendukung orang yang membuat atau menggunakan 
   karya terbuka atau non-bebas pada Debian. Kami tidak akan pernah membuat
   kebutuhan sistem untuk menggunakan komponen non-bebas.
 - Kami akan memberikan (Debian) kembali ke komunitas sumber terbuka
   Ketika kami menulis komponen dalam sistem Debian, kami akan memberikan
   lisensinya yang konsisten dengan *Debian Free Software Guidelines*. Kami akan
   membuat sistem terbaik semampu kami, sehingga karya bebas ini dapat
   didistribusikan dan digunakan. Kami akan berkomunikasi seperti perbaikan bug,
   kemajuan, dan permintaan pengguna kepada pembuat hulu yang masuk ke dalam
   sistem kami.  
 - Kami tidak akan menyembunyikan masalah
   Kami akan menyimpan basisdata bug terbuka untuk publik sepanjang waktu. Laporan
   berkas orang akan terlihat oleh orang lain.
 - Prioritas kami adalah pengguna dan perangkat lunak terbuka
   Kami akan dipandu oleh kebutuhan pengguna dan komunitas perangkat lunak
   terbuka. Kami akan menempatkan kepentingan mereka dalam prioritas utama kami.
   Kami akan mendukung kebutuhan dari pengguna untuk berjalan di berbagai macam
   lingkungan komputasi. Kami tidak akan keberatan untuk karya non-bebas yang
   dimaksudkan untuk digunakan di sistem Debian, atau mencoba untuk membuat
   biaya untuk orang-orang yang membuat atau menggunakan karya tersebut. Kami
   akam memperbolehkan orang lain untuk membuat distribusi yang mengandung sistem
   Debian dan karya lain, tanpa biaya dari kami. Dalam kelanjutan hal tersebut,
   kami akan menyediakan sistem integrated dari bahan berkualitas tinggi dengan
   tanpa batasan hukum yang akan mencegah pengguna ke sistem.
 - Karya yang tidak memenuhi standard perangkat lunak kami,
   Kami mengakui bahwa beberapa pengguna kami memerlukan karya-karya yang tidak
   sesuai dengan *Debian Free Software Guidelinues*. Kami telah menciptakan
   area contrib dan non-free dalam arsip kami untuk karya-karya ini. Paket dalam
   area ini bukan bagian dari sistem Debian, meskipun telah diatur untuk digunakan
   di Debian. Kami mendorong produsen CD untuk membaca lisensi dari paket di
   area ini untuk menentukan apakah mereka dapat mendistribusikan paket pada
   CD mereka. Dengan demikian meskipun karya non-free bukan merupakan bagian dari
   Debian, kamu mendukung penggunaan mereka untuk menyediakan infratruktur untuk
   paket non-free (seperti bug tracking system dan milis).
   
.. Note::
   	Pembuat hulu, yang berasal dari upstream author adalah orang yang membuat program
   	dan memelihara paket itu. Sedangkan Debian Developer adalah orang yang membuat
   	program dari hulu dapat dijalankan dengan baik di Debian.
   	
   
Mendapatkan Debian
------------------

Untuk informasi tentang bagaimana mengunduh Dbeian GNU/Linux dari internet
atau dari pembelian resmi CD Debian, silakan lihat `halaman web penyaluran 
<http://www.debian.org/distrib/>`_. Daftar dari `cermin Debian 
<http://www.debian.org/distrib/ftplist>`_ berisikan daftar lengkap cermin Debian,
sehingga anda dapat dengan mudah mencari yang terdekat dengan anda.

Debian dapat di upgrade dengan mudah setelah pemasangan. Jika anda  menginnginkan,
Prosedur instalasi akan membantu membangun sistem sehingga anda dapat mengupgrade
setelah instalasi selesai.

Di Indonesia, terdapat banyak cermin CD Debian seperti:

- Kambing UI, http://kambing.ui.ac.id/iso/debian/
- Datautama, http://kartolo.sby.datautama.net.id/debian-cd/

Turunan Debian
--------------

Berikut ini beberapa distro turunan Debian GNU/Linux yang dapat anda lihat di
`situs resmi Debian <http://www.debian.org/misc/children-distros>`_:

 - `Demo Linux <http://www.demolinux.org)>`_
   Merupakan distro GNU/Linux yang dapat dijalankan tanpa instalasi ataupun
   partisi hardisk.
 - `Gibraltar <http://www.gibraltar.vianova.at>`_
   Merupakan distro yang khusus diperuntukkan untuk firewall/router
 - `Knoppix <http://www.knopper.net/knoppix/index-en.html>`_
   Distro ini salah distro yang banyak digunakan oleh pengguna GNU/Linux
   karena kemudahan dalam pemakainnya serta tidak perlu melakukan instalasi.
   Selain itu, dengan distro ini anda dapat meng-hardisk-kan knoppix. Dukungan
   hardware juga sangat lengkap sehingga distro ini sangat bagus untuk digunakan
 - `Libranet <http://www.libranet.com>`_
   Distro ini memaketkan paketnya dengan kemudahan yang diberikan dalam hal
   instalasi.
 - Linex
   Distro Linex dikembangkan oleh “the regional goverment of Extramadura
   (Spain)” dengan tujuan untuk memigrasikan seluruh operation system. Distro ini
   khusus ditujukan untuk keperluan perkantoran, dan bisnis.
 - `Stromix <http://www.stromix>`_
   Para pengembang distro Stromix mengklaim distro buatannya sebagai distribusi
   GNU/Linux yang sangat stabil dan aman.
 - `Ubuntu <http://www.ubuntu.com>`_
   Ubuntu merupakan turunan dari Debian yang mempunyai banyak pengguna, hal ini dikarenakan
   filosofi Ubuntu yang menganut sistem *just work*. Dengan paham tersebut, Ubuntu lebih
   memanjakan pengguna.
 - `BlankOn <http://www.blankonlinux.or.id>`_
   BlankOn adalah distro lokal turunan debian yang mengusung konten lokal Indonesia.

Rilis Debian GNU/Linux
----------------------

Nama rilis Debian GNU/Linux diambil dari *toy story movies* seperti Bo,
Hamm, slink, Potato, Woody, Sid, Sarge, Lenny, Squeeze, Wheezy, Jessie. 
Sedangkan untuk status kestabilan paketnya terbagi atas versi stable, 
frozen, testing, unstable dan experimental.

Debian menggunakan nama lain untuk penyebutan sebelum rilis, seperti sid
unstable, testing untuk wheezy, stable untuk squeeze, oldstable untuk lenny.
Setelah rilis, nama lain akan bergeser, jika wheezy dirilis hari ini maka,
wheezy akan menjadi stable, squeeze akan menjadi oldstable, jessie menjadi
testing. Khusus untuk sid, akan selalu digunakan untuk nama lain unstable.

Rilis unstable (sid) diperuntukkan bagi paket-paket baru dan update-an 
paket dari upstream.

Sedangkan penggunaan paket terbaru dan tidak mengandung resiko dapat
menggunakan rilis paket testing. Sedangkan rilis experimental, sesuai 
dengan namanya hanya untuk paket ujicoba. Beberapa paket melalui 
experimental dahulu biasanya dikarenakan
problem migrasi pustaka sebelum pustaka tersebut benar-benar diupload ke 
unstable.

Waktu pengujian dari rilis unstable hingga mencapai testing dibutuhkan waktu
sekitar beberapa minggu. Rilis paket frozen merupakan tahapan dimana paket-
paket software yang telah melewati rilis testing akan digabungkan ke dalam
distro Debian GNU/Linux untuk diuji kinerja paket softwarenya dan
memastikan tidak adanya bug kritikal pada paket software tersebut. Pada momen frozen ini
Debian akan dirilis dalam waktu dekat. Semua paket tidak bisa masuk ke testing kecuali
paket tersebut diupload untuk menyelesaikan bug kritikal atau RC. Gambar berikut adalah
ilustrasi alur rilis Debian [#]_:

.. image:: images/Debianpackagecycl.png

Tahapan selanjutnya adalah rilis paket stable dimana waktu pengujian rilis ini
membutuhkan waktu sekitar 8 bulan atau lebih. Berikut ini rilis distro Debian
GNU/Linux. [#]_:

+--------+---------+------------+-------+---------------+-----------------------+
| Version|Code name|Release date|Ports	|Packages	|Supported until	|
+========+=========+============+=======+===============+=======================+
|+1.1	 |buzz	   |1996-06-17	|1    	|474		|1996-09		|
+--------+---------+------------+-------+---------------+-----------------------+
|1.2	 |rex	   |1996-12-12	|1	|848		|1996			|
+--------+---------+------------+-------+---------------+-----------------------+
|1.3	 |bo	   |1997-06-05	|1	|974		|1997			|
+--------+---------+------------+-------+---------------+-----------------------+
|2.0	 |hamm	   |1998-07-24	|2	| ~ 1,500	|1998			|
+--------+---------+------------+-------+---------------+-----------------------+
|2.1	 |slink	   |1999-03-09	|4	| ~ 2,250	|2000-12		|
+--------+---------+------------+-------+---------------+-----------------------+
|2.2	 |potato   |2000-08-15	|6	| ~ 3,900	|2003-04		|
+--------+---------+------------+-------+---------------+-----------------------+
|3.0	 |woody	   |2002-07-19	|11	| ~ 8,500	|2006-08		|
+--------+---------+------------+-------+---------------+-----------------------+
|3.1	 |sarge	   |2005-06-06	|11	| ~ 15,400	|2008-04		|
+--------+---------+------------+-------+---------------+-----------------------+
|4.0	 |etch	   |2007-04-08	|11	| ~ 18,000	|2010-02-15		|
+--------+---------+------------+-------+---------------+-----------------------+
|5.0     |lenny    |2009-02-14	|12	| ~ 23,000	|2012-02-06		|
+--------+---------+------------+-------+---------------+-----------------------+
|6.0     |squeeze  |2011-02-06  |9+2[A]	| ~ 29,000	|TBA			|
+--------+---------+------------+-------+---------------+-----------------------+
|7.0     |wheezy   |TBA		|TBA	|TBA	  	|TBA			|
+--------+---------+------------+-------+---------------+-----------------------+
|8.0	 |jessie   |TBA		|TBA	|TBA	 	|TBA			|
+--------+---------+------------+-------+---------------+-----------------------+

Gambar berikut merupakan lokasi para pengembang debian GNU/Linux
berdasarkan negara tempat para pengembang [#]_

.. image:: images/dd-map.png

.. [#] http://www.debian.org/News/2011/20110205a
.. [#] Sumber http://en.wikipedia.org/wiki/Debian
.. [#] Sumber http://en.wikipedia.org/wiki/File:Debian-package-cycl.svg
.. [#] http://www.debian.org/devel/developers.loc
.. _GNU Project: http://www.gnu.org/software/software.html

