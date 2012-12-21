Repositori Debian
=================

Debian mempunyai koleksi paket yang sangat banyak, semua paket yang
didistribusikan oleh Debian terkumpul dalam satu arsip yang dinamakan
dengan repository Debian. Repository Debian terdiri atas kode sumber
upstream, paket biner dan berkas perbedaan antara paket kode sumber dan
perubahan di debian.

Arsip Debian didistribusikan di ratusan server di internet keseluruh dunia.
Hal ini dapat membantu mesin utama Debian dan pengguna karena jika kita
mengambil arsip Debian dari tempat terdekat kita (misalnya dari kambing.ui.ac.id)
maka traffik ke server debian akan berkurang dan biasanya lebih cepat karena
traffik untuk mengunduh paket debian tidak perlu keluar Indonesia.

.. note::
    Hal ini berkaitan dengan routing jaringan komputer, sebagai perumpamaan
    apabila kita membeli buku lebih baik dari reseller bukan dari pabrik.
    Selain hemat ongkos, waktu kita juga mendapatkan buku dengan harga yang
    sama apabila kita membelinya dari pabrik.

Repositori ini nantinya akan dibutuhkan dalam pemasangan paket di
sistem Debian,
kecuali jika anda mempunyai repositori lokal maupun repositori CD lengkap
maka anda tidak perlu menggunakan repositori yang berada di internet.
**Kecuali** untuk repository keamanan dan pembaharuan, sangat disarankan
untuk mengambilnya dari internet.

Arsip Komponen Debian
---------------------

Di arsip Debian di bedakan menjadi beberapa macam komponen, antara lain main, contrib
dan non-free.

Arsip Komponen main
~~~~~~~~~~~~~~~~~~~

Arsip main adalah arsip utama Debian, semua paket dalam instalasi Debian harus
masuk dalam main. Untuk masuk kedalam arsip main, paket-paket harus bebas di
distribusikan ulang, di ubah ulang oleh semua orang. Paket-paket dalam arsip
main harus sejalan dengan DFSG (*Debian Free Software Guidelines*), dan dalam
kompilasi pembangunan paket dan menjalankan paket, paket ini **tidak boleh** 
tergantung dengan paket diluar main.

Arsip Komponen contrib
~~~~~~~~~~~~~~~~~~~~~~

Paket dalam arsip contrib berisikan paket tambahan yang dibutuhkan untuk
dijalankan di Debian, namun membutuhkan ketergantungan pada paket yang berapa
diluar distribusi Debian (*non-free*) baik itu proses kompilasi maupun 
menjalankan paket.

Arsip Komponen non-free
~~~~~~~~~~~~~~~~~~~~~~~

Paket yang berada di arsip *non-free* adalah paket tambahan di Debian tapi
tidak sesuai dengan DFSG atau mempunyai masalah dalam distribusi. Hal ini
dikarenakan keterbatasan dalam modifikasi paket dan ada tidaknya kode
sumber.

Pengaturan Repositori Debian
----------------------------

Untuk mengambil paket dari server penyedia paket Debian di internet, kita
harus mengatur sistem kita dulu. Berkas pengaturan tersebut berada pada berkas
``/etc/apt/sources.list``, format penulisan repository umum di berkas tersebut 
adalah sebagai berikut::

    deb protokol://alamat-mirror/debian/ kode-rilis komponen #untuk paket biner
    deb-src protokol://alamat-mirror/debian/ kode-rilis komponen #untuk kode sumber

Sebagai contoh, kita akan menggunakan server repository ``ftp.de.debian.org``,
koneksi menggunakan protokol http, lokasi repositori direktory server adalah
``/debian/``, rilis stable, dengan komponen ``main``, ``contrib``, dan ``non-free``.
Maka penulisan repositorinya adalah::

    deb http://ftp.de.debian.org/debian/ stable main contrib non-free
    deb-src http://ftp.de.debian.org/debian/ stable main contrib non-free

Sedangkan untuk repo pembaharuan keamanan adalah sebagai berikut::

    deb http://ftp.de.debian.org/debian-security stable/updates main contrib non-free
    deb-src http://ftp.de.debian.org/debian-security stable/updates main contrib non-free

.. note:: Bagaimanakah penulisan repositori jika menggunakan server http://kambing.ui.ac.id/debian?

Arsip Repositori lain
---------------------

Debian mempunyai repositori tambahan, yaitu Debian Volatile dan Debian Backports

Debian Backports
~~~~~~~~~~~~~~~~

Debian Backports adalah repositori yang mengandung paket yang dikompile 
ulang dari dari testing (kebanyakan) dan unstable, sehingga paket paket 
tersebut dapat berjalan tanpa
pustaka baru di dalam Debian stable. Sangat dianjurkan untuk mengambil
beberapa paket saja daripada menggunakan backports pada keseharian.

Untuk menambahkan paket backports ke dalam sistem, kita harus menambahkan
alamat repository ke dalam ``/etc/apt/sources.list``. Seperti baris berikut::

    deb http://backports.debian.org/debian-backports stable-backports main

Kemudian lakukan update dengan::

    apt-get update

Kemudian untuk pemasangan paket, bisa menggunakan perintah berikut::

    apt-get -t stable-backports install nama-paket-yang-akan-dipasang

Debian Volatile
~~~~~~~~~~~~~~~

Debian Volatile adalah repositori paket yang mempunyai pembaharuan yang
cepat, seperti contohnya database virus pada clamav, database spam filter.
Dikarenakan cepatnya update, sangat tidak memungkinkan untuk melalui proses
panjang pengujian di Debian. Pada saat ini repositori volatile telah di
hentikan [#]_ dan diganti dengan repositori updates dan digabung kedalam
repositori utama debian.

Untuk menggunakan repositori ini kita harus menambahkan baris berikut
kedalam ``/etc/apt/sources.list``::

    deb http://ftp.de.debian.org/debian squeeze-updates main contrib non-free

.. [#] http://www.debian.org/News/2011/20110215
