## command-git.txt

#### <details><summary>Perintah dasar git<summary><detail>
- Mengecek file
 `git status`
 
- Memindahkan 1 file ke staging index
 `git add <nama_file>`

- Memindahkan beberapa file ke staging index
 ` git add .`
 
- Menambah commit
 `git commit -m "isi commit" `
 
- Membatalkan penambahan file di Working directory
 ` git clean -f`
 atau menghapus file tersebut
 
- Membatalkan perubahan/penghapusan file di Working directory
 ` git restore <nama_file>`
 
- Mengembalikan posisi Staging Index ke Working directory
 ` git restore --staged <nama_file>`
