# 🧠 Analisis Kepuasan Pelanggan Menggunakan Fuzzy Logic

## 📘 Deskripsi Proyek
Proyek ini bertujuan untuk **memprediksi tingkat kepuasan pelanggan** berdasarkan dua variabel utama:
- **Kecepatan layanan (Service Speed)**
- **Kualitas produk (Product Quality)**

Metode yang digunakan adalah **logika fuzzy (fuzzy logic)**, yang memungkinkan penilaian lebih fleksibel dibandingkan metode konvensional.  
Setiap pelanggan dinilai berdasarkan fungsi keanggotaan dan aturan fuzzy untuk menghasilkan nilai **Predicted Satisfaction**.

---

## ⚙️ Metodologi

1. **Pembuatan Dataset**  
   Dataset disusun dalam format CSV berisi kolom:
   - `Service_Speed` (1–10)
   - `Product_Quality` (1–10)
   - `Customer_Satisfaction` (1–10)

2. **Membership Function**  
   Dibuat menggunakan `scikit-fuzzy` untuk menentukan kategori:
   - Rendah (Low)
   - Sedang (Medium)
   - Tinggi (High)

3. **Fuzzy Rules (Aturan IF–THEN)**  
   Contoh:
   - Jika *Service Speed* tinggi **dan** *Product Quality* tinggi → *Satisfaction* tinggi  
   - Jika *Service Speed* rendah **dan** *Product Quality* sedang → *Satisfaction* sedang

4. **Inferensi & Defuzzifikasi**  
   Menghasilkan nilai kepuasan numerik (0–10) untuk setiap pelanggan.

---

## 📊 Hasil Visualisasi
Proyek menghasilkan plot distribusi tingkat kepuasan pelanggan yang memperlihatkan pola hubungan antara:
- Kecepatan layanan
- Kualitas produk
- Hasil prediksi kepuasan pelanggan

---

## 🧩 Teknologi yang Digunakan
| Library | Fungsi Utama |
|----------|---------------|
| **NumPy** | Operasi numerik dan vektor |
| **Pandas** | Manipulasi dan analisis data |
| **Matplotlib** | Visualisasi grafik |
| **Scikit-Fuzzy** | Implementasi logika fuzzy |

---

## 📦 Cara Menjalankan Proyek

### 1. Clone repository
```bash
git clone https://github.com/username/fuzzy-customer-satisfaction.git
cd fuzzy-customer-satisfaction

