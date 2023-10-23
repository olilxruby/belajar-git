# "Hah, Git?!" Git Apaan Tuh?
Gaaassss ~~gak pake rem~~ pake rem dikit, biar aman.
Sebagai System Engineer (bahasa Inggrisnya As an System Engineer, gak penting ya. Xixixixi) yang biasa handle storage dan perangkat-perangkat pendukungnya, jujur merupakan hal yang ngga baru-baru amat juga sih buat gout (gout itu = ogut ya atau saya, gitu.) coba sedikit lebih cari tau apaan sih git itu. Seiring terus berkembang nya dunia IT, ya mau ga mau minimal sedikit tau atau syukur-syukur kedepan jadi tau banyak tentang dunia kode-kodean ( contoh kode yang sering digunain didunia project-an apalagi bagian pengadaan: *boss jangkrik boss, Jiah masih kaku aja*. Ahay!). Itu contoh kode kalo lagi butuh duit banget.

Tapi jujur aja, sampe sekarang gout masih bingung "kenapa bingung dinamain bingung?" Ada yang tau ngga jawabannya kenapa "Bingung" dinamain "Bingung", nah bingung kan! Okeh skip.

[![GitHub stars](https://img.shields.io/github/stars/Naereen/StrapDown.js.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/Naereen/StrapDown.js/stargazers/)
[![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com) [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
[![Visual Studio Code](https://img.shields.io/badge/--007ACC?logo=visual%20studio%20code&logoColor=ffffff)](https://code.visualstudio.com/) [![Docker](https://badgen.net/badge/icon/docker?icon=docker&label)](https://https://docker.com/) [![Discord](https://badgen.net/badge/icon/discord?icon=discord&label)](https://https://discord.com/)

## Git Command line
Gaaassss!!! Berikut perintah atau command yang sering digunakan oleh seorang programmer atau devops ketika menggunakan git:
- git init
- git add
- git commit
- git log
- git diff
- git branch
- git checkout
- git merge
- git remote
- git push
- git pull
- .gitignore

## Sebelum dimulai

Untuk mulai mencari tau apa itu VCS atau ~~Video Call Seseorang~~ padahal maksudnya S-nya itu hhhmmm?
Okeh fokus fokus, VCS atau Version Control System atau yang lebih familiar di internet disebut dengan Git adalah suatu instrument buat.. okeh coba gugling sendiri ya!! Eehh ngga deng becyaandaa.

Disclaimer first, pengertian VCS yang ogut tulis juga hasil dari gugling. Xixixi *bapack-bapack mode-on.
Jadi, Version control adalah sebuah sistem yang merekam perubahan-perubahan pada sebuah file atau sekumpulan file dari waktu ke waktu sehingga pengguna dapat mengingat versi tertentu nantinya. Version control system juga dikenal sebagai revision control (kontrol revisi) atau source control (kontrol sumber). Version control sangat penting untuk membantu tim software engineering mengelola perubahan kode sumber (source code) dengan efisien dan mengurangi risiko kesalahan atau konflik. Singkatnya dengan menguunakan vcs atau git seseorang bisa mencatat apa saja perubahan atau penambahan file yang akan atau telah di kerjakan. Untuk memulai menggunakan git, cukup install 2 aplikasi dibawah ini.

- [Git Apps](https://git-scm.com/downloads) - Wajib di install!!
- [VScode](https://code.visualstudio.com/download) - Text editor yang paling oks buat gout!
- [PC x Laptop]() - Kalo ga punya pc atau leptop mau install dimanaaa!!

## Installasi
Install  [Git](https://git-scm.com/downloads) untuk menjalankan command atau perintah yang ada pada git itu sendiri.
Untuk pengguna System Operasi (OS) Linux, beberapa distro sudah menyediakan git apps tanpa harus menginstall-nya lagi. Pada tulisan tentang git, ogut menggunakan Windows Subsystem Linux 2 atau disingkat WSL 2 dengan OS Ubuntu 22.04.

Untuk pengguna Windows pastikan download installer git di website git nya ya. untuk link nya suda gout lampirin tuh di atas. Tinggal klik aje.
#### Install git di Windows
```sh
Klik installer nya, terus next next next next. selesai
Open git bash kalau udah selesai di install
```

#### Install git di Linux

```sh
sudo apt update && sudo apt upgrade
sudo apt install git -y
```
Cek dengan mengetik git pada terminal linux temen-temen. kalau output nya seperti gambar dibawah ini itu tandanya git udah berhasil di kepasang di OS Linux temen-temen.
![Alt text](https://i.imgur.com/66lr0Hg.png "install git di linux")

#### Install VSCode
```sh
Klik installernya kalau sudah di download. Trus klik next next next. Selesai
Open vscode. Next, gaaassss pake rem dikit biar ga nabrak.
```

Tampilan VSCode di Windows
![Alt text](https://i.imgur.com/SjADR6v.png "vscode windows")

#### Extensions VSCode
![Alt text](https://i.imgur.com/uUIZtqF.png "plugins windows")

## Mari Mulai!

Big thanks! yang udah mau baca sama step ini.
Yuk mulai.
Bismillah, semoga Allah SWT memudahkan segala apapun ilmu yang baik-baik yang kita pelajarin. Aamiin.

Sebelum menggunakan git, diharuskan untuk melakukan setting konfigurasi seperti dibawah ini.
Ketikan command dibawah ini pada teriminal:

```sh
git config --global user.name "nama-user"
git config --global user.email nama-email
contoh:
git config --global user.name "nasiuduk"
git config --global user.email xxxxx@outlok.com
git config --list
```
![Alt text](https://user-images.githubusercontent.com/90337960/277147136-74962689-1ec5-4474-9db9-082e63f5820c.png "plugins windows")
output git
![Alt text](https://i.imgur.com/xbDtVzW.png "output git")
gunanya agar saat mau melakukan ``git add`` dan ``git commit`` ga ada pesan eror yang muncul.

#### Command atau Perintah yang sering digunakan di git
- #### git init
``Git init`` digunakan saat ingin menginisialisai direktori yang akan di gunakan untuk bekerja dengan git. Saat membuat folder atau direktori di Windows ataupun Linux, folder atau direktori tersebut akan di inisialisasi dengan perintah git init. Seperti yang saya bilang di awal, temen-temen juga bisa menggunakan Windows yang sudah terinstall git (git bash).

contoh pada Linux
create direktori:

```sh
mkdir belajar-git
```
![Alt text](https://i.imgur.com/U8C9xnw.png "output git")

Direktori tersebut akan di ``init`` dengan menggunakan perintah ``git init``. Setelah direktori dibuat, masuk kedalam direktori tersebut dengan menggunakan perintah ``cd belajar-git`` lalu ketikan command ``git init`` di dalam direktori belajar-git untuk melakukan inisialisasi pada direktori yang akan di gunakan. Se lanjunya perintah ``git add``, ``commit`` dst bisa di jalankan

```sh
cd belajar-git
git init
```
![Alt text](https://i.imgur.com/ib4VP7Y.png "output git")

Sampai Langkah ini, command ``git add``, ``git commit`` dan yang lainnya sudah bisa di gunakan dengan beberapa catatan yang akan dibahas lebih lanjut.

*Note: sebuah folder atau direktori tidak akan bisa dijalankan dengan perintah ``git add``, ``commit`` dst sebelum folder atau direktori tersebut di init `` git init``. Selanjutnya akan dibahas command atau perintah ``git add``.*

- #### git add

``Git add`` digunakan saat membuat file baru atau pun memodifikasi file yang berada pada direktori yang sudah di ``init``. Jika ada file baru (.js, .html, .log ataupun yang lain) pada direktori yang sudah di inisialisasi (direktori belajar-git). Selanjutnya ketikan command atau perintah ``git add`` pada file yang baru di tulis atau file yang sudah dimodifikasi.
Gunanya agar file tersebut bisa di ``commit``. Jika file tersebut sebelumnya belum di ``git add``, maka file tersebut tidak bisa di ``commit`` sebelum di add menggunakan ``git add``. Akan di contohkan bagaimana fungsi ``git add``.

Pada contoh ini, akan di contohkan dengan menggunakan tools vscode dan wsl2-ubuntu untuk masuk ke direktori yang sudah di ``init``, lalu buat file baru pada direktori yang sudah di ``init`` pada terminal OS teman-teman (jika menggunakan Windows, teman-teman bisa menjalankan git bash ya).
![Alt text](https://i.imgur.com/VkGM0za.png "output git")

Lalu ketikan command ``git add <nama-file>`` yang ingin di add
contoh:
```sh
git add contoh.js
```

*note: jika ada lebih dari 1 file yang ingin di add, bisa menggunakan command ``git add –all atau git add -A``. dan untuk mengecek status dari file yang telah di add teman-teman bisa mengetikan*

```sh
git status
```
![Alt text](https://i.imgur.com/X4XYWuJ.png "output git")

- #### git commit

``Git commit`` digunakan untuk melakukan commit atau jika ada setiap penambahan file atau modifikasi file. ``Git commit`` bisa berjalan jika sebelumnya file yang dimodifikasi atau file yang ditambahkan sudah terlebih dahulu di ``add`` menggunakan perintah ``git add <nama-file>``. Untuk lebih jelasnya seperti berikut

```sh
git commit -m "Commit contoh.js step 1"
```

(option -m bisa di artikan message atau pesan atau catatan untuk file yang di tambahkan atau di modifikasi)
![Alt text](https://i.imgur.com/iCqI5rx.png "output git")

jika output dari ``git status`` seperti pada gambar di atas setelah melakukan ``commit`` pada file, artinya sudah tidak ada lagi file yang akan di ``commit``.

- #### git log

Untuk melihat log pada git, ketikan perintah atau command
```sh
git log
```
output pada ``git log`` adalah output saat proses ``commit`` pada file sudah dilakukan, berikut contoh output ``git log``.
![Alt text](https://i.imgur.com/uBR1Ody.png "output git")

- #### .gitignore

``.gitignore`` digunakan jika ada beberapa file yang ingin di abaikan atau tidak di ``commit``. Untuk menjalankan ``.gitignore`` caranya adalah dengan mendefinisikan file yang ada di dalam folder ataupun file diluar folder dengan ekstensi tertentu kedalam file config ``.gitignore`` itu sendiri. Berikut contoh untuk menggunakan ``.gitignore``

create .gitignore file terlebih dahulu
```sh
touch .gitignore  // untuk membuat file, jika menggunakan vscode bisa langsung dari vscode
vi .gitignore     // Untuk menambahkann file yang ingin di ignore atau di abaikan
```
![Alt text](https://i.imgur.com/TdGkEB0.png "output git")
gambar diatas adalah sebelum mendefinisikan file dengan ekstensi .log dan .txt yang ada di dalam folder templates. Selanjutnya jika sudah ada file yang sudah di definisikan di dalam ``.gitignore``, status pada ``git status`` akan seperti gambar dibawah ini
![Alt text](https://i.imgur.com/OiMAAEu.png "output git")
``Git status`` di atas menginformasikan bahwa ``.gitignore`` telah di modified atau di modifikasi. Karena untuk mengabaikan .log dan semua file yang ada di direktori templates diharuskan memodifikasi file ``.gitignore``. Selanjutnya ``.gitignore`` akan di ``commit``.
![Alt text](https://i.imgur.com/pUwVx6b.png "output git")

- #### git diff

``Git diff`` digunakan untuk melihat jika ada 1 atau 2 file yang dimodifikasi. Dengan menggunakan ``git diff``, file sebelum dan sesudah di modifikasi akan bisa dilihat. Berikut contoh dari ``git diff``

Ketikan perintah
```sh
git diff
```
![Alt text](https://i.imgur.com/syAixVX.png "output git")

- #### git branch, git checkout, git merge

``Git branch`` digunakan jika melakukan kolaborasi yang di kerjakan lebih dari 1 orang. Untuk menggunakan ``git branch`` adalah sebagai berikut.

Ketikan perintah atau command pada terminal
``git branch <nama-branch>``
Lalu lihat status branch dengan mengetikan command
``git branch``
Untuk mengaktifkan branch master ke branch yang baru saja dibuat adalah menggunakan perintah
``git checkout <nama-branch>``

Contoh:
```sh
git branch login-page       // login-page adalah nama dari branch baru yang dibuat
git branch                  // untuk melihat total branch yang sudah diibuat
git checkout login-page     // untuk berganti branch
```
![Alt text](https://i.imgur.com/RO92yqs.png "output git")

Bisa dilihat pada gambar di atas, membuat branch baru dengan perintah ``git branch nama-branch``.
Cek nama branch dengan perintah ``git branch`` Lalu mengaktifkan branch yang baru saja dibuat dengan dengan mengetikan ``git checkout nama-branch``

Setelah ``branch`` sudah bukan dimaster lagi, selanjutnya buat 1 file yang nantinya akan di ``merge`` kedalam branch master dengan menggunkan perintah ``git merge nama-file``. Dengan catatan status ``branch master`` aktif.
Berikut contoh pada gambar dibawah ini:

```sh
touch templates/index.html    // membuat file di folder templates dgn nama index.html
git add -all                  // add new file
git status                    // check status file
git commit -m "Commit index.html di branch login-page"     // commit file

```
![Alt text](https://i.imgur.com/B87ZYml.png "output git")

Keterangan pada gambar di atas adalah, ``login-page`` sebagai ``branch`` yang aktif dengan membuat sebuah folder yang berisi file ``index.html``. Dimana folder dan file tersebut akan hilang dari direktori ``branch maste``r saat melakukan switching ke ``branch login-page``. Agar folder dan file yang ada didalamnya bisa terlihat pada directory ``branch master``, dibutuhkan command atau perintah ``git merge``.

Gambar dibawah ini adalah ketika melakukan switch dari ``branch login-page`` ke ``branch master``.
Bisa di lihat bahwa ``folder html`` dan juga ``file index.html`` yang ada di dalamnya hilang. Ini disebabkan karena folder yang ada di ``branch login-page`` belum di merge ke ``branch master``

```sh
git checkout master    // switch atau ubah branch master menjadi aktif branch
git branch             // check apa branch master sudah aktif yang di tandai dengan sysmbol *
```
![Alt text](https://i.imgur.com/h7vtgrV.png "output git")

Berikut adalah contoh untuk melakukan merge pada branch login-page ke branch master. Pastikan branch master dalam mode on. Atau jika kita ketikan command ~git branch akan muncul output master dikuti dengan sysmbol *.

Ketikan command:
``git merge nama-branch``

Contoh:

```sh
git checkout master     // switch branch menjadi branch master
git branch              // check branch 
git merge login-page    // merge file yang di tambahkan di branch login-page ke branch master
```
![Alt text](https://i.imgur.com/wIIGrYO.png "output git")
Setelah dilakukan ``merge`` dengan ``branch login-page``, folder html beserta isi file di dalamnya sudah muncul saat ``branch maste``r dalam posisi aktif.

- #### git remote, git push, git pull

``Git remote`` digunakan untuk membuat repositori di ``github``. Untuk masuk atau login ke ``github``, diharuskan teman-teman membuat akun di ``github``. Jika teman-teman sudah mempunyai akun ``github``, selanjutnya teman-teman bisa langsung membuat repository di ``github``. Setelah itu teman-teman akan diberikan sebuah link untuk mengakses repository menggunakan command atau perintah ``git remote <nama-repository> <link-repository-github>``. Setelah login, buat repository baru sesuai keinginan. Dalam contoh ini akan di buat nama remote repository ``remote-belajar-git``
![Alt text](https://i.imgur.com/oqxllYs.png "output git")

Klik new repository seperti pada gambar. Lalu buat sebuah repository dengan nama remote-belajar-git. Setelah selesai klik create repository.
![Alt text](https://i.imgur.com/SS9sbMu.png "output git")
![Alt text](https://i.imgur.com/6bHn6ry.png "output git")

Setelah klik repository, akan muncul tampilan seperti berikut. Yang artinya adalah repository sudah berhasil dibuat. Tapi belum ada file ataupun folder yang ditulis dalam repository tersebut. Langkah selanjutnya adalah mengcopy link dari remote repo, untuk di input pada local repo yang selanjutnya menggunakan ``git push`` atau ``git pull``.
![Alt text](https://i.imgur.com/n0Zf1fB.png "output git")

Pada tahap ini, akan dijelaskan bagaimana cara mengunakan ``git remote`` ``git push`` dan ``git pull``.
Masuk kedalam direktori ``belajar-git`` yang sudah di ``init``. Check isi dalam folder tersebut apakah sudah ada file atau belum. Dalam contoh ini sudah ada beberapa file .js dan .html dan lainnya, juga ada beberapa folder yang telah dibuat sebelumnya.
![Alt text](https://i.imgur.com/l0JhYGF.png "output git")

Setelah itu masukan link dari repository yang telah dibuat di github.
```sh
git remote add origin https://github.com/<nama-akun-github>/<nama-remote-repo>.git
```
![Alt text](https://i.imgur.com/tW18Y1T.png "output git")

Langkah selanjutnya gunakan command
``git push nama-branch``, yang ingin di ``push`` atau di upload ke ``github``. Pastikan sebelum di ``push`` sudah tidak ada file atau folder yang belum di ``commit``. Setelah melakukan ``git push`` pada local computer, akan di informasikan jika file yang ada di ``branch master`` sudah berada di ``github``
```sh
git status                // check apakah ada file yang belum di add atau di commit
git push origin master    // push folder dan file dari local repo ke remote repo
```
![Alt text](https://i.imgur.com/RGBSweY.png "output git")

Akan muncul tampilan seperti gambar dibwah ini pada akun github ketika file yang ada di branch master sudah di push
![Alt text](https://i.imgur.com/sOMokHI.png "output git")

Jika sudah seperti tampilan di atas, artinya file yang ada di local repository sudah berada di akun ``github``. File atau folder yang berada di akun ``github`` bisa di edit atau di modifikasi, ketika melakukan modifikasi file di akun ``github``, jangan lupa melakukan ``commit`` seperti halnya saat melakukan modifikasi file di local repository. Setelah file telah di modifikasi dan ``commit`` pada akun ``github``, dan jika pengguna ingin file yang telah di modifikasi tersebut juga terupdate di local repository. Caranya adalah dengan menggunakan command atau perintah ``git pull`` pada local repository.
Berikut contohnya.
![Alt text](https://i.imgur.com/H7TTeIY.png "output git")

Sebelum menggunakn ``git pull``
![Alt text](https://i.imgur.com/6smbfT7.png "output git")

Setelah menggunakan ``git pull``. Terlihat file index.html di local repository pada text editor yang di lingkari otomatis berubah atau sama dengan file index.html yang ada pada akun ``github``.
```sh
git pull origin master // menarik perubahan file yang di tulis di remote repo pada branch master
```
![Alt text](https://i.imgur.com/ZFeMdHw.png "output git")

Selanjutnya teman-teman akan memodifikasi file index.html yang ada di local repository agar ketika menggunakan command atau perintah ``git push`` file tersebut juga terupdate otomatis pada repository ``github``
```sh
untuk lebih jelasnya lihat urutan penomeran pada gambar dibawah
```
![Alt text](https://i.imgur.com/yb6pwDJ.png "output git")

Gambar dibawah ada tampilan saat ``local repo`` sudah terupdate di ``remote repo``
![Alt text](https://i.imgur.com/ErZOSSx.png "output git")

Selanjutnya teman-teman akan menambahkan branch pada ``remote git``. Berikut Langkah-langkahnya. Pastikan teman-teman memiliki ``branch`` selain ``branch master``. Pada contoh ini teman-teman akan menggunaka ``branch`` yang sudah ada, dan teman-teman juga akan menggunakan ``branch`` yang baru. Pada contoh gambar dibawah, teman-teman menggunakn ``branch`` yang sudah ada, yaitu ``branch login-page``. Untuk cara bagaimana membuat ``branch`` baru akan dijelaskan lagi pada bagian ini.
Ketikan command atau perintah:
```sh
git checkout login-page
```
![Alt text](https://i.imgur.com/vntyLY6.png "output git")

Setelah sudah masuk dengan ``branch login page``, ``push branch`` terebut kedalam ``remote git hub``. Caranya sebagai berikut:
List ``branch`` sebelum menambahkan branch yang ada pada ``local repo``
![Alt text](https://i.imgur.com/8oLQuRk.png "output git")
![Alt text](https://i.imgur.com/5mfL4Yj.png "output git")

Membuat branch baru untuk di push di github. Untuk membuat branch baru bisa juga menggunakan command atau perintah ``git branch <nama-branch>``. Pada contoh ini menggunakan command atau perintah ``git checkout -b <nama-branch>`` (option -b pada git checkout adalah shortcut yang juga bisa digunakan membuat branch baru dan langsung mengaktifkan branch tersebut seperti contoh pada gamabr dibawah ini).
```sh
git checkout -b logout-page
```
![Alt text](https://i.imgur.com/MNvDIVz.png "output git")

Setelah membuat ``branch`` terbaru dengan menggunakan command atau perintah git ``checkout -b <nama-branch>``, teman-teman bisa langsung ``push branch`` tersebut ke ``github``.
```sh
git push origin logout-page    // push branch logout-page ke remote repo github
```
![Alt text](https://i.imgur.com/o7uVaiA.png "output git")

Setalah itu refresh browser ``github`` teman-teman untuk mengupdate ``branch`` yang baru saja di ``push``. pada gambar dibawah ini terlihat ada 3 ``branch`` yang sebelumnya hanya ada ``branch master`` dan branch ``login-page``. Setelah membuat branch baru pada local repo dan melakukan ``push branch`` baru, pada tampilan github akan bertambah branch yang baru dibuat. Yaitu ``branch logout-page``.
![Alt text](https://i.imgur.com/EaO0N31.png "output git")

*Note: jika pengguna menambahkan file pada branch A, lalu pengguna belum melakukan git add dan git commit pada branch tersebut, lalu pengguna melakukan switch ke branch B, setelah switch pengguna melakukan git add dan git commit file yang ditulis di branch A melalui branch B, maka file tersebut akan menjadi bagian branch B. Kesimpulannya, jika pengguna melakukan commit suatu file yang mana file tersebut ditulis di branch sebelumnya, maka file tersebut akan menjadi milik branch yang saat ini aktif.*


## Mari Kita Tutup Sementara

Alhamdulillah, mohon di maafkan apabila tulisan ini tidak sesuai ekspektasi teman-teman yang membacanya. Tulisan ini mungkinn bisa dibilang dasar dari pengoperasian git. InsyaAllah untuk lanjutan dari tulisan ini terkait fungsi atau command lanjutan dari git akan saya tulis kembali. Seperti contoh command ``git clone``, melakukan git clone pada repository public dengan memfilter branch apa aja yang  mau di pull ke local repo, dll.

Akhir kata, Semoga Allah SWT mudahkan bagi para pencari Ilmu. Aamiin Allahumma Aamiin.

Gasss!!!
