## KONFIGURE

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
