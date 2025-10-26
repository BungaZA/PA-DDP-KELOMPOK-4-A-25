# PA-DDP-KELOMPOK-4-A-25
TEMA: Sistem Pemesanan Tiket Bis Digital

# Sistem Manajemen Transportasi Bus

## Deskripsi Proyek
Sistem Pemesanan Tiket Bis Digital adalah sistem berbasis Python yang memungkinkan pengelolaan data bus, penumpang, dan pemesanan tiket secara terintegrasi. Aplikasi ini memiliki dua jenis pengguna: **Admin** dan **Penumpang** dengan fitur yang berbeda.

## Anggota Kelompok
- **Bunga Zulfa Aqila** - 2509116024
- **Aulia Sheva Savitri** - 2509116001
- **Annisa Nayzhua Febriyani** - 2509116013


## Flowchart
<img width="2345" height="1418" alt="Bis digital-Menu utama y drawio" src="https://github.com/user-attachments/assets/0784865e-3dc9-4b63-a0f6-6bb01a8133b2" />

<img width="1295" height="999" alt="Bis Digital-menu admin drawio" src="https://github.com/user-attachments/assets/6e4eb45e-d2a1-4560-9f57-5390f73f24b2" />

<img width="610" height="507" alt="Screenshot 2025-10-26 190908" src="https://github.com/user-attachments/assets/b0708c47-d611-4b9f-bd31-b0eb69e1a680" />

<img width="1340" height="426" alt="Screenshot 2025-10-26 191113" src="https://github.com/user-attachments/assets/abffb6c8-51a7-42ee-ab49-4e45c1c9b327" />

<img width="1337" height="289" alt="Screenshot 2025-10-26 191242" src="https://github.com/user-attachments/assets/d28d8680-4928-450d-8764-0351e26269d6" />

<img width="1123" height="520" alt="Screenshot 2025-10-26 191407" src="https://github.com/user-attachments/assets/835c45ab-932b-4236-9640-64552add6e7d" />

<img width="790" height="367" alt="Screenshot 2025-10-26 191420" src="https://github.com/user-attachments/assets/3438d2e4-3767-4d53-975e-60487c231a54" />

<img width="985" height="502" alt="Screenshot 2025-10-26 191439" src="https://github.com/user-attachments/assets/215335da-83b7-44fb-a2b0-58db275beb6a" />

<img width="625" height="481" alt="Screenshot 2025-10-26 191454" src="https://github.com/user-attachments/assets/6feae965-a326-4d01-b23d-c5697934d2c3" />


## Fitur Utama

### Fitur Admin
- **Manajemen Bus**: Tambah, lihat, update, dan hapus data bus
- **Data Penumpang**: Melihat daftar penumpang terdaftar
- **Laporan Booking**: Melihat riwayat pemesanan tiket dan total pendapatan

### Fitur Penumpang
- **Registrasi & Login**: Membuat akun dan login ke sistem
- **Pemesanan Tiket**: Memesan tiket bus dengan sistem e-money
- **Manajemen Akun**: Melihat dan mengubah data akun
- **Top Up E-Money**: Mengisi saldo e-money
- **Riwayat Booking**: Melihat dan membatalkan pemesanan tiket

## Hal hal yang perlu Digunakan
- **Python 3.x**
- **JSON** untuk penyimpanan data
- **PrettyTable** untuk menampilkan data dalam format tabel
- **Pwinput** untuk input password yang aman
- **OS** untuk manipulasi sistem

## Cara Menjalankan Program

### Prasyarat
1. Install library yang diperlukan:


pip install prettytable pwinput


## Login Default

### Admin
- **Username**: admin
- **Password**: admin123

### Penumpang
- Buat akun baru melalui menu "Belum punya akun"

## Sistem E-Money
- Setiap penumpang memiliki saldo e-money
- Saldo awal: Rp 0
- Top up tersedia: Rp 20.000, Rp 50.000, Rp 100.000, Rp 500.000
- Pembayaran tiket otomatis memotong saldo e-money

## Rute yang Tersedia
- **Asal**: Samarinda, Kutai Kartanegara
- **Tujuan**: Samarinda, Kutai Kartanegara
- **Keterangan**: Asal dan tujuan tidak boleh sama

## Fitur Keamanan
- Limit percobaan login (maksimal 3 kali)
- Validasi input untuk mencegah error
- Error handling yang komprehensif
- Password hidden saat input

## Data yang Disimpan
Program secara otomatis menyimpan data dalam file JSON:
- bus.json - Data bus dan kursi tersedia
- user.json - Data akun penumpang dan saldo e-money  
- booking.json - Riwayat pemesanan tiket

## Cara Penggunaan

### Untuk Admin:
1. Login dengan user dan pw admin yang disediakan
2. Pilih "Manajemen Bus" untuk mengelola data bus
3. Gunakan fitur tambah, edit, atau hapus bus
4. Lihat semua penumpang yang telah membuat akun
5. Lihat laporan pemesanan di "Lihat Booking Penumpang"

### Untuk Penumpang:
1. Buat akun baru atau login
2. Top up e-money terlebih dahulu
3. Lihat bus tersedia dan pesan tiket
4. Kelola pemesanan melalui menu "Lihat Tiket Saya"

## Error Handling
Program telah dilengkapi dengan error handling untuk:
- Input tidak valid
- File tidak ditemukan
- Keyboard interrupt (Ctrl+C)
- EOF error (Ctrl+D)
- Exception umum lainnya

## Catatan Penting
- Bus tidak bisa dihapus jika masih ada penumpang
- Penumpang tidak bisa hapus akun jika masih ada saldo e-money
- Jumlah kursi bus antara 1-20
- Harga tiket antara Rp 10.000 - Rp 100.000


Proyek ini dibuat untuk keperluan akademik.

---

**Dibuat dengan ❤️ oleh Kelompok 4 - Mata Kuliah Praktikum Dasar Dasar Pemrograman**
