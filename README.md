**Nama  : Aldo Khrisna Wijaya**

**NIM   : 2341760091**

**Kelas : SIB - 3C**

# Jobsheet 7 Membangun Aplikasi OCR Sederhana

## Hasil Percobaan

1. Splash Screen
![Screenshot ocr_sederhana](images/00.png)

1. Home Screen
![Screenshot ocr_sederhana](images/01.png)

1. Scan Screen
![Screenshot ocr_sederhana](images/02.png)

1. Result Screen
![Screenshot ocr_sederhana](images/03.png)

# UTS Membangun Aplikasi OCR

## Soal 1: Modifikasi Struktur Navigasi dan Aliran

- Tujuan: Menyederhanakan alur navigasi dan meningkatkan pengalaman pengguna di
HomeScreen.
1. Pengubahan Navigasi Home (15 Poin):

    • Ubah ElevatedButton di HomeScreen (lib/screens/home_screen.dart) menjadi *widget* **ListTile**.
    
    • Atur ListTile: leading: Icon(Icons.camera_alt, color: Colors.blue);
    title: Text(’Mulai Pindai Teks Baru’).

    • Fungsi onTap harus menggunakan Navigator.push() untuk ke ScanScreen.

    • Hasil:
![Screenshot ocr_sederhana](images/1.1.png)

2. Teks Utuh dan Navigasi Balik (15 Poin):
    
    • Di ResultScreen (lib/screens/result_screen.dart), hapus fungsi ocrText.replaceAllagar hasil teks ditampilkan dengan baris baru (\n) yang utuh.
    
    • Tambahkan FloatingActionButton dengan ikon Icons.home.
    
    • Ketika tombol ditekan, navigasi harus kembali langsung ke HomeScreen menggunakan **Navigator.pushAndRemoveUntil()** (atau metode yang setara) untuk menghapus semua halaman di atasnya dari stack navigasi.

    • Hasil:
    
    1. scan
![Screenshot ocr_sederhana](images/1.2.1.png)
    2. hasil
![Screenshot ocr_sederhana](images/1.2.2.png)
    3. menekan tombol home
![Screenshot ocr_sederhana](images/1.1.png)