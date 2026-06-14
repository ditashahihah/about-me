<h1 align="center">Dita Shahihah</h1>

<p align="center">
  <b>Data Scientist</b>
</p>

<p align="center">
  Data Scientist dengan 3+ tahun pengalaman membangun <b>aplikasi berbasis AI</b>, solusi
  <b>analitik data</b>, dan <b>dashboard interaktif</b> untuk klien segmen politik, korporat,
  dan pemerintahan. Berpengalaman dalam AI-assisted development dengan Python &amp; LLM untuk
  mengotomasi alur riset dan analitik, serta predictive modeling, sentiment analysis, dan
  ETL pipeline engineering.
</p>

<p align="center">
  Beberapa project pilihan di bawah ini — <b>demo bisa langsung dicoba</b> lewat tautan;
  kode sumber bersifat privat dan tersedia atas permintaan.
</p>

---

## Project Pilihan

### 1. Media Intelligence Dashboard
Platform dashboard interaktif yang dapat dikonfigurasi untuk klien **politik, korporat, dan
pemerintahan** dari satu basis kode. Menyajikan metrik media &amp; analitik secara real-time di
atas **Elasticsearch**, dengan komponen visualisasi **custom HTML/CSS/SQL** yang disesuaikan
per segmen klien, dan terintegrasi otomatis dengan **ETL pipeline**.

- **Tech**: HTML/CSS · SQL · Elasticsearch · Data Visualization · Web App
- **Demo langsung**: <https://mediaintelligence.netlify.app/>

> **Cara coba**: buka tautan, jelajahi filter &amp; grafik untuk melihat metrik media dan sentimen secara real-time.

---

### 2. Public Sentiment-Based Inflation Prediction
Sistem prediktif **end-to-end** yang menggabungkan **sentimen media sosial real-time** dengan
**indikator makroekonomi historis** untuk memproyeksikan pergerakan inflasi jangka pendek.
Dibangun dengan **pipeline NLP** ekstraksi sentimen (mengubah teks tak terstruktur jadi sinyal
sentimen harian) dan **model regresi**, divalidasi terhadap data inflasi historis, lalu
ditampilkan lewat dashboard interaktif.

- **Tech**: Machine Learning · NLP · Time-series Forecasting · Web App
- **Demo langsung**: <https://prediction-inflation.netlify.app/>

> **Cara coba**: buka tautan untuk melihat proyeksi inflasi beserta visualisasinya.

---

### 3. Summary Agent (LLM API)
**Analytics API** berbasis LLM yang meringkas **data apa pun** (berbentuk JSON) menjadi
ringkasan rapi dan terstruktur. Fokus, format, dan bahasa keluaran dapat dikonfigurasi.
Dibangun mengikuti pola integrasi LLM (prompt engineering, structured output) dan di-deploy
sebagai REST API publik.

- **Tech**: FastAPI · LangChain · LLM `gpt-oss-20b` via Groq · Docker · Hugging Face Spaces
- **Demo langsung (Swagger UI)**: <https://ditash-summary-agent.hf.space/docs>

<details>
<summary><b>Contoh penggunaan (klik untuk buka)</b></summary>

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

## Tech Stack

**Bahasa &amp; Dev**: `Python` · `SQL` · `HTML/CSS` · `REST API`
**AI &amp; LLM**: `LLM Integration` · `Prompt Engineering` · `NLP` · `AI-Assisted Development`
**Data &amp; ML**: `Sentiment Analysis` · `Predictive Modeling` · `Time-series Forecasting` · `ETL Pipelines` · `Elasticsearch`
**Visualisasi &amp; Deploy**: `Pandas` · `Matplotlib` · `Custom Dashboards` · `Docker` · `Hugging Face Spaces` · `Netlify`

---

## Pendidikan
**S1 Informatika (S.Kom)** — Universitas Jember · IPK 3.56/4.00

## Kontak
- LinkedIn: [dita-shahihah](https://linkedin.com/in/dita-shahihah)
- Email: ditashahihah@gmail.com
- GitHub: [@ditashahihah](https://github.com/ditashahihah)

<sub>Demo di atas gratis dihosting; API LLM bisa "tidur" saat idle dan butuh beberapa detik untuk bangun pada request pertama.</sub>
