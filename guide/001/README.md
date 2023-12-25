
## Sejarah Git

Pada pengembangan kernel linux 1991-2002 developer komunitas nya mengupdate patch menggunakan tools Distributed version control system: **Bitkeeper**.

Namun pada 2005 hubungan komunitas dengan perusahaan bitkeeper terputus, Sehingga **linux torvalds(pembuat linux)** dan komunitas linux berencana mengembangkan software yang hampir sama dengan bitkeeper namun dengan beberapa fitur tambahan untuk mendevelop kernel linux, dan lahirlah GIT.


## Apa itu Git?

Git adalah **Version Control System** berbasis command line interface / CLI, yang di peruntukan khusus untuk menghandle source code.


## Apa sih Version Control System itu ?

**Version Control System** Adalah system yang merekam perubahan perubahan/**snapshot** dari sebuah berkas dari waktu ke waktu, sehingga kita dapat menarik kembali ke versi khusus suatu saat nanti (**rollback**)

**Contoh implementasi version control system :**
- Google Docs
- Git
- Mercurial
- etc…

## Jenis Version Control System

- Local version control system: Berjalan hanya di local computer, semua perubahan ada pada local computer kita.
- Centralized version control system: Setiap perubahan di simpan di sisi server, client akan request versi spesifik ke server. Contohnya adalah subversion
- Distributed Version control system: Improvement dari contralized version control system, Client akan request ke server dengan full version, server bisa lebih dari satu dengan riwayat versi yang sama. Contohnya adalah git, mercurial, etc…

## Perbedaan dengan Github

- Git software based command line interface
- Github cloud repo hosting service, di dalam systemnya terinstall git

**Contoh cloud repo hosting :**
- AWS Code Commit
- GitHub
- BitBucket
- GitLab

## Git Repository

**Repository** adalah project/workspace tempat source code kita yang sudah di initialized project git.

Untuk meng-initialized project git bisa menggunakan perintah:

`git init`

## Git branch

**Branch** adalah cabang bebas yang di gunakan untuk pointer pada perubahan file kita(commit)

Saat membuat commit pertama kali, maka akan di berikan 1 branch default.
Biasanya bernama **main(github)** / **master(git)**

Membuat branch bisa menggunakan perintah :

`git branch <nama_branch>`

## Git index

**Staging Index** adalah tempat untuk memindahkan file kita ke snapshot / commit 
Sebelum file di commit wajib di pindahkan ke staging index terlebih dahulu

Untuk memindahkan file ke staging index kita bisa menggunakan perintah:

`git add <nama_file/working_dir>`

## Git commit

**Commit** adalah snapshot / riwayat perubahan file kita
Dalam commit menggunakan hash(unique random string) untuk identifiernya

Untuk melakukan commit kita menggunakan perintah:

`git commit -m “message commit”`