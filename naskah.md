Berikut adalah **naskah narasi** yang dapat digunakan untuk menjelaskan proyek DMAIC beserta slide presentasi yang telah digenerate. Naskah ini disusun sesuai dengan alur presentasi dan mencakup penjelasan untuk setiap slide.

---

### **Slide 1: Cover Slide**
**Narasi**:
"Selamat pagi/siang/sore, semuanya. Terima kasih telah hadir dalam presentasi kami hari ini. Kami akan mempresentasikan proyek **Pengembangan Biller Open API AstraPay Bisnis** dengan menggunakan metodologi **DMAIC** (Define, Measure, Analyze, Improve, Control). Proyek ini bertujuan untuk meningkatkan **Number of Transactions (NOT)** dan **Gross Transaction Value (GTV)** melalui integrasi PPOB dengan aplikasi pihak ketiga seperti Moxa. Tim kami terdiri dari Baginda Syarif H., Fedora Ramadhanty W.P., Florentina Vela N., Rayyan Fathurrahman A., dan Kevin Kuwito."

---

### **Slide 2: Agenda**
**Narasi**:
"Berikut adalah agenda presentasi kami:
1. **Define**: Kami akan menjelaskan latar belakang proyek, tujuan, dan ruang lingkup.
2. **Measure**: Kami akan menunjukkan data transaksi dan performa AstraPay saat ini.
3. **Analyze**: Kami akan mengidentifikasi masalah utama menggunakan Fishbone Diagram.
4. **Improve**: Kami akan menjelaskan solusi yang diusulkan, termasuk proses integrasi dan pengembangan API.
5. **Control**: Kami akan menunjukkan bagaimana kami memastikan keberlanjutan proyek melalui dashboard merchant dan admin.
6. **Kesimpulan dan Rekomendasi**: Kami akan merangkum hasil dan memberikan rekomendasi untuk langkah selanjutnya."

---

### **Slide 3: Define - Identifikasi Proyek**
**Narasi**:
"Proyek ini dimulai dari identifikasi peluang bisnis. AstraPay sebagai penyedia jasa pembayaran di Indonesia memiliki fitur PPOB (Payment Point Online Bank) yang menjadi sumber utama **NOT** dan **GTV**. Saat ini, AstraPay tidak hanya melayani end-user, tetapi juga merchant-merchant seperti Moxa, Wanda, dan MotorkuX melalui AstraPay Bisnis. Namun, AstraPay Bisnis belum memiliki API terbuka PPOB yang memungkinkan integrasi dengan aplikasi pihak ketiga. Dengan mengembangkan **Biller Open API**, kami dapat memperluas jaringan merchant dan meningkatkan transaksi PPOB."

---

### **Slide 4: Define - Ringkasan SIPOC**
**Narasi**:
"Untuk memahami proyek ini secara holistik, kami menggunakan framework **SIPOC** (Supplier, Input, Process, Output, Customer).
- **Supplier**: Tim pengembang AstraPay, merchant, dan tim manajemen produk.
- **Input**: Data transaksi PPOB, kebutuhan merchant, dan spesifikasi API.
- **Process**: Mulai dari identifikasi kebutuhan, perencanaan, desain, pengembangan, pengujian, hingga peluncuran API.
- **Output**: Biller Open API, dokumentasi API, dan peningkatan adopsi merchant.
- **Customer**: Merchant, aplikasi pihak ketiga seperti Moxa, dan pengguna akhir."

---

### **Slide 5: Define - Project Charter**
**Narasi**:
"Berikut adalah **Project Charter** yang menjadi panduan proyek ini:
- **Stakeholders**: Anton Rifco Susilo sebagai Champion, Baginda Syarif H. sebagai Project Leader, dan tim pengembang.
- **Business Case**: AstraPay Bisnis belum memiliki API terbuka PPOB.
- **Problem Statement**: Perlunya API terbuka untuk integrasi dengan aplikasi pihak ketiga.
- **Project Goal**: Meningkatkan NOT dan GTV melalui PPOB.
- **Scope**: Fokus pada pengembangan API untuk merchant PPOB.
- **Benefit**: Meningkatkan transaksi PPOB, memperluas jangkauan pengguna, dan meningkatkan pendapatan.
- **Timeline**: Proyek ini berlangsung dari Januari hingga Mei 2024."

---

### **Slide 6: Measure - Data Collection**
**Narasi**:
"Pada tahap **Measure**, kami mengumpulkan data transaksi AstraPay dari tahun 2021 hingga 2024.
- **NOT** dan **GTV** untuk semua transaksi menunjukkan peningkatan signifikan, dari 7,1 juta transaksi pada 2021 menjadi 80,6 juta transaksi pada 2024.
- **Transaksi Biller** juga meningkat, dari 981 ribu transaksi pada 2021 menjadi 9 juta transaksi pada 2024.
- **Transaksi Payment Channel** AstraPay Bisnis juga menunjukkan pertumbuhan, dengan NOT mencapai 1,6 juta dan GTV mencapai 194 miliar pada 2024.
- Beberapa merchant seperti Moxa, MotorkuX, dan Paxel telah berkontribusi besar dalam transaksi ini."

---

### **Slide 7: Analyze - Fishbone Diagram**
**Narasi**:
"Pada tahap **Analyze**, kami menggunakan **Fishbone Diagram** untuk mengidentifikasi akar masalah. Masalah utama yang kami temukan adalah **integrasi API PPOB yang terhambat atau lambat**. Penyebabnya terbagi menjadi 5 kategori:
1. **Manusia**: Kurangnya keterampilan pengembang dan koordinasi tim.
2. **Proses**: Kompleksitas integrasi dan dokumentasi yang tidak jelas.
3. **Material**: Keterbatasan fitur dan stabilitas API.
4. **Mesin**: Keterbatasan infrastruktur dan kinerja server.
5. **Lingkungan**: Persaingan dengan penyedia lain dan regulasi yang membatasi."

---

### **Slide 8: Analyze - Fishbone Diagram Visual**
**Narasi**:
"Berikut adalah visualisasi **Fishbone Diagram** yang kami gunakan. Diagram ini membantu kami memetakan semua faktor penyebab dan fokus pada area yang perlu diperbaiki."

---

### **Slide 9: Improve - Proses Integrasi Merchant Biller Open API**
**Narasi**:
"Pada tahap **Improve**, kami merancang solusi untuk mengatasi masalah integrasi. Proses integrasi merchant meliputi:
1. Akuisisi merchant oleh tim partnership.
2. Verifikasi dan pendaftaran merchant di sistem AstraPay.
3. Generate Client ID dan Client Secret.
4. Top-up deposit oleh merchant.
5. Aktivasi merchant setelah deposit berhasil.
   Proses ini dirancang untuk memastikan integrasi yang lancar dan efisien."

---

### **Slide 10: Improve - Pengembangan Biller Open API**
**Narasi**:
"Kami juga mengembangkan **Biller Open API** dengan fitur-fitur utama:
- **Inquiry**: Untuk mengecek detail transaksi.
- **Transaksi**: Untuk memproses pembayaran.
- **Status Transaksi**: Untuk memantau status transaksi.
  Contoh request dan response API dapat dilihat pada slide ini. Dokumentasi lengkap tersedia di [link dokumentasi]."

---

### **Slide 11: Improve - Merchant Docs Biller Open API**
**Narasi**:
"Kami menyediakan **Merchant Docs** yang menjelaskan prosedur implementasi Biller Open API dari perspektif merchant. Dokumentasi ini dirancang untuk memudahkan pengembang aplikasi pihak ketiga dalam melakukan integrasi."

---

### **Slide 12: Control - Merchant Dashboard AstraPay Bisnis**
**Narasi**:
"Pada tahap **Control**, kami memastikan keberlanjutan proyek melalui **Merchant Dashboard**. Dashboard ini memungkinkan merchant untuk:
- Melihat produk dan keuntungan.
- Memantau transaksi menggunakan Biller Open API.
- Melakukan top-up deposit dan melihat mutasi saldo."

---

### **Slide 13: Control - Admin Dashboard AstraPay**
**Narasi**:
"Kami juga mengembangkan **Admin Dashboard** untuk memantau dan mengatur transaksi, produk, dan biaya layanan. Dashboard ini membantu tim AstraPay memastikan bahwa semua proses berjalan dengan lancar."

---

### **Slide 14: Kesimpulan dan Rekomendasi**
**Narasi**:
"Sebagai kesimpulan, proyek ini berpotensi meningkatkan **NOT** dan **GTV** melalui integrasi PPOB dengan aplikasi pihak ketiga. Rekomendasi kami:
1. Fokus pada penyederhanaan proses integrasi.
2. Meningkatkan kualitas dokumentasi dan pelatihan untuk pengembang.
3. Memastikan stabilitas dan performa API."

---

### **Slide 15: Q&A**
**Narasi**:
"Terima kasih atas perhatiannya. Sekarang, kami membuka sesi tanya jawab. Silakan ajukan pertanyaan atau masukan."

---

### **Slide 16: Thank You**
**Narasi**:
"Terima kasih sekali lagi atas waktu dan perhatiannya. Jika ada pertanyaan lebih lanjut, silakan hubungi tim kami melalui [email/kontak]. Sampai jumpa!"

---

Dengan naskah narasi ini, Anda dapat menjelaskan proyek DMAIC secara jelas dan terstruktur kepada audiens. Pastikan untuk menyesuaikan penjelasan dengan kecepatan dan kebutuhan audiens. Semoga presentasi Anda sukses!