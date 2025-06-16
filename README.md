# Laravel Flutter Todo App

A fullstack Todo App using **Laravel 10** (backend REST API) and **Flutter 3** (frontend mobile app).


## Fitur

- **Autentikasi**: Register, Login, Logout.
- **CRUD Todo**: Tambah, lihat, edit, hapus todo.
- **Pencarian**: Cari todo berdasarkan kata kunci.
- **Detail Todo**: Klik item untuk melihat detail di halaman baru.
- **Token Otomatis**: Token login disimpan di device, tidak perlu login ulang.

---

## Struktur Proyek

```
backend/          # Laravel 10 REST API
frontend_mobile/  # Flutter 3 mobile app
```

---

## Cara Menjalankan

### 1. Backend (Laravel)

1. Buat database baru, misal: `todo_app`.
2. Masuk ke folder `backend`:
    ```sh
    cd backend
    ```
3. Install dependencies:
    ```sh
    composer install
    npm install
    npm run dev
    ```
4. Copy `.env.example` menjadi `.env`, atur konfigurasi database, lalu generate app key:
    ```sh
    cp .env.example .env
    # Edit .env sesuai database Anda
    php artisan key:generate
    ```
5. Jalankan migrasi:
    ```sh
    php artisan migrate
    ```
6. Jalankan server Laravel:
    ```sh
    php artisan serve
    ```

### 2. Frontend (Flutter)

1. Masuk ke folder `frontend_mobile`:
    ```sh
    cd frontend_mobile
    ```
2. Pastikan file `.env` dan `.env.dev` sudah ada dan atur variabel `API_PROJECT_HOST` sesuai alamat backend.
3. Jalankan perintah berikut:
    ```sh
    flutter clean
    flutter pub get
    flutter run
    ```

---

## Konfigurasi Environment

- **Backend**: Atur `.env` di folder `backend`.
- **Frontend**: Atur `.env` dan `.env.dev` di folder `frontend_mobile` (lihat contoh pada file).

---

## Paket Flutter yang Digunakan

- [`flutter_screenutil`](https://pub.dev/packages/flutter_screenutil) - Responsive design
- [`flutter_dotenv`](https://pub.dev/packages/flutter_dotenv) - Environment variables
- [`http`](https://pub.dev/packages/http) - HTTP request
- [`shared_preferences`](https://pub.dev/packages/shared_preferences) - Local storage

---

## Minimum Requirement

- **Android**: Min SDK 21 (Android 5.0)
- **Flutter**: 3.13.2
- **Laravel**: 10.x

---

## Lisensi

- Laravel: [MIT License](https://opensource.org/licenses/MIT)
- Flutter: [BSD License](https://github.com/flutter/flutter/blob/master/LICENSE)

---




