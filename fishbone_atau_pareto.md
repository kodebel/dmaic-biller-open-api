Untuk melengkapi bagian **Analisis (Analyze)** dari metodologi DMAIC, baik **Fishbone Diagram** maupun **Pareto Chart** dapat digunakan, masing-masing untuk memberikan wawasan yang berbeda dalam mengidentifikasi masalah utama dan memprioritaskan faktor-faktor yang perlu diperbaiki.

### 1. **Fishbone Diagram**
Fishbone Diagram, yang sudah kita bahas sebelumnya, akan membantu kita mengidentifikasi berbagai penyebab potensial yang menghambat pengembangan dan implementasi **Biller Open API**. Diagram ini memungkinkan tim untuk melihat masalah dari berbagai perspektif (misalnya, proses, teknologi, orang, material, dan lingkungan).

Namun, untuk memprioritaskan masalah berdasarkan dampaknya, kita dapat melanjutkan dengan menggunakan **Pareto Chart**.

---

### 2. **Pareto Chart**

**Pareto Chart** adalah alat yang sangat efektif dalam mengidentifikasi dan memfokuskan usaha perbaikan pada masalah yang memiliki dampak paling besar. Dengan prinsip **80/20**, Pareto Chart dapat menunjukkan faktor mana yang paling berpengaruh terhadap masalah dan memberikan panduan tentang apa yang harus diprioritaskan untuk perbaikan.

#### **Langkah-langkah Membuat Pareto Chart:**

1. **Identifikasi Masalah**: Berdasarkan analisis Fishbone, kita dapat mengidentifikasi masalah yang paling sering terjadi atau yang paling kritikal. Sebagai contoh, beberapa masalah yang mungkin timbul dari analisis Fishbone adalah:
    - **Proses Integrasi yang Kompleks**.
    - **Kurangnya Dukungan Pengembang**.
    - **Stabilitas API**.
    - **Keterbatasan Platform**.

2. **Menghitung Frekuensi**: Mengukur seberapa sering masalah tersebut terjadi atau seberapa besar dampaknya terhadap tujuan proyek (misalnya, penurunan jumlah transaksi atau GTV).

3. **Mengurutkan Berdasarkan Dampak**: Setelah mengidentifikasi masalah, urutkan berdasarkan dampak atau frekuensi kejadian.

4. **Membuat Pareto Chart**: Menggunakan data yang telah dihitung, kita akan membuat sebuah diagram yang menunjukkan masalah utama di sisi kiri (dengan frekuensi terbesar) dan akan menyusun garis kumulatif untuk menunjukkan seberapa besar kontribusi masalah tersebut terhadap masalah keseluruhan.

#### **Contoh Data untuk Pareto Chart**:

Berikut adalah contoh data untuk **Pareto Chart**, berdasarkan hasil analisis yang telah kita buat sebelumnya:

| **Masalah**                        | **Frekuensi / Dampak** |
|------------------------------------|------------------------|
| **Proses Integrasi yang Kompleks** | 40%                    |
| **Kurangnya Dukungan Pengembang**  | 25%                    |
| **Stabilitas API**                 | 15%                    |
| **Keterbatasan Platform**          | 10%                    |
| **Regulasi yang Membatasi API**   | 5%                     |
| **Persaingan dengan Penyedia Lain**| 5%                     |

#### **Membuat Pareto Chart**:

1. **Data Urutkan**: Susun masalah berdasarkan **frekuensi** atau **dampak terbesar** di sisi kiri.
2. **Buat Diagram Batang**: Setiap masalah mendapat batang sesuai dengan tingkat frekuensi / dampak.
3. **Buat Garis Kumulatif**: Garis ini akan menunjukkan total kumulatif dari setiap masalah yang diselesaikan. Misalnya, 40% dari masalah terbesar ditangani, dan kemudian kita melihat berapa banyak masalah lainnya yang harus ditangani untuk mencapai total 80%.

#### **Visualisasi Pareto Chart**:

```plaintext
Masalah                            | Dampak (%) | Kumulatif (%)
---------------------------------------------------------------
Proses Integrasi yang Kompleks     | 40%        | 40%
Kurangnya Dukungan Pengembang      | 25%        | 65%
Stabilitas API                     | 15%        | 80%
Keterbatasan Platform              | 10%        | 90%
Regulasi yang Membatasi API       | 5%         | 95%
Persaingan dengan Penyedia Lain    | 5%         | 100%
```

- Dari Pareto Chart ini, kita bisa melihat bahwa **Proses Integrasi yang Kompleks** (40%) adalah masalah yang paling besar yang harus segera diatasi, diikuti oleh **Kurangnya Dukungan Pengembang** (25%), yang keduanya memberikan kontribusi lebih dari 60% terhadap masalah yang ada.

---

### **Kesimpulan dari Analisis dengan Pareto Chart:**

Dengan menggunakan **Pareto Chart**, kita dapat memfokuskan upaya perbaikan pada dua area utama:
1. **Simplifikasi Proses Integrasi**: Menyederhanakan atau merampingkan proses integrasi API akan memberikan dampak terbesar terhadap pengadopsian API dan peningkatan NOT/GTV.
2. **Peningkatan Dukungan Pengembang**: Memberikan dokumentasi yang lebih jelas dan pelatihan kepada pengembang dan merchant akan meningkatkan tingkat keberhasilan integrasi dan mempercepat adopsi API.

Penyelesaian masalah yang lebih kecil seperti **Stabilitas API** dan **Keterbatasan Platform** juga perlu diperhatikan, tetapi akan menjadi prioritas setelah dua masalah utama diatasi.

---

### **Alat Mana yang Cocok untuk Analisis (Fishbone Diagram vs. Pareto Chart)?**

- **Fishbone Diagram** cocok untuk **mengidentifikasi berbagai penyebab masalah** dan memberikan gambaran yang komprehensif tentang sumber masalah.
- **Pareto Chart** lebih efektif untuk **memprioritaskan masalah** yang memiliki dampak terbesar terhadap tujuan proyek, sehingga kita bisa memfokuskan sumber daya pada faktor-faktor yang akan memberi dampak signifikan terhadap peningkatan **NOT** dan **GTV**.

Kedua alat ini bekerja dengan baik secara bersamaan: Fishbone Diagram membantu untuk mengidentifikasi masalah utama, sedangkan Pareto Chart memberikan panduan untuk memprioritaskan masalah yang paling penting untuk ditangani terlebih dahulu.