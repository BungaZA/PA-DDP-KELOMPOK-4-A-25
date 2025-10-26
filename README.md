# PA-DDP-KELOMPOK-4-A-25
TEMA: Sistem Pemesanan Tiket Bis Digital

# Sistem Manajemen Transportasi Bus

## Deskripsi Proyek
Sistem Pemesanan Tiket Bis Digital adalah sistem berbasis Python yang memungkinkan pengelolaan data bus, penumpang, dan pemesanan tiket secara terintegrasi. Aplikasi ini memiliki dua jenis pengguna: **Admin** dan **Penumpang** dengan fitur yang berbeda.

## Anggota Kelompok
- Bunga Zulfa Aqila - 2509116024
- **Nama Anggota 2** - NIM  
- **Nama Anggota 3** - NIM


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
