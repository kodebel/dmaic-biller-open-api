# Pembuatan Biller Open API AstraPay Bisnis
#### DMAIC (Define, Measure, Analyze, Improve, Control) Methodology

## **Define (Definisikan)**

### 1. **Identifikasi Project**
AstraPay sebagai penyedia jasa pembayaran di Indonesia, menyediakan fitur PPOB (Payment Point Online Bank) untuk customer AstraPay.
Fitur PPOB tersebut menjadi salah satu sumber NOT (Number of Transaction) dan juga GTV (Gross Transaction Value) AstraPay sebagai Aplikasi pembayaran digital.
Saat ini Customer AstraPay bukan satu satu nya yang menjadi enduser dari AstraPay,
tetapi juga merchant-merchant yang tergabung menjadi AstraPay Bisnis.
Merchant merchant tersebut menggunakan produk yang ada pada AstraPay Bisnis.
Produk tersebut adalah Merchant QRIS (Merchant yang mengguanakan QRIS AstraPay sebgai penerima pembayaran), Payment Channel (Merchant yang menggunakan AstraPay sebagai alat pembayaran), Astrapay Disbursement (Merchant yang melakukan transfer dana ke banyak tujuan), dan Mitra AstraPay (Merchant yang terafiliasi dengan AstraPay untuk menjual produk AstraPay kepada yang belum menggunakan AstraPay).
Moxa, Wanda, dan MotorkuX adalah beberapa contoh merchant yang tergabung dalam AstraPay Bisnis (Payment Channel). Khususnya pada aplikasi Moxa yang telah diunduh oleh 5jt lebih dari playstore terdapat fitur PPOB. AstraPay dengan AstraPay bisnis nya dapat melihat peluang bisnis yang ada pada aplikasi Moxa tersebut, untuk menjual produk PPOB lewat Biller Open API (API terbuka biller) yang ada pada fitur PPOB AstraPay.


### 2. **Ringkasan SIPOC**

| **Supplier**                                        | **Inputs**                 | **Process**                     | **Outputs**                 | **Customer**                            |
|-----------------------------------------------------|----------------------------|---------------------------------|-----------------------------|-----------------------------------------|
| Tim Pengembang AstraPay (Product Team)              | Data Transaksi PPOB        | 1. Identifikasi Kebutuhan       | Biller Open API             | Merchant yang Terhubung dengan AstraPay |
| Merchant (Moxa, Wanda, MotorkuX)                    | Kebutuhan dari Merchant    | 2. Perencanaan Pengembangan API | Dokumentasi API             | Aplikasi Pihak Ketiga (Moxa)            |
| Tim Manajemen Produk (Partnership & BD)             | Spesifikasi Fungsional API | 3. Desain dan Pengembangan API  | Peningkatan Adopsi Merchant | Pengguna Akhir (End-User)               |
| Tim Keuangan (FBAT)                                 | Dokumentasi API            | 4. Penyusunan Dokumentasi API   | Laporan Feedback            | Tim Manajemen AstraPay                  |
| Penyedia Teknologi dan Infrastruktur (Tech & Infra) | Platform Teknologi         | 5. Pengujian API                |                             |                                         |
|                                                     |                            | 6. Peluncuran API               |                             |                                         |
|                                                     |                            | 7. Pengumpulan Feedback         |                             |                                         |


| **Aktor** | Tim Pengembang AstraPay               | Merchant, Tim Manajemen Produk (Partnership & BD) | Tim Keuangan (FBAT), Tim Manajemen Produk (Partnership) | Penyedia Teknologi dan Infrastruktur (Tech & Infra) |
|-----------|---------------------------------------|---------------------------------------------------|---------------------------------------------------------|-----------------------------------------------------|
| **Tools** | IDE, Jira, Jenkins, Github, Ms. Teams | AstraPay Docs, Sandbox                            | Power BI                                                | GCP                                                 |



### 3. **Project Charter**:

- **Stakeholders**:
  - Champion: **Anton Rifco Susilo** (Head of AstraPay Product I)
  - Project Leader: **Baginda Syarif H.**
  - Team Members: **Fedora Ramadhanty W.P.**, **Florentina Vela N.**, **Rayyan Fathurrahman A.**, **Kevin Kuwito**
  - Support Functions: **Tech & Infra Teams**, **Partnership Teams**, **FBAT Teams**, **Merchant AstraPay Bisnis**
  
- **Business Case**:
  - AstraPay Bisnis belum memiliki API terbuka PPOB yang memungkinkan integrasi dengan aplikasi pihak ketiga.
  
- **Problem Statement**:
  - AstraPay ingin mengembangkan dan meluncurkan **Biller Open API** untuk memperluas jaringan merchant dan meningkatkan **NOT (Number of Transactions)** serta **GTV (Gross Transaction Value)**, dengan memanfaatkan fitur PPOB dan memungkinkan integrasi lebih mudah dengan aplikasi pihak ketiga (termasuk aplikasi seperti Moxa yang sudah memiliki 5 juta pengguna).

- **Project Goal**:
    - Mengembangkan **Biller Open API** yang dapat diintegrasikan oleh berbagai aplikasi dan merchant untuk menawarkan layanan PPOB kepada lebih banyak pengguna.
    - Menyediakan API yang dapat diakses dengan mudah oleh developer dan merchant.
    - Meningkatkan volume transaksi dan pendapatan melalui PPOB dan produk terkait.

- **Scope**:
    - Fokus pada pengembangan API terbuka untuk **merchant PPOB** yang memungkinkan integrasi dengan aplikasi-aplikasi seperti **Moxa**.
    - Menyediakan dokumentasi API yang jelas untuk pengembang aplikasi dan merchant.
    - Mengukur dampak terhadap **Number of Transaction (NOT)** dan **Gross Transaction Value (GTV)** setelah implementasi.

- **Benefit**:
  - Meningkatkan jumlah transaksi PPOB melalui merchant yang terhubung dengan AstraPay.
  - Memperluas jangkauan pengguna melalui aplikasi pihak ketiga seperti Moxa.
  - Meningkatkan pendapatan melalui layanan PPOB dan produk terkait.
  - Memperkuat posisi AstraPay sebagai penyedia layanan pembayaran terkemuka di Indonesia.

- **Project Timeline**:
  
  | **Steps**             | Deliverables       | Jan | Feb | Mar | Apr | May |
  |-----------------------|--------------------|-----|-----|-----|-----|-----|
  | **Define**            | SIPOC              | X   |     |     |     |     |
  |                       | Project Charter    | X   |     |     |     |     |
  |                       | Project Approval   | X   |     |     |     |     |
  | **Measure & Analyze** | Data Collection    |     | X   |     |     |     |
  |                       | Data Visualization |     | X   |     |     |     |
  |                       | Solutioning        |     | X   |     |     |     |
  | **Improve**           | Implementation     |     |     | X   | X   | X   |
  | **Control**           | Documentation      |     |     |     |     | X   |
  |                       | ???                |     |     |     |     | X   |

  *referensi link: https://astrapay.atlassian.net/jira/software/c/projects/PAY/boards/52/timeline?epic=COMPLETE12M&hideProgress=true&hideVersionHeader=true&issueParent=46511%2C64135&timeline=MONTHS*

- **Project Approval**:
  - **Anton Rifco Susilo** (Head of AstraPay Product I)


## **Measure (Ukur)**

### **1. Data Collection**

  - **Number of Transactions (NOT) & Gross Transaction Value (GTV) Pertahun 2021 s.d 2024**

    - **All Transactions AstraPay**

      | **Tahun** | 2021               | 2022               | 2023               | 2024               | 2025 (Target KPI) |
      |-----------|--------------------|--------------------|--------------------|--------------------|-------------------|
      | **NOT**   | 7.159.199          | 32.002.140         | 59.882.424         | 80.658.857         | 86.3 Jt           |
      | **GTV**   | 72.856.306.280.237 | 37.804.523.134.732 | 61.155.476.439.475 | 88.654.659.193.736 | 42.4 T            |
    
    - **Transaksi Biller**

      | **Tahun** | 2021            | 2022              | 2023              | 2024              |
      |-----------|-----------------|-------------------|-------------------|-------------------|
      | **NOT**   | 981.654         | 7.160.844         | 8.782.376         | 9.052.735         |
      | **GTV**   | 781.817.785.201 | 63.95.496.716.343 | 8.600.115.136.355 | 9.290.415.703.514 |

    - **Transaksi Payment Channel AstraPay Bisnis**

      | **Tahun** | 2023           | 2024            |
      |-----------|----------------|-----------------|
      | **NOT**   | 1.257.015      | 1.698.331       |
      | **GTV**   | 76.309.766.385 | 194.976.678.921 |


- **Jumlah Merchant yang menggunakan produk Payment Channel AstraPay Bisnis (https://astrapay.atlassian.net/wiki/spaces/PD/pages/2430926913/List+Merchant+On+Development)**

 | **Merchant**                       | Ter-download (Playstore) | NOT 2024 | GTV 2024      | |
 |------------------------------------|--------------------------|----------|---------------|-|
 | **Moxa**                           | 5jt+                     | 8.311    | 594.320.434   | |
 | **MotorkuX**                       | 1jt+                     | 13       | 3.002.350     | |
 | **Wahana Honda (Booking service)** | 1jt+                     | 107      | 21.837.851    | |
 | **Daya Auto (Booking service)**    | 1jt+                     | 633      | 16.573.900    | |
 | **Brompit (Booking service)**      | 1jt+                     | 1        | 65.350        | |
 | **Paxel (Jasa logistik)**          | 1jt+                     | 33.047   | 1.347.610.222 | |
 | **Bank Saqu**                      | 1jt+                     |          |               | |
 | **Baqoel (Ecommerce sembako)**     | 5rb+                     |          |               | |


## **Analyze (Analisis)**
### 1. **Fishbone Diagram (Diagram Tulang Ikan)**

**Masalah Utama**: **Integrasi API PPOB yang Terhambat / Lambat**

#### **Kategori Penyebab:**

1. **Manusia (People)**:
    - **Keterampilan Pengembang**: Pengembang aplikasi pihak ketiga (seperti Moxa) mungkin tidak memiliki keterampilan teknis untuk melakukan integrasi API dengan benar.
    - **Kurangnya Pelatihan dan Dukungan**: Pengembang dan merchant mungkin tidak diberikan pelatihan atau dukungan yang cukup mengenai penggunaan dan integrasi API.
    - **Kurangnya Koordinasi antara Tim**: Tim pengembang AstraPay dan tim merchant mungkin tidak berkomunikasi secara efektif, yang menyebabkan penundaan dalam proses integrasi.

2. **Proses (Process)**:
    - **Proses Integrasi yang Kompleks**: Proses untuk menghubungkan aplikasi pihak ketiga dengan API PPOB AstraPay terlalu rumit dan memerlukan banyak langkah teknis, yang mempengaruhi kecepatan adopsi.
    - **Dokumentasi yang Tidak Jelas**: Dokumentasi API yang kurang lengkap atau tidak mudah dipahami, menyebabkan kesulitan bagi pengembang dan merchant untuk mengimplementasikan API.
    - **Proses Pengujian yang Tidak Memadai**: Pengujian API yang tidak memadai atau tidak cukup komprehensif, yang menyebabkan kegagalan integrasi saat aplikasi pihak ketiga mencobanya.

3. **Material (Material)**:
    - **API yang Tidak Memadai**: API yang tidak cukup fleksibel atau tidak dapat disesuaikan dengan kebutuhan merchant atau aplikasi pihak ketiga.
    - **Keterbatasan Fitur dalam API**: Beberapa fitur penting seperti pengelolaan berbagai jenis transaksi atau pengaturan pembayaran yang lebih spesifik tidak ada dalam API.
    - **Stabilitas API**: API mungkin mengalami masalah performa atau down-time, yang menghambat transaksi merchant.

4. **Mesin (Machine)**:
    - **Keterbatasan Teknologi Infrastruktur**: Infrastruktur teknis yang digunakan untuk mendukung API PPOB AstraPay mungkin tidak cukup kuat untuk menangani beban transaksi yang lebih besar atau integrasi dengan lebih banyak aplikasi pihak ketiga.
    - **Kinerja Server**: Masalah pada server atau cloud yang digunakan untuk mendukung API dapat menyebabkan masalah pada kecepatan dan keandalan layanan.
    - **Keterbatasan Platform yang Digunakan**: Beberapa platform yang digunakan oleh merchant atau pengembang aplikasi (misalnya, perangkat mobile, OS, atau library) mungkin tidak kompatibel dengan API AstraPay.

5. **Lingkungan (Environment)**:
    - **Persaingan dengan Penyedia Lain**: Penyedia PPOB lain yang menawarkan API yang lebih mudah diintegrasikan atau lebih fleksibel. Hal ini bisa membuat merchant lebih memilih menggunakan penyedia lain yang lebih mudah dan cepat diintegrasikan.
    - **Regulasi yang Membatasi**: Beberapa regulasi atau kebijakan pemerintah yang membatasi cara kerja atau pengelolaan data dalam integrasi pembayaran, yang dapat mempengaruhi adopsi API.
    - **Perubahan Teknologi atau Tren Pasar**: Perubahan dalam preferensi pasar atau teknologi yang digunakan oleh pengembang aplikasi dapat mempengaruhi keputusan untuk mengintegrasikan API AstraPay.

### **Diagram Visualisasi Fishbone**:

```plaintext
                             +-----------------------------------------------+
                             |        Masalah Utama: Lambat Integrasi API   |
                             +-----------------------------------------------+
                                      /                    |                     \
                                    /                       |                      \
                          +-----------------+       +-----------------+      +----------------+
                          |    Manusia      |       |     Proses      |      |     Material    |
                          +-----------------+       +-----------------+      +----------------+
                            /           \            /        |         \          /      \
        +------------+    +------------+  +-----------+  +------------+  +---------+  +-------------+
        |Keterampilan|    |Pelatihan   |  |Proses     |  |Dokumentasi |  |Fitur    |  |Stabilitas  |
        |Pengembang  |    |& Dukungan  |  |Integrasi  |  |API yang    |  |API      |  |API         |
        +------------+    +------------+  |Kompleksitas|  |Tidak Jelas |  |Terbatas |  |Server      |
                           |             |           |  +------------+  +---------+  +-------------+
                           |             |           |                             
                           |             |    +----------------+      +----------------------+
                  +--------+--------+    | Pengujian API   |      | Kinerja Server        |
                  | Kurangnya Koordi-|    +----------------+      +----------------------+
                  | nasi Tim         |  
                  +------------------+

                                 +---------------------------+
                                 |   Mesin (Machine)         |
                                 +---------------------------+
                                     /            |            \
                       +-------------+        +-------------+  +--------------+
                       |Keterbatasan |        | Kinerja     |  | Platform    |
                       | Infrastruktur|        | Server      |  | Kompatibilitas |
                       +-------------+        +-------------+  +--------------+

                                 +----------------------------+
                                 |  Lingkungan (Environment)  |
                                 +----------------------------+
                                      /         |        \
                        +------------+    +------------+   +-------------+
                        | Persaingan |    | Regulasi   |   | Perubahan  |
                        | dengan Peny|    | yang Membat|   | Teknologi  |
                        |edia Lain   |    | asi API    |   | dan Tren   |
                        +------------+    +------------+   +-------------+
```

---

### **Kesimpulan dari Fishbone Diagram**:
Diagram ini membantu kita mengidentifikasi berbagai faktor penyebab yang bisa mempengaruhi proses pengembangan dan adopsi **Biller Open API**. Beberapa faktor utama yang perlu segera ditangani adalah **kompleksitas integrasi API**, **kurangnya dukungan dan pelatihan untuk pengembang dan merchant**, **keterbatasan fitur dalam API**, serta **persaingan dengan penyedia PPOB lain**. Dengan fokus pada perbaikan di area ini, kita dapat meningkatkan proses integrasi API dan mempercepat adopsi oleh merchant dan aplikasi pihak ketiga.

## **Improve (Perbaikan)**
### 1. **Flow Integrasi Merchant Biller Open API**
- referensi flowchart: https://astrapay.atlassian.net/wiki/spaces/PD/pages/2643394562/Version+1.1+Enterprise+RFC+Technical+Implementation+-+Open+API+Biller+Open+API#Flow
- addjust flowchart sampai merchant live production

 
### 2. **Merchant Docs Biller Open API**
- referensi link: https://astrapay.atlassian.net/wiki/spaces/PD/pages/2643394562/Version+1.1+Enterprise+RFC+Technical+Implementation+-+Open+API+Biller+Open+API
- jelaskan 3 transaksi, 2 api athorization, 1 api products
    
    -  




