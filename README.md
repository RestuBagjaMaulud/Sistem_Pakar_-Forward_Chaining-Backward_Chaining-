# Sistem Pakar Diagnosis Penyakit
Sistem pakar adalah program komputer yang dirancang untuk meniru kemampuan pengambilan keputusan seorang pakar manusia. Dalam proyek ini, sistem pakar dibuat menggunakan metode Forward Chaining dan Backward Chaining untuk mendiagnosis berbagai penyakit berdasarkan gejala yang dialami pengguna.

## Metode Inferensi
1. Forward Chaining (Penalaran Maju)
   - Forward chaining bekerja dengan mengumpulkan fakta/gejala terlebih dahulu, lalu menerapkan aturan (rules) untuk menemukan kesimpulan (diagnosis).
   - Prosesnya seperti: Fakta ➜ Aturan ➜ Kesimpulan.
   - Cocok saat kita tahu data awal (gejala) dan ingin tahu hasil akhir (penyakit).
2. Backward Chaining (Penalaran Mundur)
   - Backward chaining mulai dari hipotesis/diagnosa lalu memeriksa apakah gejala-gejala pendukungnya terpenuhi.
   - Prosesnya seperti: Kesimpulan ➜ Periksa aturan ➜ Cek fakta.
   - Cocok saat kita ingin mengecek: “Apakah saya terkena penyakit X?”.

  ## Penjelasan Struktur Kode
  1. Fungsi ask_question() : Digunakan untuk mengumpulkan input gejala dari pengguna melalui pertanyaan.
  2. Forward Chaining : Sistem akan terus memeriksa apakah ada penyakit yang bisa disimpulkan berdasarkan fakta yang diberikan.
  3. Backward Chaining : Fungsi akan menelusuri apakah gejala yang mendukung goal ada dalam fakta pengguna, jika semua kondisi terpenuhi, maka goal dinyatakan benar.
  4. Aturan Diagnosis (rules)
