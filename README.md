# Kumpulan Web Tools

Kumpulan tools web gratis yang berjalan sepenuhnya di browser, tanpa server dan tanpa instalasi.

## Fitur
1. **Analisis Teks**: hitung kata, karakter, kalimat, paragraf, kata kunci, dan ubah format huruf.
2. **Manajemen Web**: encode/decode URL, minify HTML dan CSS.
3. **SEO & Backlink**: generator meta tag dengan validasi panjang, generator anchor link.
4. **Domain Tools**: cek record DNS (A, AAAA, MX, TXT, NS, CNAME) via Google DNS over HTTPS.
5. **Image Tools**: ubah ukuran dan format gambar (WebP, JPEG, PNG) di perangkat pengguna.
6. **Website Checker**: validasi URL dan cek keterjangkauan dengan timeout.
7. **PDF Converter**: teks ke PDF dan gambar ke PDF (memakai jsPDF).
8. **Konverter Unit**: panjang, berat, volume, ukuran data, dan suhu.
9. **Binary Translator**: teks, biner, dan hex (UTF-8).

## Cara Deploy ke GitHub Pages
1. Buat repository baru, misalnya `web-tools`.
2. Upload `index.html` dan `README.md` ke branch `main`.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**, lalu branch `main` dan folder `/ (root)`.
5. Tunggu beberapa menit. Situs aktif di `https://<username>.github.io/web-tools/`.

## Cara Menguji Lokal
Klik dua kali `index.html`, atau jalankan server lokal sederhana:
```bash
python -m http.server 8000
```
lalu buka `http://localhost:8000`.

## Catatan Keterbatasan
- Jumlah backlink, WHOIS, dan kode status HTTP membutuhkan server atau API pihak ketiga.
- Fitur PDF memuat jsPDF dari cdnjs, sehingga membutuhkan internet.
- Cek DNS dan Cek Website membutuhkan koneksi internet dan bisa gagal jika diblokir jaringan.

## Checklist Uji Sebelum Publikasi
- [ ] Konsol browser (F12) tidak menampilkan error merah.
- [ ] Navigasi berpindah antar tool dan kartu di Beranda berfungsi.
- [ ] Analisis teks: statistik berubah saat mengetik.
- [ ] Encode dan decode URL dengan karakter khusus (contoh: `a b&c=d`).
- [ ] Meta tag menampilkan peringatan panjang judul dan deskripsi.
- [ ] Cek DNS `google.com` tipe A menampilkan hasil.
- [ ] Unggah gambar JPG, proses, lalu unduh hasilnya.
- [ ] Cek website `https://github.com` menampilkan "Dapat dijangkau".
- [ ] Unduh PDF teks dan PDF gambar.
- [ ] Konversi 1 km ke mil menghasilkan 0,621371.
- [ ] Binary translator: `Halo` → biner → kembali ke `Halo`.
- [ ] Tampilan benar di HP dan mode gelap.
