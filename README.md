# Ca · SSA-Nyala — Streamlit

Aplikasi pembelajaran **Gangguan Analisis Ca pada Spektrofotometri Serapan Atom-Nyala (AAS)**.

## Isi repository
- `app.py` — aplikasi pembuka Streamlit.
- `index.html` — antarmuka dan logika interaktif aplikasi asli.
- `requirements.txt` — dependensi Python.

## Jalankan di komputer sendiri
1. Pasang Python 3.10 atau lebih baru.
2. Buka terminal pada folder proyek.
3. Buat virtual environment (opsional tetapi disarankan):
   ```bash
   python -m venv .venv
   ```
4. Aktifkan environment:
   - Windows: `.venv\\Scripts\\activate`
   - macOS/Linux: `source .venv/bin/activate`
5. Instal dependensi:
   ```bash
   pip install -r requirements.txt
   ```
6. Jalankan aplikasi:
   ```bash
   streamlit run app.py
   ```
7. Buka URL lokal yang ditampilkan di terminal, biasanya `http://localhost:8501`.

## Publikasikan melalui GitHub dan Streamlit Community Cloud
1. Masuk/daftar di GitHub, lalu buat repository baru, misalnya `aas-ca-ssa-nyala`.
2. Unggah **ketiga file**: `app.py`, `index.html`, dan `requirements.txt` (README juga boleh diunggah).
3. Pastikan `app.py` berada di folder utama repository, bukan di dalam subfolder.
4. Buka https://share.streamlit.io/ dan masuk menggunakan akun GitHub.
5. Pilih **Create app** / **Deploy an app**.
6. Pilih repository `aas-ca-ssa-nyala`, branch `main`, dan file utama `app.py`.
7. Klik **Deploy** dan tunggu proses instalasi selesai.
8. Setelah selesai, Streamlit akan memberikan URL aplikasi yang bisa dibagikan.

## Catatan
- Model 3D menggunakan Three.js dari CDN, jadi fitur tersebut memerlukan koneksi internet.
- Aplikasi HTML berjalan di dalam komponen iframe Streamlit. Gulir di area aplikasi untuk melihat seluruh bagian; jika ingin ruang tampilan lebih tinggi, ubah `height=1100` di `app.py`.
- Data awal pada aplikasi HTML merupakan data contoh. Ganti dengan data praktikum yang sebenarnya sebelum digunakan untuk laporan.
- Setelah mengubah file, unggah/commit perubahan ke GitHub. Streamlit Cloud biasanya akan memperbarui aplikasi secara otomatis.
