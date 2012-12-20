Debian GNU/Linux
================

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
`GNU project`_. [#]_

Distro ini sering disebut-sebut sebagai pure GNU/Linux karena satu-satunya
distro yang sampai saat ini masih menuruti asas free software. Debian sendiri
memiliki sistem pemaketan sendiri (\*.deb). Paket-paket yang akan dipaketkan
ke dalam distro debian haruslah menuruti Debian Free Software Guidelines.

Selain itu, paket-paket tersebut harus melalui 3 fase penyeleksian paket yakni
stabel, testing, dan unstable. Untuk melewati ke tiga fase tersebut, sampai
mendapatkan predikat software stable biasanya memakan waktu yang cukup
lama. Patut untuk diketahui bahwa saat ini versi debian baru mencapai versi 6.0
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
   	Pembuat hulu, yang berasal dari upstream author adalah orang yang 
    	membuat program
   	dan memelihara paket itu. Sedangkan Debian Developer adalah orang yang 
    	membuat program dari hulu dapat dijalankan dengan baik di Debian.
   	

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
paket dari upstream. Penggunaan paket terbaru dan tidak mengandung resiko 
dapat menggunakan rilis paket testing. Sedangkan rilis experimental, sesuai 
dengan namanya hanya untuk paket ujicoba. Beberapa paket melalui 
experimental dahulu biasanya dikarenakan
problem migrasi pustaka sebelum pustaka tersebut benar-benar diupload ke 
unstable.

Waktu pengujian dari rilis unstable hingga mencapai testing dibutuhkan waktu
sekitar beberapa minggu. Rilis paket frozen merupakan tahapan dimana paket-
paket software yang telah melewati rilis testing akan digabungkan ke dalam
distro Debian GNU/Linux untuk diuji kinerja paket softwarenya dan
memastikan tidak adanya bug kritikal pada paket software tersebut. Pada 
momen frozen ini
Debian akan dirilis dalam waktu dekat. Semua paket tidak bisa masuk ke 
testing kecuali
paket tersebut diupload untuk menyelesaikan bug kritikal atau RC. Gambar 
berikut adalah
ilustrasi alur rilis Debian [#]_:

.. image:: ../images/Debianpackagecycl.png

Tahapan selanjutnya adalah rilis paket stable dimana waktu pengujian rilis ini
membutuhkan waktu sekitar 8 bulan atau lebih. Berikut ini rilis distro Debian
GNU/Linux. [#]_

+--------+-----------+---------------+----------+-----------+-----------------+
| Versi  | Kode nama | Tanggal rilis | Ports    | Packages  | Didukung hingga |
+========+===========+===============+==========+===========+=================+
| +1.1   | buzz      | 1996-06-17    | 1        | 474       | 1996-09         |
+--------+-----------+---------------+----------+-----------+-----------------+
| 1.2    | rex       | 1996-12-12    | 1        | 848       | 1996            |
+--------+-----------+---------------+----------+-----------+-----------------+
| 1.3    | bo        | 1997-06-05    | 1        | 974       | 1997            |
+--------+-----------+---------------+----------+-----------+-----------------+
| 2.0    | hamm      | 1998-07-24    | 2        | ~ 1,500   | 1998            |
+--------+-----------+---------------+----------+-----------+-----------------+
| 2.1    | slink     | 1999-03-09    | 4        | ~ 2,250   | 2000-12         |
+--------+-----------+---------------+----------+-----------+-----------------+
| 2.2    | potato    | 2000-08-15    | 6        | ~ 3,900   | 2003-04         |
+--------+-----------+---------------+----------+-----------+-----------------+
| 3.0    | woody     | 2002-07-19    | 11       | ~ 8,500   | 2006-08         |
+--------+-----------+---------------+----------+-----------+-----------------+
| 3.1    | sarge     | 2005-06-06    | 11       | ~ 15,400  | 2008-04         |
+--------+-----------+---------------+----------+-----------+-----------------+
| 4.0    | etch      | 2007-04-08    | 11       | ~ 18,000  | 2010-02-15      |
+--------+-----------+---------------+----------+-----------+-----------------+
| 5.0    | lenny     | 2009-02-14    | 12       | ~ 23,000  | 2012-02-06      |
+--------+-----------+---------------+----------+-----------+-----------------+
| 6.0    | squeeze   | 2011-02-06    | 9+2      | ~ 29,000  | TBA             |
+--------+-----------+---------------+----------+-----------+-----------------+
| 7.0    | wheezy    | TBA           | TBA      | TBA       | TBA             |
+--------+-----------+---------------+----------+-----------+-----------------+
| 8.0    | jessie    | TBA           | TBA      | TBA       | TBA             |
+--------+-----------+---------------+----------+-----------+-----------------+

Debian sebagai organisasi
-------------------------

Sesuatu hal yang tidak mungkin untuk mengelola suatu distro tanpa organisasi
yang dapat dipercaya. Begitu juga dengan Debian, Debian memiliki struktur
organisasi yang jelas dan terbuka untuk umum. Seperti pada struktur
organisasi pada umunya, Debian memiliki ketua, komisi teknis, sekretaris,
dan beberapa sub divisi.

Berikut adalah rincian struktur organisasi Debian:

 * Petugas

   - Ketua, Stefano Zacchiroli.
   - Sekretaris, Kurt Roeckx dan Neil McGovern.
   - Komisi Teknis, Bdale Garbee (ketua), Russ Allbery, Don Amstrong,
     Andreas Barth, Ian Jackson, Steve Lengasek, Colin Watson.
     
 * Tim Teknis

   - Arsip FTP, bertanggung jawab sebagai pengelola arsip dan berkas berkas
     di Debian.
   - Backports, bertanggung jawab untuk menyediakan paket terbaru diluar
     rilis stable.
   - Menejemen rilis, bertanggung jawab untuk menentukan apakah Debian siap
     untuk rilis, menentukan apakah paket dapat dari pembaharuan dapat di
     unggah ke rilis stabil, menentukan apakah diperbolehkanya transisi
     pustake paket 
   - Jaminan kualitas, bertanggung jawab akan kualitas paket dan kualitas
     Debian pada umumnya
   - Instalasi, tim ini bertanggung jawab bagaimana prosedur instalasi
     dan membuat instalasi yang baik.
   - Dokumentasi, menyediakan dokumentasi proyek Debian
   - CD Image, bertanggung jawab untuk menyediakan distribusi CD/DVD Debian.
   - Buildd, bertanggung jawab untuk menyediakan dan memelihara mesin mesin
     pembangun paket.
   - Debian ports, menyediakan paket debian kedalam arsitektur arsitektur 
     tertentu
   - Tim Tim lain, seperti penerjemahan, pemaketan yang spesifik terhadap
     teman tertentu.

Debian secara tahunan akan mengadakan pengumutan suara [#]_ untuk menentukan
ketua proyek, dan hanya bisa diikuti oleh anggota proyek.

Debian Developer
----------------

Debian Developer adalah anggota proyek Debian resmi dan berhak mendapatkan
akses penuh proyek Debian. Beberapa fasilitas Debian Developer adalah:

 - Dapat mengikuti pengumutan suara yang dilakukan oleh proyek Debian.
 - Mendapatkan akses ke beberapa mesin Debian.
 - Mendapatkan email debian.org.
 - Dapat mengunggah paketnya langsung tanpa melalui perantara.

Pada saat ini, jumlah Debian Developer adalah kurang lebih 951 [#]_
Gambar berikut merupakan lokasi para pengembang debian GNU/Linux
berdasarkan negara tempat para pengembang [#]_

.. image:: ../images/dd-map.png

.. Note::
    Sayangnya, hingga sekarang belum ada satupun dari warga Indonesia yang
    menjadi Debian Developer.

Debian Maintainer
-----------------

Umumnya pada tahap menjadi Debian Developer, seseorang akan menjadi Debian
Maintainer dahulu, perbedaan mendasar dari keduanya adalah hak upload.
Seorang Debian Maintainer **hanya** dapat mengunggah paketnya tanpa
perantara, hal ini beda dengan Debian Developer yang dapat mengunggah
**semua** paket meskipun bukan dirinya yang menjadi pengelola paket.

.. Note::
    Berbeda dengan Debian Developer, di Indonesia baru ada satu Debian 
    Maintainer. 

.. _mendapatkan-debian:

Mendapatkan Debian
------------------

Untuk informasi tentang bagaimana mengunduh Dbeian GNU/Linux dari internet
atau dari pembelian resmi CD Debian, silakan lihat `halaman web penyaluran 
<http://www.debian.org/distrib/>`_. Daftar dari `cermin Debian 
<http://www.debian.org/distrib/ftplist>`_ berisikan daftar lengkap cermin Debian,
sehingga anda dapat dengan mudah mencari yang terdekat dengan anda.

Di Indonesia, terdapat banyak cermin CD Debian seperti:

- Kambing UI, http://kambing.ui.ac.id/iso/debian/
- Datautama, http://kartolo.sby.datautama.net.id/debian-cd/

.. [#] http://www.debian.org/intro/about
.. [#] http://www.debian.org/News/2011/20110205a
.. [#] http://en.wikipedia.org/wiki/File:Debian-package-cycl.svg
.. [#] http://en.wikipedia.org/wiki/Debian
.. [#] http://www.debian.org/vote/2012/vote_001
.. [#] http://www.debian.org/vote/2012/vote_002_quorum.log
.. [#] http://www.debian.org/devel/developers.loc

.. _GNU Project: http://www.gnu.org/software/software.html
