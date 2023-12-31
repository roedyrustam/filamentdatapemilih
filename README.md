# API Wilayah Indonesia 2024

API Wilayah Indonesia adalah project open source laravel Filament untuk akses data Provinsi, Kabupaten, Kecamatan dan Kelurahan di Indonesia.
2024
## Requirement

-   PHP 8.1
-   MYSQL (untuk Database)
-   Composer 2.1^
-   Internet, karena menggunakan composer dan untuk mengunduh dependency yang diperlukan saat install
-   Git (Optional) Untuk clone project
-   Code Editor (Optional) Untuk edit konfigurasi .env (bisa pakai notepad, notepad++, vscode, sublime, atau nano, vim dll)

## Installation

-   Untuk mejalankan project ini di lokal, ikuti langkah berikut:

-   Clone project ini dengan cara download atau dengan command :

```bash
git clone https://github.com/roedyrustam/filamentdatapemilih.git
```

-   Masuk ke folder project dan Install dependency dengan composer

```bash
cd laravel-api-wilayah
composer install
```

-   Buat File .env dan generate key

```
cp .env.example .env
php artisan key:generate
```

-   Buka vscode atau kode editor lain untuk ubah konfigurasi db di file .env

## Migrasi Data dan Seeding Data'

Secara default, master data Provinsi, Kabupaten, Kecamatan dan Kelurahan ada di folder `public/json` dengan format json.

-   Untuk migrasi jalankan command :

```
php artisan migrate
```

-   Untuk seeding data jalankan command :

```
php artisan db:seed --class=FromJsonSeeder
```

## Run Project

-   Jalankan command :

```
php artisan serve
```

-   Buka browser, akses http://127.0.0.1:8000/admin
    Done.

- Login User = admin@gmail.com
- pass = admin12345


## Roadmap

-   [x] Include dasboard to manage data
-   [x] Update data terbaru
-   [x] Include kode pos
-   [ ] Include latitude and longitude
