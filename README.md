# Food / Fruit & Veg Estimation Classifier

Aplikasi ini menggunakan model deep learning untuk mengklasifikasikan gambar makanan, buah, dan sayur, serta memberikan estimasi waktu dan tips penyimpanan berdasarkan hasil klasifikasi.

## Fitur

- Upload gambar makanan, buah, atau sayur
- Klasifikasi otomatis menggunakan model MobileNetV2
- Estimasi waktu dan tips penyimpanan dari Gemini API
- Visualisasi probabilitas prediksi

## Instalasi

### 1. Clone repository

```powershell
git clone https://github.com/Hazz-i/Food-Estimation.git
cd Food-Estimation
```

### 2. Buat dan aktifkan environment (opsional, rekomendasi)

```powershell
python -m venv venv
.\venv\Scripts\activate
```

### 3. Install dependencies

```powershell
pip install -r requirements.txt
```

### 4. Siapkan file model dan label

Pastikan file berikut tersedia di folder `model/`:

- `mobilenetv2_fruit_veggie.keras` (model)
- `class_names.txt` (label kelas, satu label per baris)

### 5. Konfigurasi API Key Gemini

Buat file `.env` di root folder, isi dengan:

```
GEMINI_API_KEY=your_api_key_here
```

## Menjalankan aplikasi

```powershell
streamlit run main.py
```

Akses aplikasi melalui browser di alamat yang tertera.

## Catatan

- Model dan label sudah disediakan di folder `model/`.
- Untuk hasil estimasi penyimpanan, pastikan API key Gemini valid.
- Jika ada error, cek kembali dependensi dan file yang diperlukan.

## Lisensi

MIT
