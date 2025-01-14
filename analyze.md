### **Analyze (Analisis)**

Dalam tahap analisis, tujuan utama adalah untuk menggali akar masalah yang menghambat pencapaian target proyek serta mengidentifikasi peluang dan penyebab ketidakefisienan yang ada dalam proses integrasi PPOB dengan merchant. Berikut adalah hasil analisis berdasarkan data yang telah dikumpulkan serta evaluasi mendalam mengenai tantangan yang dihadapi oleh AstraPay dan para merchantnya.

#### **1. Data Transaksi dan Tren Pertumbuhan**

Berdasarkan data transaksi yang ada, kita bisa melihat adanya peningkatan yang signifikan dalam **Number of Transactions (NOT)** dan **Gross Transaction Value (GTV)** baik untuk **transaksi seluruh AstraPay** maupun khusus untuk layanan PPOB. Namun, ada beberapa temuan yang perlu diperhatikan:

- **Pertumbuhan Transaksi PPOB (Biller)** relatif lebih rendah dibandingkan dengan total transaksi yang terjadi di platform AstraPay. Hal ini menunjukkan bahwa meskipun ada adopsi yang meningkat, **fokus pada transaksi PPOB** belum maksimal.

- Meskipun **jumlah transaksi PPOB** meningkat dari tahun ke tahun, kontribusinya terhadap **GTV** masih relatif kecil. Ini bisa menjadi indikasi bahwa meskipun volume transaksi meningkat, rata-rata nilai transaksi PPOB masih relatif rendah.

#### **2. Analisis Transaksi berdasarkan Merchant**

Tabel berikut menunjukkan volume transaksi yang terjadi untuk beberapa merchant yang menggunakan **Payment Channel AstraPay Bisnis** pada 2024. Hal ini memberikan gambaran seberapa besar kontribusi setiap merchant terhadap volume transaksi PPOB di AstraPay:

| **Merchant**                    | **Jumlah Download (Playstore)** | **NOT 2024**  | **GTV 2024**  |
|----------------------------------|---------------------------------|---------------|---------------|
| **Moxa**                         | 5jt+                            | 8.311         | 594.320.434   |
| **MotorkuX**                     | 1jt+                            | 13            | 3.002.350     |
| **Wahana Honda**                 | 1jt+                            | 107           | 21.837.851    |
| **Daya Auto**                    | 1jt+                            | 633           | 16.573.900    |
| **Brompit**                      | 1jt+                            | 1             | 65.350        |
| **Paxel**                        | 1jt+                            | 33.047        | 1.347.610.222 |
| **Bank Saqu**                    | 1jt+                            |               |               |
| **Baqoel (Ecommerce sembako)**   | 5rb+                            |               |               |

**Temuan:**
- **Moxa** menunjukkan kontribusi yang sangat besar terhadap **NOT** dan **GTV**, yang menunjukkan bahwa merchant dengan pengguna aktif yang banyak dapat memberikan dampak signifikan terhadap volume transaksi.
- **MotorkuX** dan **Wahana Honda** menunjukkan performa yang lebih rendah dalam hal **NOT** dan **GTV**, meskipun jumlah download cukup tinggi. Ini bisa mengindikasikan masalah dalam pemanfaatan fitur PPOB oleh pengguna mereka.

Penting untuk dicatat bahwa meskipun beberapa merchant seperti **Moxa** memiliki basis pengguna yang besar, fitur PPOB mungkin belum sepenuhnya dimanfaatkan oleh pengguna mereka, atau terdapat hambatan dalam integrasi yang mempengaruhi volume transaksi. Ini juga menjadi area yang perlu diperbaiki dengan mempermudah proses integrasi API.

#### **3. Masalah yang Dihadapi Merchant dalam Menggunakan PPOB**

Berdasarkan umpan balik dari merchant, beberapa masalah utama yang dapat menghambat adopsi dan penggunaan layanan PPOB AstraPay antara lain:

1. **Proses Integrasi yang Kompleks**:
    - Beberapa merchant mengeluhkan bahwa integrasi dengan sistem PPOB AstraPay membutuhkan waktu yang lama dan keterampilan teknis yang mendalam. Hal ini bisa menghalangi merchant kecil atau pengembang independen yang ingin bergabung.

2. **Kurangnya Dokumentasi yang Jelas**:
    - Dokumentasi API yang tidak cukup jelas atau lengkap menyebabkan kesulitan dalam implementasi bagi developer yang ingin mengintegrasikan PPOB ke dalam aplikasi mereka.

3. **Fitur API yang Tidak Memadai**:
    - Merchant mungkin mengalami keterbatasan dalam fitur API yang tersedia, seperti tidak dapat menyesuaikan pengalaman pengguna atau mengatur berbagai jenis transaksi (misalnya, pembayaran listrik, air, telepon) dengan cara yang lebih fleksibel.

4. **Persaingan dengan Penyedia PPOB Lain**:
    - Beberapa aplikasi atau platform lain mungkin menawarkan integrasi PPOB yang lebih mudah dan memiliki API yang lebih terbuka. Hal ini membuat merchant lebih tertarik untuk memilih penyedia lain yang lebih fleksibel dan cepat diintegrasikan.

#### **4. Evaluasi dari Kompetitor**

Analisis terhadap kompetitor dalam industri PPOB menunjukkan beberapa faktor kunci yang membuat mereka lebih unggul dalam hal adopsi oleh merchant:

- **API Terbuka**: Beberapa platform kompetitor sudah memiliki API terbuka yang lebih mudah diakses oleh merchant. Dengan menggunakan API terbuka, pihak ketiga dapat dengan cepat mengembangkan aplikasi yang terintegrasi dengan sistem pembayaran mereka.

- **Fitur yang Fleksibel dan Dapat Disesuaikan**: Penyedia PPOB lain mungkin menawarkan API dengan fitur yang lebih fleksibel dan lebih mudah disesuaikan dengan kebutuhan bisnis merchant, seperti kemampuan untuk mengelola berbagai jenis pembayaran atau menawarkan harga yang lebih kompetitif.

- **Dukungan Pengembang yang Lebih Baik**: Kompetitor mungkin memiliki dokumentasi yang lebih lengkap dan lebih baik, serta tim dukungan yang lebih responsif untuk membantu merchant dalam proses integrasi.

#### **5. Penyebab Utama dari Masalah yang Dihadapi**

- **Kompleksitas Integrasi API**: API AstraPay mungkin belum cukup sederhana dan membutuhkan waktu lebih lama untuk diintegrasikan oleh merchant, terutama untuk aplikasi pihak ketiga yang ingin menggunakan layanan PPOB.

- **Keterbatasan dalam Dokumentasi**: Dokumentasi API yang kurang jelas dan tidak memadai menghambat pengembang dalam memahami cara mengintegrasikan API secara efisien.

- **Kurangnya Dukungan Pengembang**: Ketidakhadiran dukungan teknis yang cukup untuk pengembang yang ingin memanfaatkan API PPOB AstraPay bisa membuat merchant kesulitan dalam implementasi dan adopsi.

#### **6. Peluang yang Dapat Diberikan oleh Biller Open API**

Melalui Biller Open API, AstraPay memiliki peluang untuk:

- **Meningkatkan Volume Transaksi**: Dengan membuka API untuk integrasi lebih banyak aplikasi, AstraPay dapat menarik lebih banyak merchant dan meningkatkan volume transaksi PPOB.

- **Memperluas Pasar**: Dengan memungkinkan aplikasi seperti Moxa dan lainnya untuk mengintegrasikan layanan PPOB AstraPay, AstraPay dapat memperluas jangkauan pasar dan menjangkau lebih banyak pengguna.

- **Meningkatkan Keterlibatan Merchant**: Mempermudah integrasi dan menyediakan dukungan teknis yang lebih baik dapat membantu AstraPay mempertahankan hubungan yang lebih kuat dengan merchant dan meningkatkan loyalitas mereka.

---

### **Kesimpulan dari Analisis**

Untuk mencapai tujuan dari proyek **Biller Open API**, AstraPay perlu mengatasi beberapa tantangan yang dihadapi oleh merchant dan pengguna aplikasi pihak ketiga. **Menyederhanakan integrasi API**, **menyediakan dokumentasi yang lebih jelas dan lengkap**, serta **menyediakan dukungan yang lebih baik** bagi pengembang akan menjadi langkah kunci untuk meningkatkan adopsi PPOB AstraPay dan mencapai target **NOT** dan **GTV** yang lebih tinggi.