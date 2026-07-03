# Portofolio Pribadi & Studi Kasus Konsultasi Bisnis

Situs statis (HTML/CSS/JS vanilla, tanpa framework) yang berisi **portofolio pribadi**
sebagai konsultan sistem & digitalisasi bisnis, sekaligus sebuah **studi kasus konsultasi**
nyata: analisis peluang digitalisasi untuk **PT Weleri Bersaudara Semesta (PT WBS)**,
sebuah reseller alat kesehatan diagnostik B2B.

## Isi Situs

| Halaman | Keterangan |
|---|---|
| `index.html` | Landing page — nama, tagline, dan navigasi ke halaman lain. |
| `tentang.html` | Kerangka CV (skill, pengalaman, pendidikan). **Masih berisi placeholder `ISI DI SINI`** yang perlu diisi. |
| `studi-kasus-wbs.html` | Studi kasus PT WBS: ringkasan eksekutif, status verifikasi data, profil bisnis, temuan data stok (tabel + chart), peta risiko, rencana bertahap, faktor non-teknis, dan rekomendasi. |
| `style.css` | Desain B2B profesional, palet **navy + gold**, responsive mobile. |

## Teknologi

- HTML5, CSS3 (tanpa framework), JavaScript vanilla.
- [Chart.js](https://www.chartjs.org/) via CDN untuk grafik data stok (kombinasi bar + line).
- Tidak butuh proses build — cukup buka file HTML di browser.

## Menjalankan Secara Lokal

Karena situs statis murni, cukup buka `index.html` di browser. Di Windows PowerShell:

```powershell
start index.html
```

Atau (opsional) jalankan server lokal ringan agar path relatif konsisten:

```powershell
# butuh Python
python -m http.server 8000
# lalu buka http://localhost:8000 di browser
```

## Catatan Penting

- **Placeholder identitas:** teks `[NAMA ANDA]`, `[TAGLINE ANDA]`, dan `ISI DI SINI`
  sengaja dibiarkan kosong. Ganti dengan data faktual Anda sendiri — halaman CV
  tidak diisi dengan klaim yang tidak dapat didukung.
- **Transparansi data studi kasus:** dokumen studi kasus membedakan secara eksplisit
  antara data yang **terverifikasi** dan klaim yang **belum diverifikasi independen**
  (mis. angka omset dan kelengkapan izin edar/PAK). Pembedaan ini dipertahankan di situs.
- **Sumber data:** studi kasus disusun dari dokumen analisis internal
  (`Analisis_Peluang_PT_WBS.docx`) yang menggabungkan riset web terbatas, file stok
  internal, dan keterangan pihak internal perusahaan.

---

Dibuat sebagai portofolio pribadi + demonstrasi pendekatan konsultasi digitalisasi
yang realistis, bertahap, dan berbasis data.
