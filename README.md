
### git *dasar* :writing_hand:

| **Command** | **Description** |
| --- | --- |
| `git init` | Membuat repository  |
| `git status` | Daftar semua file baru atau yang dimodifikasi |
| `git add <nama_file>` | Memindahkan 1 file ke staging index |
| `git add .` | Memindahkan beberapa file ke staging index |
| `git  commit -m "isi commit" ` | Menambah commit |
| `git  clean -f` |  Membatalkan penambahan file di Working directory  atau menghapus file tersebut |
| `git restore <nama_file>` | Membatalkan perubahan/penghapusan file di Working directory |
| `git restore --staged <nama_file>` | Mengembalikan posisi Staging Index ke Working directory |
| `git log` | Melihat semua riwayat commit |
| `git log --oneline` | Melihat commit log message sederhana |
| `git log --oneline --graph` | Melihat commit log dengan commit sebelumnya/ yang lain |
| `git show hash` | Melihat detail perubahan yang terjadi apada sebuah commit |
| `git diff <hash1> <hash2>` | Membandingkan hasil antar commit  |
| `git difftool <hash1> <hash2>` | Membandingkan hasil antar commit menggunakan vscode |
| `git reset --soft <hash>` | Memindahkan HEAD pointer, namun tidak melakukan perubahan apapun di Staging Index dan Working directory |
| `git reset --mixed <hash>` | Memindahkan HEAD pointer, mengubah Staging Index menjadi sama seperti dengan Repository . Namun tidak mengubah apapun di Working directory |
| `git reset --hard <hash>` | Memindahkan HEAD pointer dan mengubah Staging Index dan Working directory sehingga sama dengan repository|
| `git commit --amend` | Menambah beberapa baris kode tanpa melakukan reset |
| `git checkout <hash> <nama_file>` | Melihat versi file pada commit sebelumnya. Dan file tersebut akan berada di staging index |
| `git checkout <hash>` | Menuju ke snapshot tertentu |
| `git revert <hash>` | Membatalkan commit yang sudah di buat |
| `git blame <nama_file>` | Mencari tahu siapa yang menambahkan perubahan pada file tersebut dan juga mengetahui commitnya |


### git *branch* :writing_hand:

| **Command** | **Description** |
| --- | --- |
| `git branch --show-current` | Melihat nama branch saat ini |
| `git branch` atau  `git branch --list` | Melihat semua branch |
| `git branch <nama_branch_baru>` | Membuat branch |
| `git checkout <nama_branch>` atau  `git swith <nama_branch>`| Pindah ke branch lain |
| `git branch -m <nama_branch_baru>` | Mengubah nama branch |
| `git branch -d <nama_branch>` atau `git branch -delete <nama_branch>` | Menghapus branch|
| `git merge` | Melakukan penggabungan dua buah branch |
| `git merge --abort` | Membatalkan merge |
| `git cherry-pick <commitId>` | Melakukan merge sebagian artinya mengambil commit dari branch lain dan melakukan penggabungan ke dalam branch saat ini |
| `git tag <example 1.0.0> <commit Id>` | Menandai sebuah commit id |
| `git tag -l` atau `git tag -list`| Menampilkan semua tag |
| `git checkout <tagName>` | Melihat snapshot sebelumnya |
| `git tag -d <tagName>` atau `git tag -d <tagName>`  | Menghapus tag |
| `git stash push -m "message stash"` | Untuk menyimpan perubahan di Working directory atau Staging Index secara sementara agar branch saat inimenjadi bersih kembali |
| `git stash list` | Melihat semua stash |
| `git stash show <stashId>` | Melihat perubahan yang terjadi di stash|
| `git stash apply <stashId.` | Mengambil perubahan di stash |
| `git stash drop <stashId>` | Menghapus stash |
| `git stash clear` | Menghapus semua stash |


### git *remote* :writing_hand:

| **Command** | **Description** |
| --- | --- |
| `git remote add <name> <ssh-url>` | Menambah remote repository |
| `git remote` | Melihat remote repository |
| `git remoteget -url <name>` | Melihat URL detail remote repository |
| `git remote rm <name>` | Menghapus remote repository |
| `git push <name_remote> <local_branch>` | Mengirim perubahan branch ke remote repository dengan nama branch yang sama |
| `git push <name_remote> <local_branch>:<remote_branch>` | Mengirim perubahan branch ke remote repository dengan nama branch yang berbeda |
| `git push origin --all` | Mengirim semua perubahan di semua branch ke remote repository |
| `git push --delete <name_remote> <name_repository>` | Menghapus branch yang ada di remote directory |
| `git clone <url_remote_repository>` | Download project di remote repository ke local |
| `git branch -r` | Melihat semua daftar branch yang ada remote repository |
| `git branch -a` | Melihat semua daftar branch yang ada remote repository dan local |
| `git checkout -b <local_branch> <remote_name>/<remote_branch>` | Membuat branch dari remote branch |
| `git fetch <remote_name>` | Mendapatkan perubahan terakhir dari remote repository dan tidak mengubah isi local git |
| `git fetch <remote_name> <remote_branch>` | Melakukan fetch untuk branch tertentu di remote |
| `git pull <remote_name> <remote_name_branch>` | Mendapatkan perubahan terakhir dari remote repository dan disimpan di local repository |
| `git push <remote_name> <tagName>` | Mengirim tag ke remote repository |
| `git push <remote_name> --tags` | Mengirim semua tag ke remote repository |
| `git fetch <remote_name> <tagName>` | Mengambil tag |
| `git fetch <name_remote>` | Mengambil semua tag |
| `git push --delete <remote_name> <tagName>` | Menghapus tag |
