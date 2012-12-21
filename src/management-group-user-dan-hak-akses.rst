===================================
MANAJEMEN GROUP, USER,DAN HAK AKSES
===================================

Pentingnya Membuat Group dan User Account
=========================================
Pada bab sebelumnya telah dijelaskan bahwa kepemilikan sebuah file atau
direktori dapat ditentukan oleh user pembuatnya. File atau direktori tersebut
tidak dapat diakses oleh user lain baik yang tergabung dalam group yang sama
atau other tanpa adanya pemberian hak akses oleh user pemilik.
Kerahasian sebuah data khususnya data pribadi merupakan hal yang sangat
penting, sehingga adanya tindakan pengamanan terhadap data yang
bersangkutan. Disinilah pentingnya pembuatan group dan user account pada
sistem GNU/Linux. Setiap direktori atau file yang terdapat pada hirarki sistem
file GNU/Linux tidak semuanya dapat diakses oleh user lain selain oleh user
root sebagai pemegang hak akses penuh pada sistem GNU/Linux.
Pengaturan hak akses terhadap sebuah file atau direktori menentukan dapat
tidaknya file atau direktori tersebut dapat diakses oleh orang lain selain pemilik
dan superuser (root). Setiap group pada sistem GNU/Linux akan membawahi
user-user yang terdapat pada sistem. Sebuah group sangat diperlukan untuk
pengaturan user seperti pada contoh kasus pada bab sebelumnya.

Manajemen group dengan Command Line
===================================

Menambahkan Group Account
-------------------------
Pembuatan group menentukan pengaturan hak akses file atau direktori yang
dapat digunakan oleh setiap user dalam satu group. Penambahan group pada
sistem debian GNU/Linux dapat menggunakan perintah berikut:

::

	debian:~# groupadd –g value namagroup

Catatan:

- -g: group ID
- value: nilai group ID
- namagroup: diisikan dengan nama group yang ada ingin buat.

Misal:

Anda ingin membuat sebuah group dengan nama linuxer, maka perintah yang
digunakan adalah::

	debian:~# groupadd –g 500 linuxer

Menghapus Group Account
Penghapusan group account pada sistem GNU/Linux dapat menggunakan perintah berikut::

	debian:~# groupdel namagroup

Misal:

Penulis akan menghapus group account linuxer yang terdapat pada sistem
debian GNU/linux, maka perintah yang digunakan adalah::

	debian:~# groupdel linuxer

Manajemen Group Account dengan GUI
==================================
Pada start menu, klik System → User Manager (Kuser).

.. figure:: images/kmenu-group-user.png

**Start menu KDE 3.2 debian GNU/Linux**

Selanjutnya sistem akan meminta anda memasukkan password user root.klik [ok]
untuk melanjutkan ke proses berikutnya.

.. figure:: images/kdsu.png

**Jendela dialog untuk akses ke user root**

Pembuatan group account dapat anda lakukan dengan mengklik group pada
main bar KDE User Manager-KUser seperti yang tampak pada gambar berikut.
Sorot opsi Add... untuk menambah group baru.

.. figure:: images/manager-group.png
   
**Manajemen group GNU/Linux**



















