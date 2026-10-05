# Telkom University Company Profile - Praktikum

Project simulasi HTML, CSS, PHP native, MySQL/MariaDB, dan Git.

## Cara Menjalankan

1. Letakkan folder project di `C:\xampp\htdocs\telkom-company-profile`.
2. Jalankan Apache dan MySQL lewat XAMPP Control Panel.
3. Buka phpMyAdmin, lalu impor atau jalankan `database/telkom_profile.sql`.
4. Buka `http://localhost/telkom-company-profile/` di browser.

## Dokumentasi Merge Conflict

Simulasi conflict dilakukan pada file `includes/header.php`, tepatnya pada baris menu navigasi Profil.

| Branch | Perubahan | Teks menu |
|---|---|---|
| `main` | Commit `style: ubah label profil pada main` | Tentang Kampus |
| `conflict-navbar` | Commit `feat: ubah label profil pada branch conflict` | Tentang Kami |

**Penyebab conflict:** kedua branch mengubah baris yang sama pada file yang sama dengan isi berbeda, sehingga Git tidak dapat menentukan versi mana yang dipakai.

**Cara penyelesaian:**
1. Membuka `includes/header.php` dan membaca marker `<<<<<<<`, `=======`, dan `>>>>>>>`.
2. Menentukan teks final, yaitu **Profile**.
3. Menghapus seluruh marker conflict dan menyisakan satu baris menu.
4. Menjalankan `git add includes/header.php`.
5. Menjalankan `git commit -m "merge: selesaikan conflict navbar"`.
6. Memeriksa halaman di browser untuk memastikan navbar tetap valid.

## Simulasi Dua Laptop

Folder kedua (`telkom-company-profile-B`) dibuat dengan `git clone` untuk mensimulasikan Laptop B.

Perubahan ini dibuat dari simulasi Laptop B.

Catatan tahap kedua dari Laptop B.

## Riwayat Praktikum Git

```text
* 14c818e (HEAD -> main, origin/main, origin/HEAD) docs: rapikan format README
* 438f7a3 docs: tambahkan cara menjalankan project
* abf1398 Revert "docs: tambah catatan dari Laptop A"
*   8be0cb4 Merge branch 'main' of https://github.com/syakirabdurrahman42-art/telkom-company-profile-109062500151
|\
| * b462bea docs: tambah catatan dari Laptop B
* | 92637da docs: tambah catatan dari Laptop A
|/
* e1c7cf5 docs: perbarui README dari Laptop B
* dda40c2 docs: dokumentasikan penyelesaian conflict
*   615c068 merge: selesaikan conflict navbar
|\
| * 1f7b936 feat: ubah label profil pada branch conflict
* | 6c3a486 style: ubah label profil pada main
|/
* 5280527 feat: tambahkan informasi fokus pembelajaran
* 7437396 feat: tambahkan form admin lokal untuk berita
* 4c95e28 feat: simpan pesan kontak ke database
* 74b7483 feat: tambahkan daftar dan detail berita
* e2399a5 feat: hubungkan database dan tampilkan program studi
* f8550fd docs: ubah judul tujuan proyek
* 934c9a4 docs: ubah judul visi pembelajaran
* d3f2b28 feat: tambahkan layout dasar dan stylesheet
* 6e87ef8 chore: inisialisasi project dan dokumentasi awal
```