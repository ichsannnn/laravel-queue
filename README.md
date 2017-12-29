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
$ php artisan queue:work
```
* Jalankan aplikasi, dan lakukan registrasi
* Email verifikasi akun hanya akan dikirimkan jika perintah **php artisan queue:work** dijalankan. Jika tidak, email tidak akan dikirimkan sampai perintah tersebut dijalankan.
* Alternatifnya gunakan perintah berikut untuk menjalankan perintah tersebut pada _background progress_
```bash
$ nohup php artisan queue:work &
```
* Alternatif lainnya adalah gunakan [Cron Job](https://github.com/skadevz/laravel-task-scheduling) untuk menjalankan perintah setiap menit
* Alternatif lain untuk pengguna linux, gunakan [Supervisor](https://laravel.com/docs/5.5/queues#supervisor-configuration).
