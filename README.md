# UAS Kecerdasan Buatan (SIF210)
## Sistem Penjadwalan Otomatis Mata Kuliah menggunakan Algoritma Genetika

**Nama Lengkap :** Hafizh Akramullah
**NIM          :** 24146054

---

## Deskripsi Proyek
Proyek ini merupakan Ujian Akhir Semester mata kuliah Kecerdasan Buatan. Tujuannya
adalah membangun sistem penjadwalan otomatis untuk 24 mata kuliah, 6 dosen tetap,
4 ruang kelas, dan 12 slot waktu, menggunakan **Algoritma Genetika (Genetic Algorithm)**
dengan tujuan meminimalkan konflik penjadwalan (konflik ruang, konflik dosen-waktu,
dan konflik dosen-hari).

## Struktur Repository
```
.
├── UAS_Penjadwalan_GA.ipynb   # Notebook lengkap (sudah dijalankan)
├── README.md                  # File ini
└── Laporan_UAS_Kecerdasan_Buatan.pdf   # Laporan ilmiah
```

## Parameter Algoritma Genetika
- Populasi awal: 60 individu
- Generasi maksimum: 100
- Tingkat crossover: 85% (single-point crossover)
- Tingkat mutasi: 20%
- Seleksi: tournament selection (k=3)
- Elitism: individu terbaik selalu dipertahankan ke generasi berikutnya
- Fitness: skala 0-100, dihitung dengan rumus `100 / (1 + jumlah_konflik)`

## Hasil
Algoritma Genetika berhasil menurunkan jumlah konflik secara signifikan selama
100 generasi, dengan hasil akhir:

- **Fitness Terbaik: 25.00**
- **Jumlah Konflik Tersisa: 3**

Grafik perkembangan fitness maksimum menunjukkan pola tangga (staircase) akibat
strategi elitism, sedangkan fitness rata-rata berfluktuasi mengikuti dinamika
populasi pada setiap generasi.

## Cara Menjalankan
1. Buka `UAS_Penjadwalan_GA.ipynb` di Google Colab.
2. Jalankan seluruh sel notebook secara berurutan (Runtime → Run all). Tidak
   diperlukan dataset eksternal atau API key, karena data mata kuliah, ruang,
   dan slot waktu sudah didefinisikan langsung di dalam notebook.

## Dosen Pengampu
Teuku Rizky Noviandy, S.Kom., M.Kom.
