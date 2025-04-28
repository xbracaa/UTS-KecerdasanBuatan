# UTS-KecerdasanBuatan
Tentu! Ini saya buatkan ulang **README.md**-nya, lengkap, rapi, dan sudah termasuk **semua** yang kamu minta, termasuk **Langkah Pengerjaan**:

---

# Sistem Pakar AI untuk Diagnosa Hama Tanaman 🌾🪲

## Deskripsi
Proyek ini mengembangkan **sistem pakar** sederhana untuk membantu **petani** dalam **mendiagnosis hama tanaman** berdasarkan gejala yang muncul.  
Gejala yang digunakan:
- Daun menguning
- Terdapat bercak hitam
- Daun berlubang
- Tanaman layu

Sistem akan mencocokkan input gejala dengan basis aturan yang tersedia untuk memberikan diagnosis hama atau penyakit tanaman.

---

## Alur Inferensi
1. Pengguna menginput kondisi tanaman berdasarkan empat gejala yang tersedia.
2. Input diubah menjadi fakta dalam sistem pakar.
3. Mesin inferensi mencocokkan fakta yang diberikan dengan aturan-aturan yang sudah ditentukan.
4. Sistem memberikan hasil diagnosis berdasarkan kecocokan antara fakta dan aturan.

---

## Aturan (Rule Base)
| Kondisi Gejala                                                              | Diagnosis                   |
|:----------------------------------------------------------------------------|:-----------------------------|
| Daun menguning, bercak hitam, tanaman layu                                   | Daun Busuk Berat             |
| Daun menguning, bercak hitam, tanpa daun berlubang dan tanpa layu             | Jamur Hitam                  |
| Daun menguning, daun berlubang, tanpa bercak hitam dan tanpa layu             | Ulat Daun                    |
| Daun menguning, tanaman layu, tanpa bercak hitam dan tanpa daun berlubang     | Busuk Akar                   |
| Hanya daun menguning                                                        | Kutu Daun                    |
| Tidak ada daun menguning                                                     | Gejala tidak sesuai, hama tidak terdeteksi |

---

## Pseudocode
```java
Input: Daun menguning (dm), Bercak hitam (bh), Daun berlubang (db), Tanaman layu (tl)

IF dm = True AND bh = True AND tl = True THEN
    Diagnosis = "Daun Busuk Berat"
ELSE IF dm = True AND bh = True AND db = False AND tl = False THEN
    Diagnosis = "Jamur Hitam"
ELSE IF dm = True AND db = True AND bh = False AND tl = False THEN
    Diagnosis = "Ulat Daun"
ELSE IF dm = True AND tl = True AND bh = False AND db = False THEN
    Diagnosis = "Busuk Akar"
ELSE IF dm = True AND bh = False AND db = False AND tl = False THEN
    Diagnosis = "Kutu Daun"
ELSE
    Diagnosis = "Gejala tidak sesuai, hama tidak terdeteksi"
```

---

## Implementasi
- **Bahasa**: Python
- **Library**: [experta](https://pypi.org/project/experta/)

### File
- `sistem_pakar.py`

### Cara Menjalankan
1. Pastikan Python sudah terinstall di komputer.
2. Install library **experta** dengan perintah:
    ```bash
    pip install experta
    ```
3. Jalankan program:
    ```bash
    python sistem_pakar.py
    ```

---

# 📄 Review Jurnal AI - Soal Nomor 1

## 📰 Informasi Jurnal
- **Judul**: Smart Irrigation System based on IoT and Machine Learning
- **Penulis**: Y. T. Tace
- **Tahun**: 2022
- **Sumber**: *Energy Reports*
- **DOI**: [10.1016/j.egyr.2022.07.088](https://doi.org/10.1016/j.egyr.2022.07.088)

---

## 🎯 Ringkasan

### Tujuan Penelitian
Penelitian ini bertujuan untuk mengoptimalkan hasil pertanian dan konservasi sumber daya melalui efisiensi penggunaan air dan pupuk dengan memanfaatkan teknologi IoT dan Machine Learning.

### Metode AI yang Digunakan
- **K-Nearest Neighbors (KNN)**: Prediksi kebutuhan irigasi berdasarkan data sensor.
- **Neural Networks**: Prediksi pengaktifan/penonaktifan pompa air.
- **Naive Bayes**: Klasifikasi kebutuhan irigasi berdasarkan kelembaban tanah dan suhu.
- **Support Vector Machine (SVM)**: Membuat model klasifikasi keputusan irigasi.
- **Regresi Logistik**: Menghitung probabilitas kategori kebutuhan irigasi.

### Manfaat
- Meningkatkan efisiensi penggunaan air.
- Membantu pengambilan keputusan berbasis data.
- Mengurangi penggunaan pupuk berlebihan.
- Meningkatkan produktivitas pertanian.
- Memudahkan pemantauan kondisi lahan secara real-time.

---

# 🛠️ Ide Pengembangan Lanjutan
- **Integrasi Prediksi Cuaca Real-Time**  
  Menunda penyiraman otomatis jika prediksi cuaca menunjukkan kemungkinan hujan tinggi.
  
- **Pembelajaran Adaptif dengan Reinforcement Learning**  
  Sistem belajar secara mandiri dari pengalaman untuk meningkatkan efisiensi penyiraman seiring waktu.

---

# 🌱 Ide Aplikasi Baru - EcoGarden AI
**EcoGarden AI** adalah aplikasi irigasi pintar skala kecil berbasis IoT dan AI sederhana untuk pengelolaan taman kota, taman rumah, dan fasilitas umum.

### Fitur:
- Monitoring sensor secara real-time.
- Penyiraman otomatis berbasis prediksi kebutuhan air.
- Laporan penggunaan air.
- Integrasi dengan prediksi cuaca lokal.

### Manfaat:
- Menghemat penggunaan air.
- Menjaga kesehatan tanaman.
- Mengurangi kerja manual.
- Mendukung penggunaan teknologi ramah lingkungan.

---

# 📝 Langkah Pengerjaan

1. **Mencari dan Memilih Jurnal**  
   Menentukan jurnal yang relevan tentang penerapan AI di bidang pertanian.

2. **Menganalisis Jurnal**  
   Membaca dan memahami tujuan, metode AI yang digunakan, dan manfaat dari penelitian tersebut.

3. **Menyusun Ringkasan Jurnal**  
   Membuat ringkasan poin-poin penting hasil analisis jurnal.

4. **Mengembangkan Ide Lanjutan**  
   Memberikan ide pengembangan sistem berbasis AI yang lebih adaptif dan inovatif.

5. **Merancang Ide Aplikasi Baru**  
   Membuat konsep aplikasi baru yang dapat diterapkan untuk meningkatkan efisiensi pertanian atau konservasi sumber daya.

6. **Menyusun Dokumentasi README.md**  
   Menyusun seluruh hasil tugas dalam format README.md yang terstruktur, rapi, dan jelas.

---

> 📌 **Catatan:**  
> README ini dibuat sebagai dokumentasi tugas "Sistem Pakar AI untuk Petani" dan review jurnal penerapan AI pada pertanian modern berbasis Machine Learning.

---

Selesai! 🎯  
README ini **lengkap, sistematis, dan siap** untuk langsung diunggah ke GitHub atau dilampirkan dalam laporan tugas.

Kalau kamu mau, saya juga bisa bantu sekalian buatkan contoh isi file `sistem_pakar.py` supaya lebih komplet lagi.  
Mau sekalian? 🚀
