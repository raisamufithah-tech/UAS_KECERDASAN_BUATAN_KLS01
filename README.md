# UAS Kecerdasan Buatan - Sistem Penjadwalan Mata Kuliah (Algoritma Genetika)

Repositori ini berisi implementasi program **Algoritma Genetika (Genetic Algorithm)** untuk sistem penjadwalan otomatis mata kuliah, sebagai bagian dari penyelesaian Ujian Akhir Semester (UAS) mata kuliah Kecerdasan Buatan.

## 👤 Informasi Mahasiswa
- **Nama Lengkap** : RAISA MUFITHAH
- **NIM**          : 24146039
- **Mata Kuliah**  : Kecerdasan Buatan (SIF210)
- **Program Studi**: Sistem Informasi
- **Dosen Pengampu**: Teuku Rizky Noviandy, S.Kom., M.Kom.

## 📝 Deskripsi Proyek
Proyek ini membangun sistem yang secara otomatis menghasilkan jadwal kuliah optimal dengan meminimalkan bentrok (konflik). Sistem dirancang untuk mengelola:
- 24 mata kuliah
- 6 dosen tetap
- 4 ruang kelas (R1 - R4)
- 12 slot waktu (Hari Senin - Kamis)

### Parameter Algoritma Genetika
- **Populasi Awal** : 60 individu (jadwal)
- **Generasi Maksimum** : 100 generasi
- **Tingkat Crossover** : 85%
- **Tingkat Mutasi** : 20%
- **Skala Fitness** : 0 - 100

### Aturan & Evaluasi Konflik (Constraint)
Sistem ini mencoba meminimalkan 3 jenis konflik utama:
1. **Konflik Ruang**: Dua mata kuliah berada di ruang dan waktu yang sama.
2. **Konflik Dosen-Waktu**: Dosen yang sama mengajar mata kuliah berbeda pada waktu yang sama.
3. **Konflik Dosen-Hari**: Dosen mengajar lebih dari satu mata kuliah pada hari yang sama.

## 📊 Hasil Evaluasi Akhir
Setelah berjalan selama 100 generasi, model menghasilkan penjadwalan terbaik dengan skor:
- **Fitness Terbaik** : 97
- **Sisa Konflik**    : 3
