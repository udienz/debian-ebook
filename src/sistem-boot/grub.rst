GRUB: The Grand Unified Boot Loader 
===================================

Grub (the grand unified bootloader) adalah sebuah boot loader yang didesain untuk mengatasi kekurangan dari Lilo boatloader sebagai bootloader konvensional dari linux. Grub dilengkapi dengan feature-feature baru serta tampilan yang lebih elegan dibanding dengan Lilo karena dilengkapi dengan tampilan grafis yang tentu saja lebih menarik jika dibanding dengan mode text seperti yang ada pada lilo bootloader. 

Grub pertama kali diperkenalkan oleh Erich Boleyn pada tahun 1995 saat mencoba mem-boot OS GNU HURD dengan University the Multiboot Mach 4 microkernel (sekarang dikenal dengan GNU Mach). 


Mengganti lilo boat loader dengan grub 
--------------------------------------

Untuk mengganti lilo boot loader dengan grub, perintah yang digunakan adalah::

   ~# apt-get install grub 
   ~# grub-install /dev/hda 
   ~# update-grub 

**Asumsi:**
Anda menginstal boot loader di */dev/hda*, dan letak partisi GNU/Linux berada di */dev/hda2* sedangkan Windows XP anda berada di */dev/hda1*. Kemudian edit file konfigurasi ``/boot/grub/menu.lst`` untuk mengganti dua baris berikut::

   # kopt=root=/dev/hda1 ro 
   # groot=(hd0,0) 
   
ganti dengan baris berikut::

   # kopt=root=/dev/hda2 ro 
   # groot=(hd0,1) 
   
.. Note::
   Anda tidak perlu menghilangkan tanda # pada bagian awal dari baris tersebut. Tambahkan pula baris berikut::
   
      title          Windows XP 
      rootnoverify   (hd0,0) 
      makeactive 
      chainloader    +1 
      
Selanjutnya reboot komputer dengan perintah::

   ~# reboot 

   
Update Boot Loader Grub secara Otomatis saat Instalasi Kernel Baru 
------------------------------------------------------------------

Ketika menginstall kernel baru, anda dapat menambahkan kernel tersebut ke dalam menu list secara otomatis tanpa melakukan pengeditan lagi. Tambahkan baris berikut pada file konfigurasi ``/etc/kernel-img.conf``::

   # Turn off lilo stuff 
   do_symlinks = no 
   do_bootloader = no 
   
   # Initrds are OK for GRUB 
   do_initrd = yes 
   
   # Run cool GRUB stuff 
   postinst_hook = /sbin/update-grub 
   postrm_hook = /sbin/update-grub 

   
Boot Loader GRUB Tertimpa oleh Ms-Windows 
-----------------------------------------

Boot loader grub ataupun lilo biasanya akan tertimpa oleh boot loader windows saat anda melakukan instalasi windows baru atau saat anda mengubah posisi master-slave hardisk. Perintah berikut akan mengembalikan boot loader grub. 
Boot sistem anda dengan menggunakan diskboot (floppy, atau CD installer debian GNU/Linux), kemudian pada prompt ketikkan perintah berikut::

   boot: rescue root=/dev/hda2 
   
atau 

::

   boot: rescbf24 root=/dev/hda2 
   
Setelah menekan tombol enter, maka Debian GNU/Linux dapat anda gunakan kembali. 
Instal kembali boot loader GRUB anda dengan perintah berikut.::

   ~# grub-install /dev/hda 
   
Reboot sistem dan boot loader grub anda akan berfungsi kembali sebagaimana mestinya. 


Boot Loader GRUB tidak dapat Meload Windows XP pada Partisi Master Slave 
------------------------------------------------------------------------

Jika windows berada pada partisi primary slave, maka secara default boot loader GRUB tidak dapat me-load windows. Salah satu solusi yang dapat anda lakukan adalah melakukan sedikit perubahan pada konfigurasi grub. 
Pada file konfigurasi ``/boot/grub/menu.lst``, tambahkan baris berikut::

   title winxp
   map (hd0) (hd1)
   map (hd1) (hd0)
   rootnoverify (hd1,0) 
   makeactive 
   chainloader +1 



