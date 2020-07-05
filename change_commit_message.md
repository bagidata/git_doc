## Change Commit Message Terakhir

perintah :

`git commit --amend -m 'new message'`

### Tanpa pushed commit
Untuk mengubah message commit terakhir yang belum di push ke remote repository.

Jalankan perintah amend (change) message pada commit terakhir:

`git commit --amend -m "New commit message."`

Sebelum melalukan message commit, Anda juga dapat melakukan penambahan file yang berubah jika ada :

```
git add .
git commit --amend -m "New commit message."
```

### Dengan Pushed commit
Jika Anda mengubah pesan commit maka Anda harus melakukan push secara paksa (--force).

Push message coomit terbaru :

```
git commit --amend -m "New commit message."
git push --force branch-name
```

contoh :

```
git commit --amend -m "New commit message."
git push --force origin master
```
