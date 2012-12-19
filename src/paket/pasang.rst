============================
Instalasi paket di GNU/Linux
============================

Di sistem Debian, kita dapat memasang sebuah program dari kumpulan file
installer. Program atau paket (kita akan lebih menggunakan kata paket)
biasanya berasal dari kode sumber dari upstream yang kemudian di atur
sehingga dapat berjalan dengan baik di Debian. Di Debian menggunakan berkas
dengan extensi \*.deb untuk paket yang langsung bisa diinstall. Adapun
berkas lain yang dapat digunakan untuk instalasi debian adalah:

 - Berkas \*.tar.gz, \*.tar.bz2, \*.zip, biasanya berkas-berkas ini adalah
   berkas dari upstream yang berisikan kode sumber yang belum dimodifikasi.
 - Berkas \*.deb, berkas ini adalah berkas installer umum yang digunakan
   oleh debian dan turunannya. Sesuai debian *Debian Free Software Guide*
   paket Debian akan menyediakan kode sumber yang terbuka untuk publik.
   Dalam pemaketan Debian, ada beberapa berkas yang akan di distibusikan
   yaitu:

   - Berkas kode sumber upstream. Berkas ini cirinya dapat dilihat dari
     ekstensinya, biasanya adalah \*.orig.tar.gz, \*.orig.tar.bz2, dan
     \*.xz
   - Berkas modifikasi debian pada berkas sumber. Untuk melihat apa saja
     yang berubah atau apa yang dikerjakan di debian dapat dilihat dari
     berkas yang mempunyai extensi \*.diff.gz untuk metode pemaketan lama
     dan \*.debian.tar.gz untuk metode pemaketan baru (quilt).
   - Berkas biner, berkas biner ini adalah berkas hasil kompilasi antara
     kode sumber dan berkas diff. Berkas biner ini ada dua macam yaitu
     \*.deb dan \*.udeb. Perbedaannya adalah \*.deb untuk instalasi paket
     pada umumnya, sedang \*.udeb adalah installer pada waktu instalasi
     pertama kali yang disebut daalam kelompok paket debian-installer.

Struktur Paket Software Debian GNU/Linux
----------------------------------------

Debian GNU/linux memiliki standar pemaketan software tersendiri yakni
dengan ekstensi deb. Berikut format struktur paket software di Debian:
namapaket_upstream.version-revisidebian.deb


.. image :: ../images/package-version.png

Contoh pada paket vlc, pada rilis wheezy mempunyai versi 2.0.3-4 yang
berarti:

 - 2.0.3 adalah versi upstream
 - 4 adalah versi terahir revisi debian

Sedangkan untuk

Instalasi Paket Software dari Source Code
-----------------------------------------
Instalasi paket software dari kode sumber (source code) merupakan cara instalasi
yang berlaku umum untuk semua distribusi GNU/Linux yang ada. Perintah
umum yang sering digunakan adalah::

	:~# tar zxvf paketsoftware.tar.gz
	:~# tar jxvf paketsoftware.tar.bz2

.. Note::
	Opsi -x dan -j digunakan untuk tipe kompresi yang berbeda. Opsi -x untuk tipe
	kompresi \*.gz dan opsi -j untuk tipe kompresi \*.bz2.

Setelah ekstraksi paket software, langkah berikutnya
adalah konfigurasi kompilasi, dan terakhir adalah instalasi software.::

	:~# cd paketsoftware
	:~# ls
	:~# more readme
	:~# ./configure
	:~# make
	:~# make install
	:~# make clean

.. warning::
	Disarankan membaca readme setiap kali instalasi paket software sehingga dapat memudahkan dalam proses instalasi.

Misal:

Penulis ingin menginstal paket videolan client (vlc-0.8.1.tar.bz2). Perintah yang
digunakan adalah::

	:~# tar xjvf vlc-0.8.1.tar.bz2
	:~# cd vlc-0.8.1
	:/vlc-0.8.1# ./configure
	:/vlc-0.8.1# make
	:/vlc-0.8.1# make install
	:/vlc-0.8.1# make clean

Instalasi Paket Software dari Binary Code
-----------------------------------------
Distribusi debian GNU/Linux memiliki 3 buah cara dalam instalasi paket
software untuk binary code (deb). Berikut cara penggunaan perintah instalasi
software dengan ``dpkg``.


