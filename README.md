Belajar version control system atau yang biasa dikenal dengan git.
sebelum menggunakan git, diharuskan untuk melakukan setting konfigurasi seperti dibawah ini.
Ketikan command dibawah ini pada teriminal:

git config --global user.name "nama-user"
git config --global user.email nama-email
Setelah itu, cek dengan mengetikan perintah:

~ git config --list

![image](https://github.com/olilxruby/ujian-git/assets/90337960/74962689-1ec5-4474-9db9-082e63f5820c)

 
Pada perintah pada gambar di atas, akan keluar output seperti pada gambar

![image](https://github.com/olilxruby/ujian-git/assets/90337960/3ab019b7-0b63-462a-b841-de0d6d7e58e9)

 
gunanya agar saat mau melakukan "git add dan git commit" tidak ada pesan eror yang muncul.

Berikut adalah beberapa git command yang sering digunakan.

git init
   
git init digunakan saat ingin menginisialisai direktori yang akan di gunakan untuk bekerja dengan git.
Saat membuat folder atau direktori di windows ataupun Linux, folder atau direktori tersebut akan di inisialisasi dengan perintah git init.
Teman-teman juga bisa menggunakan windows yang sudah terinstall git (git bash)

contoh pada Linux
create direktori:

~ mkdir belajar-git

![image](https://github.com/olilxruby/ujian-git/assets/90337960/37716b1c-4a96-42f4-a1c2-3399a2179eb9)

 
Direktori tersebut akan di init dengan menggunakan perintah ~git init.
Setelah direktori dibuat, masuk kedalam direktori tersebut dengan menggunakan perintah

~cd belajar-git
lalu ketikan command ~git init di dalam direktori belajar-git untuk melakukan inisialisasi pada direktori yang akan di gunakan.
Selanjunya perintah git add, commit dst bisa di jalankan.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/fcd4734a-dcf1-425e-af78-e5902953820c)
 
Sampai Langkah ini, command git add, git commit dan yang lainnya sudah bisa di gunakan dengan beberapa catatan yang akan dibahas lebih lanjut.
Note: sebuah folder atau direktori tidak akan bisa dijalankan dengan perintah git add, commit dst sebelum folder atau direktori tersebut di init (~ git init).
Selanjutnya akan dibahas command atau perintah git add.

git add
   
git add digunakan saat membuat file baru atau pun memodifikasi file yang berada pada direktori yang sudah di init. Jika ada file baru (.js, .html, .log ataupun yang lain)
pada direktori yang sudah di inisialisasi (direktori belajar-git).
Selanjutnya ketikan command atau perintah git add pada file yang baru di tulis atau file yang sudah dimodifikasi. Gunanya agar file tersebut bisa di commit.
Jika file tersebut sebelumnya belum di ~git add, maka file tersebut tidak bisa di commit sebelum di add menggunakan git add.
Akan di contohkan bagaimana fungsi git add. Pada contoh ini, akan di contohkan dengan menggunaka tools vscode dan wsl2-ubuntu
Masuk ke direktori yang sudah di init, lalu buat file baru pada direktori yang sudah di init pada terminal OS teman-teman (jika menggunakan Windows, teman-teman bisa menjalankan git bash).

![il49samKRH](https://github.com/olilxruby/ujian-git/assets/90337960/c9124ca3-a8e8-4be7-825c-44574b4c0684)

Lalu ketikan command ~ git add (nama file yang ingin di add)
contoh:

~ git add contoh.js (contoh.js adalah nama file)

note: jika ada lebih dari 1 file yang ingin di add, bisa menggunakan command ~git add –all atau git add -A.
dan untuk mengecek status dari file yang telah di add teman-teman bisa mengetikan

~ git status

![bcG4nO2V4S](https://github.com/olilxruby/ujian-git/assets/90337960/a8a65078-0947-4e7f-b787-a070aa65d525)

git commit
   
Git commit digunakan untuk melakukan commit atau jika ada setiap penambahan file atau modifikasi file.
Git commit bisa berjalan jika sebelumnya file yang dimodifikasi atau file yang ditambahkan sudah terlebih dahulu di add menggunakan perintah ~git add nama-file.
Untuk lebih jelasnya seperti berikut

~ git commit -m "Commit contoh.js step 1"

(option -m bisa di artikan message atau pesan atau catatan untuk file yang di tambahkan atau di modifikasi)

![m9496RNgaP](https://github.com/olilxruby/ujian-git/assets/90337960/b4445609-ef3a-4d9b-a7f6-8ee61e34ef61)

jika output dari git status seperti pada gambar di atas setelah melakukan commit pada file, artinya sudah tidak ada lagi file yang akan di commit.

git log
   
Untuk melihat log pada git, ketikan perintah atau command

~git log

output pada git log adalah output saat proses commit pada file sudah dilakukan, berikut contoh output git log.

![4wyN6UFth5](https://github.com/olilxruby/ujian-git/assets/90337960/1531f63a-d36b-437c-b0d1-07386fbaf018)

.gitignore
   
.gitignore digunakan jika ada beberapa file yang ingin di abaikan atau tidak di commit.
Untuk menjalankan .gitignore caranya adalah dengan mendefinisikan file yang ada di dalam folder ataupun file diluar folder dengan ekstensi tertentu kedalam file config .gitignore itu sendiri.
Berikut contoh untuk menggunakan .gitignore

create .gitignore file terlebih dahulu

![WINWORD_uKJWdsHkZP](https://github.com/olilxruby/ujian-git/assets/90337960/29ca5397-ec68-4534-bf58-d42792577a3a)

gambar diatas adalah sebelum mendefinisikan file dengan ekstensi .log dan .txt yang ada di dalam folder templates.
Selanjutnya jika sudah ada file yang sudah di definisikan di dalam .gitignore, status pada git status akan seperti gambar dibawah ini

![th8UTgcFkW](https://github.com/olilxruby/ujian-git/assets/90337960/c69840c9-3e1a-4706-8b46-e3261e658c86)

Git status di atas menginformasikan bahwa .gitignore telah di modified atau di modifikasi.
Karena untuk mengabaikan .log dan semua file yang ada di direktori templates diharuskan memodifikasi file .gitignore. Selanjutnya .gitignore akan di commit.

![geIVuJcpA2](https://github.com/olilxruby/ujian-git/assets/90337960/3d3b5c9f-2744-46db-ae73-98e60f4fdbb6)

git diff
   
Git diff digunakan untuk melihat jika ada 1 atau 2 file yang dimodifikasi. Dengan menggunakan git diff, file sebelum dan sesudah di modifikasi akan bisa dilihat. Berikut contoh dari git diff

![ta3GnZK17b](https://github.com/olilxruby/ujian-git/assets/90337960/ccd9e76e-e2d5-4552-a32a-916613d3ed10)

git branch, git checkout, git merge

Git branch digunakan jika melakukan kolaborasi yang di kerjakan lebih dari 1 orang.
Untuk menggunakan git branch adalah sebagai berikut.
Ketikan perintah atau command pada terminal 

~git branch nama-branch

Lalu lihat status branch dengan mengetikan command

~git branch

Untuk mengaktifkan branch master ke branch yang baru saja dibuat adalah menggunakan perintah

~git checkout nama-branch

![nXvUZUy7EJ](https://github.com/olilxruby/ujian-git/assets/90337960/644c5da3-eb87-4188-89c0-c40471a19bd1)

Bisa dilihat pada gambar di atas, membuat branch baru dengan perintah ~git branch nama-branch.
cek nama branch dengan perintah 

~git branch

Lalu mengaktifkan branch yang baru saja dibuat dengan dengan mengetikan

~git checkout nama-branch

Setelah branch sudah bukan dimaster lagi, selanjutnya buat 1 file yang nantinya akan di merge kedalam branch master dengan menggunkan perintah git merge nama file.
Dengan catatan status branch master aktif. Berikut contohnya.

![AjcHwAeA6F](https://github.com/olilxruby/ujian-git/assets/90337960/77b5a23d-d0cd-4838-8467-3dcf906e7bdb)

Keterangan pada gambar di atas adalah, login-page sebagai branch yang aktif dengan membuat sebuah folder yang berisi file index.html.
Dimana folder dan file tersebut akan hilang dari direktori branch master saat melakukan switching ke branch login-page.
Agar folder dan file yang ada didalamnya bisa terlihat pada directory branch master, dibutuhkan

~git merge.

Gambar dibawah ini adalah Ketika melakukan switch dari branch login-page ke branch master.
Bisa di lihat bahwa folder html dan juga file index.html yang ada di dalamnya hilang.
Ini disebabkan karena folder yang ada di branch login-page belum di merge ke branch master.

![Kpzfju5MAC](https://github.com/olilxruby/ujian-git/assets/90337960/bfb71909-4e56-4a68-8517-fd8b3e0a0a59)

Berikut adalah contoh untuk melakukan merge pada branch login-page ke branch master.
Pastikan branch master dalam mode on. Atau jika kita ketikan command ~git branch akan muncul output master dikuti dengan sysmbol *.
Ketikan command

~git merge nama-branch

Contoh: ~git merge login-page.

![UQRUtMdDJJ](https://github.com/olilxruby/ujian-git/assets/90337960/f7923b6e-fe1a-4d50-96fb-fc2f221f57c2)

Setelah dilakukan merge dengan branch login-page, folder html beserta isi file di dalamnya sudah muncul saat branch master dalam posisi aktif.

git remote, git push, git pull

Git remote digunakan untuk membuat repositori di github. Untuk masuk atau login ke github, diharuskan teman-teman membuat akun di github.
Jika teman-teman sudah mempunyai akun github, selanjutnya teman-teman bisa langsung membuat repository di github.
Setelah itu teman-teman akan diberikan sebuah link untuk mengakses repository menggunakan command atau perintah ~git remote nama-repository link-repository-github.
Setelah login, buat repository baru sesuai keinginan. Dalam contoh ini akan di buat nama remote repository remote-belajar-git

![K4TsEiHHaW](https://github.com/olilxruby/ujian-git/assets/90337960/858309ab-bd62-4020-9b42-a13e7f459411)

Klik new repository seperti pada gambar. Lalu buat sebuah repository dengan nama remote-belajar-git. Setelah selesai klik create repository.

![12EVD3cOfd](https://github.com/olilxruby/ujian-git/assets/90337960/ecfc6dc2-1ed6-42cc-aa03-f002978e7784)

Setelah klik repository, akan muncul tampilan seperti berikut. Yang artinya adalah repository sudah berhasil dibuat.
Tapi belum ada file ataupun folder yang ditulis dalam repository tersebut.
Langkah selanjutnya adalah mengcopy link dari remote repo, untuk di input pada local repo yang selanjutnya untuk digunakan dengan ~git push atau ~git pull. 

![TjjEUOuy2G](https://github.com/olilxruby/ujian-git/assets/90337960/3655ab9d-b342-4275-a007-294ca9c6462c)

Pada tahap ini, akan dijelaskan bagaimana cara mengunakan ~git remote ~git push dan ~git pull.
Masuk kedalam direktori belajar-git yang sudah di init.
Cek isi dalam folder tersebut apakah sudah ada file atau belum. Dalam contoh ini sudah ada beberapa file .js dan .html dan lainnya, juga ada beberapa folder.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/9128c9e8-0bfc-4783-8148-3110dded5094)

Setelah itu masukan link dari repository yang telah dibuat di github.
 
![image](https://github.com/olilxruby/ujian-git/assets/90337960/1e286ac0-db00-41c3-83eb-303de3c072c6)
 
Langkah selanjutnya gunakan command 

~git push nama-branch

yang ingin di push atau di upload ke github.
Pastikan sebelum di push sudah tidak ada file atau folder yang belum di commit.
Setelah melakukan ~git push pada local computer, akan di informasikan jika file yang ada di branch master sudah berada di github

![image](https://github.com/olilxruby/ujian-git/assets/90337960/80db41ba-e3bc-4c58-bff3-3cba88071c0a)

Akan muncul tampilan seperti ini pada akun github ketika file yang ada di branch master sudah di push

![image](https://github.com/olilxruby/ujian-git/assets/90337960/67a50c8f-14d1-43e4-9870-35805a1ffbcf)

Jika sudah seperti tampilan di atas, artinya file yang ada di local repository sudah berada di akun github.
File atau folder yang berada di akun github bisa di edit atau di modifikasi, ketika melakukan modifikasi file di akun github, 
jangan lupa melakukan commit seperti halnya saat melakukan modifikasi file di local repository.
Setelah file telah di modifikasi dan commit pada akun github, dan jika pengguna ingin file yang telah di modifikasi tersebut juga terupdate di local repository.
Caranya adalah dengan menggunakan command atau perintah ~git pull pada local repository. Berikut contoh nya.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/f043bbfb-99de-42fe-bf43-257052542c64)

Sebelum menggunakn ~git pull

![image](https://github.com/olilxruby/ujian-git/assets/90337960/780e5520-8b64-44ad-ac07-7a0e0474efc6)

Setelah menggunakan ~git pull. Terlihat file index.html di local repository pada text editor yang di lingkari otomatis berubah atau sama dengan file index.html yang ada pada akun github.
 
![image](https://github.com/olilxruby/ujian-git/assets/90337960/bd57800a-5664-4b9f-a056-fbf31b438de0)
 
Selanjutnya teman-teman akan memodifikasi file index.html yang ada di local repository agar ketika menggunakan command atau perintah ~git push file tersebut juga terupdate otomatis pada repository github.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/3238503c-61a4-4452-af1f-1bddd3f417c7)

![image](https://github.com/olilxruby/ujian-git/assets/90337960/2fcaabcd-1135-418b-8feb-efdf1af0e3fa)

Selanjutnya teman-teman akan menambahkan branch pada remote git.
Berikut Langkah-langkahnya.
Pastikan teman-teman memiliki branch selain branch master. Pada contoh ini teman-teman akan menggunaka branch yang sudah ada, dan teman-teman juga akan menggunakan branch yang baru. 
Pada contoh gambar dibawah, teman-teman menggunakn branch yang sudah ada, yaitu branch login-page.
Untuk cara bagaimana membuat branch baru akan dijelaskan lagi pada bagian ini.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/7b97e649-b80a-449f-9fea-9476c0f8bbc4)

Setelah sudah masuk dengan branch login page, push branch terebut kedalam remote git hub. Caranya sebagai berikut
List branch sebelum menambahlan branch yang ada pada local repo

![image](https://github.com/olilxruby/ujian-git/assets/90337960/8f0fb082-5154-4e2a-a7bf-db68890f56e9)

![image](https://github.com/olilxruby/ujian-git/assets/90337960/e5ec9b67-62c0-47d9-8721-d2e0aff2cf25)

Membuat branch baru untuk di push di github. Untuk membuat branch baru bisa juga menggunakan command atau perintah
~git branch nama-branch

Pada contoh ini menggunakan command atau perintah

~git checkout -b nama-branch 

(option -b pada git checkout adalah shortcut yang juga bisa digunakan membuat branch baru
dan langsung mengaktifkan branch tersebut seperti contoh pada gamabr dibawah ini).

![image](https://github.com/olilxruby/ujian-git/assets/90337960/6e0e6fb0-aa36-4bfe-8519-2a47ca041547)

Setelah membuat branch terbaru dengan menggunakan command atau perintah git checkout -b nama-branch, teman-teman bisa langsung push branch tersebut ke github pengguna.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/898ba58c-ae3d-4707-8975-3fc2e387aa1f)

 
Setalah itu refresh browser github teman-teman untuk mengupdate branch yang baru saja di push.
pada gambar dibawah ini terlihat ada 3 branch yang sebelumnya hanya ada branch master dan branch login-page.
Setelah membuat branch baru pada local repo dan melakukan push branch baru akan bertambah branch yang baru dibuat. Branch logout-page.

![image](https://github.com/olilxruby/ujian-git/assets/90337960/01e29d11-3ead-484a-b6d0-2b930a1b8bd6)

Note: jika pengguna menambahkan file pada branch A, lalu pengguna belum melakukan git add dan git commit pada branch tersebut, lalu pengguna melakukan switch ke branch B,
setelah switch pengguna melakukan git add dan git commit file yang ditulis di branch A melalui branch B, maka file tersebut akan menjadi bagian branch B.
Kesimpulannya, jika pengguna melakukan commit suatu file yang mana file tersebut ditulis di branch sebelumnya, maka file tersebut akan menjadi milik branch yang saat ini aktif.


