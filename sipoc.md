Berikut adalah **SIPOC** (Supplier, Inputs, Process, Outputs, Customer) yang relevan untuk proyek **Biller Open API** dalam konteks **Define** tahap DMAIC dari AstraPay:

---

### **SIPOC - Biller Open API (AstraPay)**

#### **1. Supplier (Pemasok)**
Supplier adalah pihak-pihak yang menyediakan sumber daya, informasi, atau input yang diperlukan untuk menjalankan proses.

- **Tim Pengembang AstraPay**: Menyediakan keahlian teknis dalam mengembangkan **Biller Open API**.
- **Merchant yang ada (misalnya Moxa, Wanda, MotorkuX)**: Memberikan insight tentang kebutuhan mereka dan bagaimana API dapat diterapkan dalam sistem mereka.
- **Tim Manajemen Produk**: Mengidentifikasi dan mendefinisikan fitur dan fungsi yang harus ada pada **Biller Open API** berdasarkan kebutuhan pasar dan pengguna.
- **Tim Keuangan dan Analitik**: Menyediakan data terkait dengan **NOT** (Number of Transaction) dan **GTV** (Gross Transaction Value) untuk mengukur dampak dari proyek ini.
- **Penyedia Teknologi dan Infrastruktur**: Memberikan alat dan platform yang diperlukan untuk menghosting dan mendukung API.

#### **2. Inputs (Masukan)**
Inputs adalah bahan atau informasi yang digunakan untuk melaksanakan proses yang ada.

- **Data Transaksi PPOB**: Informasi tentang **Number of Transactions (NOT)** dan **Gross Transaction Value (GTV)** yang akan digunakan untuk menilai keberhasilan API setelah diluncurkan.
- **Kebutuhan dari Merchant**: Umpan balik dari merchant mengenai tantangan yang mereka hadapi dalam proses pembayaran PPOB dan kebutuhan integrasi API.
- **Spesifikasi Fungsional API**: Dokumen yang mendefinisikan bagaimana API seharusnya bekerja, termasuk endpoint, autentikasi, dan struktur data yang diperlukan.
- **Dokumentasi API**: Dokumen panduan yang menjelaskan cara integrasi API dengan aplikasi pihak ketiga.
- **Platform Teknologi**: Infrastruktur dan teknologi yang akan digunakan untuk mengembangkan dan menghosting **Biller Open API**.

#### **3. Process (Proses)**
Proses adalah serangkaian langkah yang diperlukan untuk mengubah input menjadi output.

1. **Identifikasi Kebutuhan**: Mengumpulkan data tentang kebutuhan merchant dan pengguna akhir terkait dengan layanan PPOB yang bisa diakses melalui API.
2. **Perencanaan Pengembangan API**: Menyusun rencana pengembangan untuk **Biller Open API** berdasarkan spesifikasi teknis dan umpan balik yang diperoleh dari pihak terkait.
3. **Desain dan Pengembangan API**: Tim pengembang membuat API yang mudah digunakan dan dapat diintegrasikan oleh merchant dan aplikasi pihak ketiga (seperti Moxa).
4. **Penyusunan Dokumentasi API**: Menyusun dokumentasi yang jelas dan mudah dipahami, termasuk contoh kode dan tutorial integrasi.
5. **Pengujian API**: Melakukan uji coba untuk memastikan API berfungsi dengan baik dalam berbagai kondisi dan integrasi yang dilakukan oleh merchant berjalan lancar.
6. **Peluncuran API**: Setelah API siap, meluncurkan API untuk digunakan oleh merchant dan aplikasi pihak ketiga, dengan dukungan dan edukasi terkait penggunaan API.
7. **Pengumpulan Feedback**: Mengumpulkan umpan balik dari merchant dan pengguna mengenai penggunaan **Biller Open API** serta melakukan perbaikan yang diperlukan.

#### **4. Outputs (Keluaran)**
Outputs adalah hasil atau produk yang dihasilkan dari proses yang telah dilakukan.

- **Biller Open API**: API yang dapat diintegrasikan dengan aplikasi pihak ketiga dan digunakan oleh merchant untuk memproses transaksi PPOB.
- **Dokumentasi API**: Panduan teknis lengkap yang memungkinkan pengembang mengintegrasikan API dengan mudah.
- **Peningkatan Adopsi Merchant**: Merchant yang mulai mengadopsi API untuk memproses transaksi PPOB, yang meningkatkan **Number of Transactions (NOT)** dan **Gross Transaction Value (GTV)**.
- **Laporan Feedback**: Umpan balik yang dikumpulkan dari merchant dan pengguna tentang API dan integrasinya.

#### **5. Customer (Pelanggan)**
Customer adalah pihak yang menerima output dari proses.

- **Merchant yang Terhubung dengan AstraPay**: Merchant yang mengintegrasikan API untuk memproses pembayaran PPOB dan meningkatkan efisiensi transaksi mereka. Contoh: Moxa, Wanda, MotorkuX, dan merchant lainnya.
- **Aplikasi Pihak Ketiga (misalnya Moxa)**: Aplikasi yang terhubung dengan **Biller Open API** untuk menawarkan produk PPOB kepada pengguna akhir mereka.
- **Pengguna Akhir (End-User)**: Konsumen yang melakukan pembayaran melalui aplikasi yang mengintegrasikan **Biller Open API** untuk melakukan transaksi PPOB.
- **Tim Manajemen AstraPay**: Menerima laporan kinerja API, feedback dari merchant, dan data transaksi untuk menganalisis dampak terhadap **NOT** dan **GTV**.

---

### **Ringkasan SIPOC:**

| **Supplier**                       | **Inputs**                                                    | **Process**                                                                                                                                       | **Outputs**                                                                            | **Customer**                                      |
|------------------------------------|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|--------------------------------------------------|
| Tim Pengembang AstraPay            | Data Transaksi PPOB                                          | 1. Identifikasi Kebutuhan                                                                                                                      | Biller Open API                                                                    | Merchant yang Terhubung dengan AstraPay         |
| Merchant (Moxa, Wanda, MotorkuX)   | Kebutuhan dari Merchant                                       | 2. Perencanaan Pengembangan API                                                                                                                  | Dokumentasi API                                                                    | Aplikasi Pihak Ketiga (Moxa)                    |
| Tim Manajemen Produk               | Spesifikasi Fungsional API                                    | 3. Desain dan Pengembangan API                                                                                                                   | Peningkatan Adopsi Merchant                                                          | Pengguna Akhir (End-User)                       |
| Tim Keuangan dan Analitik          | Dokumentasi API                                              | 4. Penyusunan Dokumentasi API                                                                                                                    | Laporan Feedback                                                                    | Tim Manajemen AstraPay                         |
| Penyedia Teknologi dan Infrastruktur | Platform Teknologi                                           | 5. Pengujian API                                                                                                                                 |                                                                                      |                                                  |
|                                    |                                                              | 6. Peluncuran API                                                                                                                                 |                                                                                      |                                                  |
|                                    |                                                              | 7. Pengumpulan Feedback                                                                                                                           |                                                                                      |                                                  |

---

Dengan menggunakan SIPOC ini, **AstraPay** dapat lebih jelas memahami alur proses pengembangan **Biller Open API** dan bagaimana tiap pihak terkait berperan dalam menyukseskan proyek ini. SIPOC ini juga membantu dalam mengidentifikasi pemangku kepentingan (stakeholders) dan memastikan bahwa input yang tepat diperoleh untuk menghasilkan output yang diinginkan untuk pelanggan (merchant dan pengguna akhir).