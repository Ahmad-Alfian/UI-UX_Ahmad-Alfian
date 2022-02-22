
Version Control and Branch Management SECTION 2

Single User (Lokal hanya bisa diakses oleh 1 orang)
Centralized (Bisa diakses oleh beberapa orang cuman jika server mati tidak bisa diakses)
Distributed (diakses oleh banyak orang/team dan jika servers mati maka masih bisa digunakan via lokal nanti jika server sudah normal bisa dipush kembali ke server)

gitignore (node)
gitignore berisi log, dan berfungsi untuk memfilter mana saja yang boleh/tidak boleh dimasukkan ke repository 

Cara Setting git bash
git config --global user.name "Ahmad Alfian"
git config --global user.email "email"
git config --list

Start Clone 
git clone "http ssh"
cd my-project

Cara memasukkan working directory 
ke staging area :
New terminal -> ketik "git add ." (Memasukan Semua Perubahan)
"git add <directory>"
"git add hello.py"
"git add ."
ke repository git :
New terminal -> ketik "git commit -m "inisialisasi index.html"" (Warping dahulu)
"inisisalisasi" pesan entah itu info ada bug atau perbaikan pada file ketika commit
Lanjut terminal -> ketik "git push origin"

"git diff" Mengetahui perubahan pada code:
New terminal-> ketik "git diff"
Maka akan keluar warna pada kode: 
warna putih : kode awal/kode asli
warna merah : kode asli tapi masih kosong
warna hijau : tambahan/perubahan pada kode

"git stash" menyimpan perubahan atau update
stash : menyimpan perubahan
pop stash : memunculkan perubahan
drop stash : menghapus perubahan
apply stash : memasukkan
pop latest stash : terakhir

Git log, check out.
git log -- (untuk membuka log selama proses)
git checkout paste nomor (untuk mengembalikan proses)

git reset paste nomor --soft atau --hard
Kalau --soft itu perubahan tidak sebanyak hard.
Kalau --hard itu perubahan yang sangat besar dapat merusak commit yang telah dibuat.

git pull origin main (untuk mengembalikan repo dari git ke lokal, biasanya dikarenakan lokal ada bug) untuk "main" itu hanya nama bagiannya

git branch --list (untuk check bagian-bagiannya)
git branch nama branch (untuk menambahkan branch pada lokal)
git push -u origin nama branch (untuk upload branch terbaru dari lokal ke git)
