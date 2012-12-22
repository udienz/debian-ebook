Instalasi Paket Software dari kode biner
========================================

Distribusi debian GNU/Linux memiliki 3 buah cara dalam instalasi paket
software untuk binary code (deb). Yaitu dpkg, apt-get, dan aptitude

dpkg
----

Tool instalasi dpkg ini merupakan program yang pertama kali digunakan dalam
instalasi paket software distro debian GNU/Linux sebelum muncul tool-tool lain
seperti dselect, apt-get, serta synaptic. Untuk melihat bagaimana penggunaan tool
dpkg, gunakan perintah berikut::

    debian:~# dpkg --help | more

Instalasi dengan dpkg
~~~~~~~~~~~~~~~~~~~~~

Penginstalan sebuah paket software (deb) dapat menggunakan perintah berikut
ini::

    debian:~# dpkg –i namapaket.deb

Misal: Penulis ingin menginstal paket software videolan client (vlc-0.8.1.deb), maka perintah yang digunakan adalah::

    debian:~# dpkg –i vlc-0.8.1.deb

atau menggunakan opsi -- install)

Unistall Paket Software
~~~~~~~~~~~~~~~~~~~~~~~

Uninstall software pada sistem debian GNU/linux dapat menggunakan perintah
berikut::

    debian:~# dpkg –r | --remove | -P | --purge | paketsoftware...

.. note::
    Opsi `-r` atau `--remove` akan menghapus paket software namun tidak
    membersihkan file konfigurasi. Hal ini bertujuan untuk mencegah konfigurasi
    ulang jika suatu saat software tersebut diinstal ke sistem debian GNU/Linux.
    Opsi `-P` atau `--purge` akan menghapus seluruh software termasuk file
    konfigurasi bawaan.

Misal: Penulis ingin menghapus paket software vlc dari sistem debian GNU/Linux,
maka perintah yang digunakan adalah::

    debian:~# dpkg --remove vlc-0.8.1 (atau cukup dengan `-r` saja)
    debian:~# dpkg --purge vlc-0.8.1 (atau cukup dengan `-P` saja)

Menampilkan Deskripsi Paket Software
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Untuk menampilkan informasi tentang software pada sistem debian GNU/Linux,
perintah yang digunakan adalah::

    debian:~# dpkg --print-avail paketsoftware

Misal: Penulis ingin menampilkan informasi software ``mc``.::

	debian:~# dpkg --print-avail mc
	Package: mc
	Priority: optional
	Section: utils
	Installed-Size: 5412
	Maintainer: Adam Byrtek <alpha@debian.org>
	Architecture: i386
	Version: 1:4.6.0-4.6.1-pre1-3
	Replaces: mc-common, manpages-pl (<= 20030210)
	Depends: e2fslibs, libc6 (>= 2.3.2.ds1-4), libcomerr2 (>= 1.33-
	3), libglib2.0-0 (>= 2.2.3), libgpmg1 (>= 1.19.6-1)
	Suggests: perl, mime-support
	Conflicts: mc-common, suidmanager (<< 0.52)
	Size: 1991720
	Description: Midnight Commander - a powerful file manager
	GNU Midnight Commander is a text-mode full-screen file manager.
	It
	uses a two panel interface and a subshell for command execution.
	It
	includes an internal editor with syntax highlighting and an
	internal
	viewer with support for binary files. Also included is Virtual
	Filesystem (VFS), that allows files on remote systems (e.g. FTP
	servers) and files inside archives to be manipulated like real
	files.
	
Mengekstrak Paket Software
~~~~~~~~~~~~~~~~~~~~~~~~~~

Mengekstrak/unpack software dapat menggunakan perintah berikut::

    debian:~# dpkg --unpack paketsoftware.deb

Misal: Penulis ingin mengekstrak software mc, maka perintah yang
digunakan adalah::

	debian:~# dpkg --unpack mc_4.8.3-10_amd64.deb 
	(Reading database ... 30428 files and directories currently installed.)
	Preparing to replace mc 3:4.7.0.9-1 (using mc_4.8.3-10_amd64.deb) ...
	Moving obsolete conffile /etc/mc/mc.charsets out of the way...
	Moving obsolete conffile /etc/mc/mc.lib out of the way...
	Moving obsolete conffile /etc/mc/Syntax out of the way...
	Unpacking replacement mc ...
	Processing triggers for man-db ..

Konfigurasi Paket Software Hasil Ekstraksi
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Konfigurasi software yang telah diekstrak dapat menggunakan perintah berikut::

	debian:~# dpkg --configure paketsoftware #(paket bukan dalam format .deb)

Misal: Penulis ingin mengkonfigurasi software mc yang telah diekstrak
sebelumnya. Perintah yang digunakan adalah::

	debian:~# dpkg --configure mc_4.8.3-10

Menampilkan Arsiktektur Komputer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Untuk menampilkan arsitektur komputer host yang akan diinstal paket software
dapat menggunakan perintah berikut::

	debian:~# dpkg --print-architecture
	amd64

Menampilkan Informasi sebuah Paket Software
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Untuk menampilkan informasi tentang sebuah paket software dapat
menggunakan perintah berikut::

	debian:~# dpkg –I paketsoftware.deb

Misal: Penulis ingin melihat informasi paket software mc sebelum
diinstal ke sistem debian GNU/Linux. Perintah yang digunakan adalah::

 dpkg -I mc_4.8.3-10_amd64.deb 
 new debian package, version 2.0.
 size 470358 bytes: control archive= 3282 bytes.
     225 bytes,    11 lines      conffiles            
    1058 bytes,    18 lines      control              
    3850 bytes,    66 lines      md5sums              
     879 bytes,    24 lines   *  postinst             #!/bin/sh
     664 bytes,    28 lines   *  postrm               #!/bin/sh
     344 bytes,    10 lines   *  preinst              #!/bin/sh
     157 bytes,    11 lines   *  prerm                #!/bin/sh
 Package: mc
 Version: 3:4.8.3-10
 Architecture: amd64
 Maintainer: Debian MC Packaging Group <pkg-mc-devel@lists.alioth.debian.org>
 Installed-Size: 1300
 Depends: e2fslibs (>= 1.42.2), libc6 (>= 2.11), libcomerr2 (>= 1.01), libglib2.0-0 (>= 2.24.0), libgpm2 (>= 1.20.4), libslang2 (>= 2.2.4), mc-data (= 3:4.8.3-10)
 Recommends: mime-support, unzip, perl
 Suggests: zip, bzip2, links | w3m | lynx, arj, file, xpdf | pdf-viewer, dbview, odt2txt, gv, catdvi, djvulibre-bin, imagemagick, python, python-boto, python-tz
 Section: utils
 Priority: optional
 Homepage: http://www.midnight-commander.org
 Description: Midnight Commander - a powerful file manager
  GNU Midnight Commander is a text-mode full-screen file manager. It
  uses a two panel interface and a subshell for command execution. It
  includes an internal editor with syntax highlighting and an internal
  viewer with support for binary files. Also included is Virtual
  Filesystem (VFS), that allows files on remote systems (e.g. FTP, SSH
  servers) and files inside archives to be manipulated like real files.

Mendaftar Seluruh File yang Terinstal bersama Paket
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Mendaftar seluruh file bawaan paket software instalasi dapat menggunakan
perintah berikut::

	debian:~# dpkg –L | --listfiles paketsoftware

Penulis ingin menampilkan seluruh file yang terinstal bersama paket software
`mc`. Perintah yang digunakan adalah::

	debian:~## dpkg -L mc
	/.
	/usr
	/usr/bin
	/usr/bin/mc
	/usr/lib
	/usr/lib/mc
	/usr/lib/mc/mc-wrapper.csh
	/usr/lib/mc/mc-wrapper.sh

Menampilkan Status Software yang Terinstal
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Untuk menampilkan status sebuah software yang terinstal dapat menggunakan
perintah berikut::

	debian:~# dpkg –s | --status paketsoftware

Misal: Penulis ingin menampilkan status dari software `mc`, maka perintah yang
digunakan adalah::

	debian:~# dpkg -s mc
	Package: mc
	Status: install ok unpacked
	Priority: optional
	Section: utils
	Installed-Size: 1300
	Maintainer: Debian MC Packaging Group <pkg-mc-devel@lists.alioth.debian.org>
	Architecture: amd64
	Version: 3:4.8.3-10
	Config-Version: 3:4.7.0.9-1
	Depends: e2fslibs (>= 1.42.2), libc6 (>= 2.11), libcomerr2 (>= 1.01), libglib2.0-0 (>= 2.24.0), libgpm2 (>= 1.20.4), libslang2 (>= 2.2.4), mc-data (= 3:4.8.3-10)
	Recommends: mime-support, unzip, perl
	Suggests: zip, bzip2, links | w3m | lynx, arj, file, xpdf | pdf-viewer, dbview, odt2txt, gv, catdvi, djvulibre-bin, imagemagick, python, python-boto, python-tz
	Conffiles:
	 /etc/mc/mc.keymap.emacs 2be8442a33951cb4d45e072b76b09dda
	 /etc/mc/mc.keymap 2ea38e5be6c591b56c9a62ee92d8256a
	 /etc/mc/mc.ext e7758e2f4b2f899f87502d54de690462
	 /etc/mc/edit.spell.rc 6c46bc0859a452b43f4fa7fb435b1325
	 /etc/mc/filehighlight.ini 715504387dcae9c3a3fcfa090414db5e
	 /etc/mc/mc.keymap.default 2ea38e5be6c591b56c9a62ee92d8256a
	 /etc/mc/mcedit.menu newconffile
	 /etc/mc/edit.indent.rc 008c6d0205315a87a977c7cd74a1526e
	 /etc/mc/mc.menu.sr b394f31ffaea9efd083c142491bc1ad7
	 /etc/mc/sfs.ini 316dc92f3fdec60a7aaf0866edc361db
	 /etc/mc/mc.menu 6187dd1b6029bfc91484000843635653
	Description: Midnight Commander - a powerful file manager
	 GNU Midnight Commander is a text-mode full-screen file manager. It
	 uses a two panel interface and a subshell for command execution. It
	 includes an internal editor with syntax highlighting and an internal
	 viewer with support for binary files. Also included is Virtual
	 Filesystem (VFS), that allows files on remote systems (e.g. FTP, SSH
	 servers) and files inside archives to be manipulated like real files.
	Homepage: http://www.midnight-commander.org
