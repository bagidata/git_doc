## KONFIGURASI

### Konfigurasi informasi user untuk semua lokal repository
    $ git config --global user.name "[name]"
    
    $ git config --global user.email "[email address]"

    $ git config --global color.ui auto

### Cek setting proxy saat ini

    git config --global --get http.proxy

### Proxy

    $ git config --global http.proxy http://username:password@proxyname:8080

### Unset proxy

    git config --global --unset http.proxy
    
    
### Koneksi Github dengan SSH

#### Membuat key SSH

```
$ ssh-keygen
```

Maka didalam direktori ~/.ssh/ akan terdapat file key baru.

#### Jalankan SSH agent dan load SSH key

pastikan SSH agent sudah berjalan dengan baik.

```
ps -e | grep [s]sh-agent
```

Jika belum jalan gunakan perinta berikut untuk menjalankan SSH agent :

```
ssh-agent /bin/bash
```

Load SSh key :
```
ssh-add ~/.ssh/id_anda
```

Cek apakah sudah diload :

```
ssh-add -l
```

#### Jalankan SSH key ke Github

Copy text yang ada pada direktori `~/.ssh/id_anda.pb`

Paste-kan ke Github di `Setting>SSH and GPG Keys`

#### Tes Konektivitas

Jalankan perinya berikut :

```
ssh -T git@github.com
```

Selesai.

