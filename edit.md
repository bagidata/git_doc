## Melihat Perubahan

### Melihat Status
    $ git status
    
### Traking file
#### Melihat traking file
    $ git diff
#### Melihat traking file antara staging dengan file terakhir
    $ git diff --staged
    
### Menambahkan perubahan ke staging atau commit berikutnya
#### Menambahkan semua file dengan dot (.)
    $ git add .
#### Menambahkan file tertentu
    $ git add nama_file.txt
#### Menambahkan file tertentu dengan melihat interaktif perubahan
    $ git add -p nama_file.txt
#### Menambahkan file ekstensesi tertentu
    $ git add *.txt
    
### Commit  
#### Commit semua perubahan yang berda dalam staging atau next commit
    $ git commit -a
#### Commit dengan memberi komentar
    $ git commit -m "is pesan"
    
### Unstaging
#### Menghapus file dari staging area dan tetap menjaga konten
    git reset nama_file.txt


## Working Directory
### Pindah Working Directory Cabang
    git checkout <branch>
> ini akan mengubah atau memindahkan isi direktori ke branch tertentu.
    
### Restore Working Directory
    git checkout .
> ini akan mereset dan mengembalikan isi direktori sebelum di edit atau di hapus.
