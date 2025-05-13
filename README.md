# 🌍 World Population Insights: Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Status-Active-green)
![License](https://img.shields.io/badge/License-MIT-green)

## 📖 Overview

Ini adalah proyek **Exploratory Data Analysis (EDA)** yang mengeksplorasi tren populasi dunia berdasarkan dataset `world_population2024.csv`.  
Analisis ini mencakup **pembersihan data**, **deteksi outlier**, **korelasi antar variabel**, dan **dimensionality reduction** menggunakan **Principal Component Analysis (PCA)**.

📊 **Disajikan dalam:** Digital Skill Fair 39.0  
📄 **Dokumen Pendukung:** [`EDA_Portfolio.pptx`](./EDA_Portfolio.pptx)

---

## 📂 Project Structure

```plaintext
.
├── data
│   └── world_population2024.csv
├── notebooks
│   └── EDA_World_Population.ipynb
├── presentation
│   └── EDA_Portfolio.pptx
├── src
│   └── eda_analysis.py
└── README.md
```

---

## 📊 Dataset Information

- **File:** `world_population2024.csv`
- **Size:** 216 rows × 12 columns
- **Key Columns:**
  - `Rank`
  - `Country (or dependency)`
  - `Population (2024)`
  - `Yearly Change`
  - `Net Change`
  - `Density (P/km^2)`
  - `Land Area (Km^2)`
  - `Migrants (net)`
  - `Fert. Rate`
  - `Med. Age`
  - `Urban Pop %`
  - `World Share`

---

## 🔍 Exploratory Data Analysis (EDA)

<details>
  <summary>Click to Expand</summary>

### **Libraries Used**
- `pandas`, `numpy` → Data processing  
- `matplotlib`, `seaborn` → Visualization  
- `sklearn` → PCA & StandardScaler  

### **Data Cleaning**
✔️ **Tidak ada missing values**  
✔️ **Tidak ada data duplikat**  
✔️ **Dataset siap untuk analisis lanjut**  

### **Outlier Analysis**
| Kolom           | Jumlah Outlier | Persentase |
|----------------|--------------|------------|
| Yearly Change | 5            | 2.31%      |
| Fert. Rate    | 5            | 2.31%      |
| World Share   | 23           | 10.65%     |

### **Correlation Analysis**
Variabel dengan korelasi kuat:
- **Fert. Rate** & **Med. Age** → r = **-0.87** (negatif kuat)

### **Principal Component Analysis (PCA)**
- **Total variansi dijelaskan oleh 2 komponen pertama:** **71.26%**
- **Variabel utama dalam PCA:**  
  `Rank`, `Fert. Rate`, `Med. Age`, `Urban Pop %`, `World Share`

</details>

---

## 📌 Recommendations & Next Steps

🔍 **Analisis Lanjutan:**
| Area Analisis | Rekomendasi |
|--------------|------------|
| Korelasi | Investigasi hubungan antar variabel |
| Segmentasi | Identifikasi karakteristik tiap kelompok |
| Outlier | Evaluasi apakah outlier merupakan fenomena alami atau kesalahan data |
| Time Series | Analisis tren populasi dari waktu ke waktu |
| Clustering | Gunakan K-Means untuk mencari pola |
| Predictive Modeling | Bangun model prediktif berdasarkan hasil EDA |

---

## 🚀 Getting Started

### **Prerequisites**
- **Python 3.x**  
- Install libraries yang dibutuhkan:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
  ```

### **Running the Analysis**
Gunakan script Python atau Jupyter Notebook:
```bash
python src/eda_analysis.py
```

---

## 📩 Contact

📧 Email: [febrianto078@gmail.com](mailto:febrianto078@gmail.com)  
💻 GitHub: [github.com/FBTO45](https://github.com/FBTO45)  
🔗 LinkedIn: [Febrianto](https://www.linkedin.com/in/febrianto/)  

---

🔹 **Silakan eksplor, kontribusi, atau berikan feedback pada proyek ini!**
```

---

### 🚀 **Enhancements in This Version:**
✅ **Lebih rapi & profesional**  
✅ **Menggunakan badge & emoji untuk tampilan menarik**  
✅ **Menambahkan collapsible sections** untuk bagian yang panjang  
✅ **Format tabel lebih informatif**  
✅ **Link ke kontak & proyek GitHub**  

README ini siap untuk diunggah ke repositori **GitHub** Anda!  
Apakah ada detail tambahan yang ingin Anda masukkan? 🚀😃
