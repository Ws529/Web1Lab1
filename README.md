# Git
1. Pengertian Git
Git adalah salah satu sistem pengontrol versi (Version Control System)
pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds. Git juga dikenal dengan distributed revision control (VCS terdistribusi),
artinya penyimpanan database Git tidak hanya berada dalam satu
tempat saja.

3. Cara Install Git
- Download Git, buka website resmi Git (git-scm.com).
- Kemudian unduh Git sesuai dengan spek komputer. jika ingin menggunakan 64bit, unduh yang 64bit. Begitu juga jika ingin menggunakan 32bit, unduh 32bit
- jika sudah terinstall, buka cmd atau powershell, lalu ketik git --version.

4. Menambahkan Global Config
konfigurasi ini bisa dilakukan untuk global repository atau individual repository, apabila belum melakukan konfigurasi akan mengakibatkan kegagalan saat menjalankan perintah git commit
Config Global Repository:
 - $ git config --global user.name "nama_user"
 - $ git config --global user.email "nama_user"

5. Membuat Reposiory Local
• Buka direktory aktif, misal: d:\bahasa_pemrograman1 (buka
menggunakan Windows Explorer)
• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
sehingga muncul git bash commad
• Buat direktory project praktikum pertama dengan nama praktikum1
  $ mkdir praktikum1
  $ cd praktikum1/
 Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya
masuk kedalam direktori tersebut dengan perintah cd (change
directory)
• direktory aktif menjadi: d:\bahasa_pemrograman1\praktikum1
Jalankan perintah git init, untuk membuat repository local.
  $ git init
• Repository baru berhasil di inisialisasi, dengan terbentuknya satu
direktori hidden dengan nama .git
• Pada direktori tersebut, semua perubahan pada working directory
akan disimpan.

6. Menambahkan File baru pada repository
• Untuk membuat file dapat menggunakan text editor, lalu menyimpan
filenya pada direktori aktif (repository)
c disini kita akan coba buat satu file bernama README.md (text file)
  $ echo "#latihan1" >> README.md
• File README.md berhasil dibuat.

7. Menambahkan File baru pada repository
• Untuk menambahkan file yang baru saja dibuat tersebut gunakan
perintah git add.
  $ git add README.md
• File README.md berhasil ditambahkan.

8. Commit (Menyimpan perubahan ke database)
• Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m “komentar commit”
  $ git commit -m "file pertama saya"
• Perubahan berhasil disimpan.

9. Menambahkan Remote Repository
• Remote Repository merupakan repository server yang akan
digunakan untuk menyimpan setiap perubahan pada local repository,
sehingga dapat diakses oleh banyak user.
• Untuk menambahkan remote repository server, gunakan perintah
git remote add origin [url]
  $ git remote add origin link repository saya

10. Push (Mengirim perubahan ke server)
• Untuk mengirim perubahan pada local repository ke server gunakan
perintah git push.
  $ git push -u origin master
• Perintah ini akan meminta memasukkan username dan password
pada akun github.com

11. Melihat hasilnya pada server repository
• Buka laman github.com,
arahkan pada repositorinya.
• Maka perubahan akan
terlihat pada laman
tersebut.

