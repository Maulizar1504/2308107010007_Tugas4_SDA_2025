Nama : MAulizar

NPM  : 2308107010061

-Penjelasan Tugas 4 :

# 📊 Tugas 4 – Evaluasi Algoritma Sorting (Waktu & Memori)

Proyek ini mengevaluasi performa enam algoritma sorting berdasarkan **waktu eksekusi** dan **penggunaan memori**, terhadap dataset **angka dan kata acak** hingga 2 juta elemen. Semua algoritma diimplementasikan dalam bahasa C dan diuji pada sistem operasi Windows menggunakan `psapi.h`.

## 📚 Algoritma yang Diuji
- Bubble Sort
- Selection Sort
- Insertion Sort
- Merge Sort
- Quick Sort
- Shell Sort

## 🧪 Desain Eksperimen
- Dataset: angka acak dan kata acak berukuran dari 10.000 hingga 2.000.000 elemen
- Bahasa: C
- Pengukuran waktu: `clock()` dari `<time.h>`
- Pengukuran memori: `GetProcessMemoryInfo()` dari `psapi.h` (Windows only)
- Setiap algoritma diuji secara independen untuk masing-masing dataset dan ukuran

## ⚙️ Cara Menjalankan
```bash
gcc main.c -o benchmark_sort -lpsapi
./benchmark_sort angka data_angka.txt
./benchmark_sort kata data_kata.txt

