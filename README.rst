debian-ebook
============

Ebook debian dalam bahasa indonesia, ebook ini pertama kali dipublikasikan
oleh Askari Azikin dan ditulis ulang lagi oleh Tim Debian Indonesia. (sudah
mendapatkan ijin dari mas Kari)

Tujuan dari penulisan ini adalah pengguna debian agar mendapatkan informasi
tentang debian yang up-to-date

Kontribusi
----------

Dalam penyusunan ebook debian ini, garis besar yang akan ditulis antara lain
seputar distro debian mulai dari pemasangan sampai kedalam pengaturan lanjut.
Silakan melihat ebook mas Askari Azikin dan debian-handbook sebagai acuan.
Jadi untuk kopi paste dari ebook mas Askari tidak apa-apa, yang penting kita ubah
ke restructured format dulu dan bisa disunting, agar bisa dikerjakan rame-rame

Rilis debian yang akan dipakai dalam ebook ini adalah wheezy (saat ini testing).


Unduh
-----

Silakan menyalin berkas pdf dari `sini <http://doc.deb-id.org/ebook/askari_azikin/>`_ 
dan salin kedalam format reStructuredText.

Untuk mengunduh silakan ketik::

	git clone git://github.com/debian-id/debian-ebook.git

Kemudian sunting dan lakukan permintaan merge.

Rujukan reStructuredText
------------------------

Berikut rujukan reStructuredText:

 - `Quick reStructuredText <http://docutils.sourceforge.net/docs/user/rst/quickref.html>`_
 - `reStructuredText Markup Specification <http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html>`_
 - `Online reST to HTML conversion <http://www.tele3.cz/jbar/rest/rest.html>`_
 - `Online reStructuredText editor <http://rst.ninjs.org/>`_


Testing!
--------

install dulu paket-paket berikut::

	sudo apt-get install python-sphinx texlive-fonts-recommended texlive-latex-extra texlive-fonts-extra dvipng

Untuk melihat hasil keluaran, bisa mengetikkan::

	make html
	make latexpdf

Masukan dan patch selalu diterima.
Terimakasih!

Mahyuddin Susanto <udienz@gmail.com>
