<h1 align="center">Hai, saya Dita 👋</h1>

<p align="center">
  <b>Data & AI Engineer</b> — membangun agent berbasis LLM, dashboard analitik, dan model prediktif.
</p>

<p align="center">
  Di bawah ini beberapa project pilihan. <b>Demo bisa langsung dicoba</b> lewat tautan;
  kode sumber bersifat privat dan tersedia atas permintaan.
</p>

---

## 🚀 Project Pilihan

### 1. 📊 Media Intelligence Dashboard
Dashboard interaktif untuk memantau dan menganalisis percakapan media sosial —
tren topik, sentimen, dan aktivitas akun dalam satu tampilan.

- **Tech**: Dashboard analitik · Visualisasi data · Web app
- **🔗 Demo langsung**: <https://mediaintelligence.netlify.app/>

> **Cara coba**: buka tautan, jelajahi filter & grafik untuk melihat ringkasan tren dan sentimen secara real-time.

---

### 2. 📈 Inflation Prediction
Aplikasi prediksi inflasi berbasis model machine learning, menampilkan proyeksi
angka inflasi beserta visualisasinya agar mudah dipahami.

- **Tech**: Machine Learning · Time-series forecasting · Web app
- **🔗 Demo langsung**: <https://prediction-inflation.netlify.app/>

> **Cara coba**: buka tautan, masukkan parameter/periode untuk melihat proyeksi inflasi dan grafiknya.

---

### 3. 🤖 Summary Agent (LLM API)
REST API yang meringkas **data apa pun** (berbentuk JSON) menjadi ringkasan rapi
menggunakan LLM. Bisa diarahkan fokus, format, dan bahasanya.

- **Tech**: FastAPI · LangChain · LLM `gpt-oss-20b` via Groq · Docker · Hugging Face Spaces
- **🔗 Demo langsung (Swagger UI)**: <https://ditash-summary-agent.hf.space/docs>

<details>
<summary><b>📥 Contoh penggunaan (klik untuk buka)</b></summary>

**Request:**
```bash
curl -X POST https://ditash-summary-agent.hf.space/api/v1/summarize \
  -H "Content-Type: application/json" \
  -d '{
    "data": {
      "judul": "Laporan Penjualan Q2 2026",
      "total_penjualan": 1850000000,
      "pertumbuhan_yoy": 0.23,
      "produk_terlaris": "Paket Pro",
      "catatan": "churn pelanggan Basic naik jadi 6%"
    },
    "instruction": "Ringkas 1 paragraf + 2 insight",
    "language": "Indonesian"
  }'
```

**Response:**
```json
{
  "metaData": { "status": true, "message": "OK", "timeExecution": "0.369" },
  "data": "**Laporan Penjualan Q2 2026** menunjukkan total penjualan mencapai **Rp1.850.000.000** dengan pertumbuhan tahunan **23%**. Produk **Paket Pro** menjadi terlaris, sementara catatan penting menyoroti kenaikan churn pelanggan **Basic** menjadi **6%**.\n\n**Insight 1:** Pertumbuhan 23% menandakan performa penjualan yang kuat, namun peningkatan churn Basic mengindikasikan risiko retensi pelanggan yang perlu diatasi.\n**Insight 2:** Dominasi Paket Pro sebagai produk terlaris memberi peluang memperluas penawaran premium dan meningkatkan margin."
}
```

</details>

---

## 🛠️ Tech Stack

`Python` · `FastAPI` · `LangChain` · `LLM / Groq` · `Machine Learning` ·
`Time-series Forecasting` · `Data Visualization` · `Docker` · `Hugging Face Spaces` · `Netlify`

---

## 📫 Kontak

- GitHub: [@ditashahihah](https://github.com/ditashahihah)

<sub>Demo di atas gratis dihosting; API LLM bisa "tidur" saat idle dan butuh beberapa detik untuk bangun pada request pertama.</sub>
