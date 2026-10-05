# Telkom University Company Profile - Praktikum

Project simulasi HTML, CSS, PHP native, MySQL/MariaDB, dan Git.

## Dokumentasi Merge Conflict

Simulasi conflict dilakukan pada file `includes/header.php`, tepatnya pada baris menu navigasi Profil.

| Branch | Perubahan | Teks menu |
|---|---|---|
| `main` | Commit `style: ubah label profil pada main` | Tentang Kampus |
| `conflict-navbar` | Commit `feat: ubah label profil pada branch conflict` | Tentang Kami |

**Penyebab conflict:** kedua branch mengubah baris yang sama pada file yang sama dengan isi berbeda, sehingga Git tidak dapat menentukan versi mana yang dipakai.

**Cara penyelesaian:**
1. Membuka `includes/header.php` dan membaca marker `<<<<<<<`, `=======`, dan `>>>>>>>`.
2. Menentukan teks final, yaitu **Profil**.
3. Menghapus seluruh marker conflict dan menyisakan satu baris menu.
4. Menjalankan `git add includes/header.php`.
5. Menjalankan `git commit -m "merge: selesaikan conflict navbar"`.
6. Memeriksa halaman di browser untuk memastikan navbar tetap valid.

Perubahan ini dibuat dari simulasi Laptop B.

   Catatan tahap kedua dari Laptop B.

   ## Cara Menjalankan

1. Letakkan folder project di `C:\xampp\htdocs\telkom-company-profile`.
2. Jalankan Apache dan MySQL lewat XAMPP Control Panel.
3. Buka phpMyAdmin, lalu impor atau jalankan `database/telkom_profile.sql`.
4. Buka `http://localhost/telkom-company-profile/` di browser.