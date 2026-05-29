## ⚙️ Instalasi Lengkap

### 1. Clone Repository

```bash
git clone https://github.com/Ariefhuda434/BinaryProject.git
cd BinaryProject
```

### 2. Install Dependency

```bash
composer install
npm install
```

### 3. Konfigurasi Environment

Salin file `.env.example` menjadi `.env`

```bash
cp .env.example .env
```

Lalu generate application key:

```bash
php artisan key:generate
```

### 4. Konfigurasi Database

Sesuaikan konfigurasi database pada file `.env`

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=binaryproject
DB_USERNAME=root
DB_PASSWORD=
```

### 5. Migrasi Database

```bash
php artisan migrate --seed
```

### 6. Storage Link

```bash
php artisan storage:link
```

### 7. Jalankan Server

```bash
php artisan serve
npm run dev
```

Akses aplikasi melalui:

```txt
http://127.0.0.1:8000
```

---

# 🔑 Role Pengguna

| Role            | Hak Akses                                       |
| --------------- | ----------------------------------------------- |
| Admin           | Mengelola laporan, artikel, pengguna, statistik |
| Verifikator     | Memvalidasi laporan masyarakat                  |
| User/Masyarakat | Membuat dan memantau laporan                    |

---

# 📌 Alur Sistem

1. Masyarakat membuat laporan lokasi kotor.
2. Sistem menyimpan lokasi dan bukti foto.
3. Admin melakukan verifikasi laporan.
4. Dinas terkait menindaklanjuti laporan.
5. Status laporan diperbarui secara realtime.
6. Laporan selesai dapat dipublikasikan menjadi artikel berita.

---

# 🔐 Keamanan Sistem

BinaryProject menerapkan berbagai standar keamanan modern:

* Password hashing menggunakan Argon2id/Bcrypt
* CSRF Protection
* Rate Limiting API & Form
* Role Based Access Control (RBAC)
* Validasi upload file
* Activity Logging
* Secure Session Handling
* XSS Protection bawaan Blade Laravel

---

# 📈 Rencana Pengembangan

* [ ] Notifikasi WhatsApp / Telegram
* [ ] Progressive Web App (PWA)
* [ ] AI Deteksi Jenis Sampah dari Foto
* [ ] Heatmap Area Kotor di Kota Medan
* [ ] Sistem Reward Pelapor Aktif
* [ ] Export laporan PDF & Excel
* [ ] Mobile Apps Android/iOS

---

# 🤝 Kontribusi

Kontribusi sangat terbuka untuk pengembangan project ini.

Langkah kontribusi:

1. Fork repository
2. Buat branch fitur baru

```bash
git checkout -b fitur-baru
```

3. Commit perubahan

```bash
git commit -m "Menambahkan fitur baru"
```

4. Push ke branch

```bash
git push origin fitur-baru
```

5. Buat Pull Request

---

# 📄 License

Project ini menggunakan lisensi MIT License.

---

# 👨‍💻 Developer

Developed with ❤️ by BinaryProject Team

Jika project ini bermanfaat, jangan lupa ⭐ repository ini.
