# Laravel Queue
Pengiriman verifikasi email menggunakan modul Queue

## Instalasi
* Buka terminal linux
* Jalankan perintah berikut
```bash
$ cp .env.example .env
$ composer install
$ php artisan key:generate
```
* Buka file .env menggunakan text editor, lalu ubah dan sesuaikan dengan settingan yang dimiliki
* Setelah itu jalankan perintah berikut
``` bash
$ php artisan migrate
```
