# Data-Summarization-With-IBM

# UFC Fight Outcome Classification & Summarization using IBM Granite

## Overview  
Project ini merupakan bagian dari Capstone Assignment Hacktiv8 yang berfokus pada data classification dan summarization.  
Dataset UFC digunakan untuk menganalisis hasil pertarungan (KO/TKO, Submission, Decision) dengan memanfaatkan LLM IBM Granite melalui Replicate API.  

Tujuan utama:  
-  Melakukan klasifikasi hasil pertarungan UFC menggunakan bantuan LLM.  
-  Membuat ringkasan insight berdasarkan hasil klasifikasi.  
-  Mendemonstrasikan pemanfaatan LLM IBM Granite untuk analisis data tabular.  

---

## 📂 Dataset  
Dataset berasal dari Kaggle:  
🔗 [UFC Fight Forecast Complete Gold Modeling Dataset](https://www.kaggle.com/datasets/jerzyszocik/ufc-fight-forecast-complete-gold-modeling-dataset)  

File utama yang digunakan:  
- `UFC_full_data_golden.csv`  

## ⚙️ Metodologi  

### 1. Preprocessing Data  
- Ambil kolom relevan:  
  - `event_name`  
  - `winner`  
  - `weight_class`  
  - `gender`  
  - `result`  
  - `finish_round`  
- Hapus nilai kosong (`NaN`) agar data lebih bersih.  

### 2. Classification dengan IBM Granite  
Model IBM Granite digunakan untuk mengklasifikasikan hasil pertarungan menjadi:  
- KO/TKO  
- Submission  
- Decision  

### 3. Summarization dengan IBM Granite  
Hasil klasifikasi kemudian diringkas untuk menemukan insight utama dengan bantuan Granite.  

---

## Insight & Findings  
Berikut beberapa insight awal dari analisis UFC:  

| Insight | Penjelasan |
|---------|------------|
| KO/TKO dominan | Kemenangan KO/TKO paling sering muncul di kelas berat. |
| Submission lebih sering di kelas ringan | Terutama terjadi pada pertarungan wanita dan kelas bawah. |
| Round awal krusial | Banyak pertarungan selesai di round 1–2 melalui KO/TKO. |

---

## 🤖 AI Support Explanation  
Analisis ini didukung oleh LLM IBM Granite (via Replicate API) yang digunakan untuk:  
- Mengklasifikasikan teks hasil pertarungan.  
- Membuat ringkasan insight berdasarkan hasil klasifikasi.  
