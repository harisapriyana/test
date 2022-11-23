<!-- Menyiapkan Tools -->
A. Hal pertama yang harus dilakukan adalah menyiapkan dan menginstal tools yang diperlukan untuk memulai sebuah program.
Untuk Aplikasi ini saya menggunakan
    1.  XAMPP 8.1.6 (https://www.apachefriends.org/download.html).
    2.  Composer (https://getcomposer.org/download/).
    3.  VS Code (https://code.visualstudio.com/download).
    4.  NPM (https://nodejs.org/en/download/).
    5.  Git (https://git-scm.com/downloads).

<!-- Installasi Laravel -->
B. Pada program web ini menggunakan PHP dengan framework Laravel beserta packagenya yaitu Breeze dan  Livewire
Langkah-langkah yang kita lakukan adalah meng-install melalui command line (cmd atau git bash) dimana saja bebas, misalnya di drive D:\
    1.  Laravel (composer create-project laravel/laravel story).
    2.  story pada akhir langkah pertama merupakan nama website atau projek kita dan otomatis dibuatkan folder dengan nama yang 
        sama yaitu story dan di dalamnya sudah terdapat default folder dan file yang dibutuhkan. Lalu pindahkan direktori tempat
        kita bekerja ke dalam folder story tersebut (cd story).
    3.  Tambahkan Livewire dengan cara (composer require laravel/jetstream) lalu, (php artisan jetstream:install livewire) dan 
        terakhir (php artisan vendor:publish --tag=jetstream-views). Bisa dilihat di (https://jetstream.laravel.com/)
    5.  Buat database baru dengan nama story dan tambahkan tabel yang sudah diberikan oleh Laravel dengan cara (php artisan 
        migrate) karena Livewire merupakan fitur bawaan dari Laravel untuk Login dan Registrasi User sehingga perlu dimasukan 
        tabel User.
    6.  Lalu akan diperintahkan untuk melakukan (npm install && npm run dev).
    7.  Tunggu sampai proses selesai.
    8.  Kita sudah bisa menggunakan fitur registrasi dan login, coba daftarkan satu user baru (haris@example.com, password).