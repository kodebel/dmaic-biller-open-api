# Biller Open API
#### DMAIC (Define, Measure, Analyze, Improve, Control) Methodology

## AstraPay Bisnis
AstraPay sebagai penyedia jasa pembayaran di Indonesia, menyediakan fitur PPOB (Payment Point Online Bank) untuk customer AstraPay.
Fitur PPOB tersebut menjadi salah satu sumber NOT (Number of Transaction) dan juga GTV (Gross Transaction Value) AstraPay sebagai Aplikasi pembayaran digital.
Saat ini Customer AstraPay bukan satu satu nya yang menjadi enduser dari AstraPay,
tetapi juga merchant-merchant yang tergabung menjadi AstraPay Bisnis.
Merchant merchant tersebut menggunakan produk yang ada pada AstraPay Bisnis.
Produk tersebut adalah Merchant QRIS (Merchant yang mengguanakan QRIS AstraPay sebgai penerima pembayaran), Payment Channel (Merchant yang menggunakan AstraPay sebagai alat pembayaran), Astrapay Disbursement (Merchant yang melakukan transfer dana ke banyak tujuan), dan Mitra AstraPay (Merchant yang terafiliasi dengan AstraPay untuk menjual produk AstraPay kepada yang belum menggunakan AstraPay).
Moxa, Wanda, dan MotorkuX adalah beberapa contoh merchant yang tergabung dalam AstraPay Bisnis (Payment Channel). Khususnya pada aplikasi Moxa yang telah diunduh oleh 5jt lebih dari playstore terdapat fitur PPOB. AstraPay dengan AstraPay bisnis nya dapat melihat peluang bisnis yang ada pada aplikasi Moxa tersebut yang menjual produk PPOB yang mungkin serupa dengan yang ada pada AstraPay.

### **1. Define (Definisikan)**
- **Problem Statement**:
  AstraPay ingin mengembangkan dan meluncurkan **Biller Open API** untuk memperluas jaringan merchant dan meningkatkan **NOT (Number of Transactions)** serta **GTV (Gross Transaction Value)**, dengan memanfaatkan fitur PPOB dan memungkinkan integrasi lebih mudah dengan aplikasi pihak ketiga (termasuk aplikasi seperti Moxa yang sudah memiliki 5 juta pengguna).

- **Project Goal**:
    - Mengembangkan **Biller Open API** yang dapat diintegrasikan oleh berbagai aplikasi dan merchant untuk menawarkan layanan PPOB kepada lebih banyak pengguna.
    - Menyediakan API yang dapat diakses dengan mudah oleh developer dan merchant.
    - Meningkatkan volume transaksi dan pendapatan melalui PPOB dan produk terkait.

- **Scope**:
    - Fokus pada pengembangan API terbuka untuk **merchant PPOB** yang memungkinkan integrasi dengan aplikasi-aplikasi seperti **Moxa**.
    - Menyediakan dokumentasi API yang jelas untuk pengembang aplikasi dan merchant.
    - Mengukur dampak terhadap **Number of Transaction (NOT)** dan **Gross Transaction Value (GTV)** setelah implementasi.
