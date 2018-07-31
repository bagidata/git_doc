## WARNING

Saat melakukan `git add` mungkin kita pernah menemukan warning seperti dibawah ini

`warning: LF will be replaced by CRLF in README.`

Dalam sistem unix akhir baris diwakili oleh Line Feed (LF). Sedangkan dalam sistem windows baris diwakili oleh carriage return (CR) dan akhir baris LF dengan CRLF.

Untuk mematikannya gunakan perintah berikut

```
git config core.autocrlf true
```

Untuk lebih detail bisa baca dokumentasinya di [Formating whitespace](http://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#Formatting-and-Whitespace)
