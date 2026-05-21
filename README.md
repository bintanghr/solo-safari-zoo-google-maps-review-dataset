# Solo Safari Zoo Google Maps Review Dataset

## Deskripsi singkat
Dataset ini berisi ulasan Google Maps untuk lokasi Solo Safari Zoo. Setiap baris mewakili satu ulasan, termasuk rating bintang, teks ulasan, metadata reviewer, konteks kunjungan, dan tautan ulasan.

## Rentang waktu
- 30 Januari 2023 hingga 20 Septermber 2025

## File
- dataset_solo_safari.csv

## Format
- Tipe: CSV
- Header: ya (baris pertama berisi nama kolom)
- Pemisah: koma (,)
- Nilai kosong: ditulis kosong di antara dua koma
- Tanggal: ISO 8601 (contoh: 2025-09-20T09:23:40.489Z)

## Kolom
- isLocalGuide: string boolean ("true"/"false"), apakah reviewer adalah Local Guide
- likesCount: jumlah like pada ulasan (integer)
- name: nama reviewer (string)
- originalLanguage: bahasa asli ulasan (string, bisa kosong)
- publishedAtDate: waktu publikasi ulasan (ISO 8601)
- responseFromOwnerText: balasan pemilik (string, bisa kosong)
- reviewContext/Sebaiknya buat reservasi: jawaban konteks, mis. "Ya"/"Tidak"/"Tidak yakin" (string, bisa kosong)
- reviewContext/Waktu antrean: durasi antrean, mis. "Tanpa mengantre", "Maks 10 mnt" (string, bisa kosong)
- reviewContext/Waktu kunjungan: waktu kunjungan, mis. "Hari biasa", "Akhir pekan" (string, bisa kosong)
- reviewId: ID ulasan (string)
- reviewUrl: URL ulasan Google Maps (string)
- reviewerNumberOfReviews: jumlah ulasan reviewer (integer)
- stars: rating bintang (integer, 1-5)
- text: isi ulasan (string, bisa kosong)

## Catatan
- Beberapa kolom dapat kosong, termasuk originalLanguage, responseFromOwnerText, dan text.
- Kolom reviewContext/* adalah atribut konteks yang bergantung pada ketersediaan jawaban dari reviewer.