============================
Instalasi paket di GNU/Linux
============================

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

Struktur Paket Software Debian GNU/Linux
----------------------------------------

Debian GNU/linux memiliki standar pemaketan software tersendiri yakni
dengan ekstensi deb. Berikut format struktur paket software debian GNU/Linux.

.. image :: images/package-version.png
