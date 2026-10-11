---
name: gerbang-gaya-cek-gaya-ai
description: Aturan keras anti gaya AI plus pemeriksa cek_gaya_ai.py; Tristan minta ini jadi gerbang untuk setiap teks yang saya tulis di proyek abroad
metadata: 
  node_type: memory
  type: feedback
  originSessionId: 46d76093-5d82-4100-9f1f-90f77dd5ec17
  modified: 2026-09-18T20:57:51.831Z
---

Tristan menyuruh saya membawa gerbang gaya dari proyek `general-ai` ke sini dan memakainya untuk
**setiap** tulisan, termasuk email, surat, dokumen sekolah, dan lampiran paper. Dua bagian:

1. **Aturannya**, aslinya memori `gaya-tulisan-anti-ai` di proyek `general-ai` dan
   `research-startup`, hasil risetnya sendiri 18 September 2026.
2. **Pemeriksanya**, `cek_gaya_ai.py`, 237 baris, sudah disalin ke
   `Downloads/to abroad/cek_gaya_ai.py`. Jalankan `py cek_gaya_ai.py berkas.txt`, keluar 0 kalau
   lolos.

Dia menyimpan aturan ini "secara keras". Sebelum menyerahkan tulisan apa pun, jalankan pemeriksanya
dan perbaiki setiap temuan aturan keras sampai nol.

## A. Konstruksi terlarang, target nol

1. **Paralelisme negatif.** `bukan X melainkan Y`, `bukan X tetapi Y`, `tidak hanya X tetapi juga
   Y`, `bukan sekadar`, `X, bukan Y` sebagai hiasan. Bahasa Inggris: `not only`, `but also`,
   `it is not X it is Y`, dan `rather than`. Tulis Y langsung. Kalau kontrasnya memang temuannya,
   pecah jadi dua kalimat afirmatif: "Proposal memperkirakan X. Pengukuran menghasilkan Y."
2. **Ekor partisipial penegas.** `, menegaskan`, `, mencerminkan`, `, menyoroti`, `, menandai`;
   Inggris `, highlighting`, `, underscoring`, `, demonstrating the`. Ganti dengan kalimat yang
   menyebut angkanya.
3. **Pertanyaan retoris yang dijawab sendiri.** "Hasilnya? ...", "Mengapa ini penting? Karena ..."
4. **Penutup paragraf bergaya kata mutiara** atau kesimpulan moral. Wikipedia menyebutnya
   "section summaries". Pemeriksanya tidak menangkap ini; saya yang harus menangkapnya. Saya
   pernah melakukannya tiga kali dalam satu surat 790 kata.
5. **Frasa pengisi.** `perlu dicatat bahwa`, `penting untuk dicatat`, `pada dasarnya`,
   `singkatnya`, `pada akhirnya`, `secara keseluruhan`, `mari kita`, `di era digital saat ini`;
   Inggris `it is important to note`, `in conclusion`, `moreover`, `furthermore`, `additionally`,
   `ultimately`, `overall`.
6. **Kosakata pembesar makna.** `krusial`, `memainkan peran penting`, `menjadi bukti nyata`,
   `tonggak`, `lanskap`, `ranah`, `menavigasi`, `menggali lebih dalam`, `mengeksplorasi`,
   `memberdayakan`, `holistik`, `revolusioner`, `transformatif`, `mulus`, `sinergi`,
   `paradigma baru`, `mutakhir` sebagai pujian. Inggris: delve, tapestry, testament, pivotal,
   crucial, intricate, meticulous, showcase, underscore, landscape, realm, vibrant, boasts,
   garner, foster, seamless, holistic, groundbreaking, leverage, embark, navigate, multifaceted,
   nuanced.
7. **Suara penulis dan penjilat.** "pertanyaan bagus", sapaan ke pembaca, "kami harap".
8. **Atribusi kabur.** `para ahli berpendapat`, `banyak penelitian menunjukkan`.
9. **Tanda pisah panjang dan sedang** sebagai pemutus klausa. Pakai koma, titik, titik dua, atau
   kurung. Rentang angka di prosa: `sampai` atau `hingga`.
10. **Emoji, panah di prosa**, subjudul berhuruf kapital tiap kata di luar konvensi naskah.
11. **Kopula yang dihindari.** Pakai `is` dan `are` apa adanya. Jangan `serves as`, `stands as`,
    `functions as`, `represents`, `boasts`, `features`. Jangan pula `is a testament to`,
    `underscores the importance`, `plays a crucial role`, `marks a shift`, `evolving landscape`.

## B. Aturan lunak, berjatah per sepuluh ribu kata

Tricolon jangan otomatis; pakai jumlah butir yang sebenarnya. Jatah pemeriksanya: `merupakan` 14,
`sangat` 12, `hal ini` 8, `berbagai` 8, `selain itu` 6, `oleh karena itu` 5, `signifikan` 4,
`lebih lanjut` 4, `dengan demikian` 3, `komprehensif` 1. Hindari juga cetak tebal berlebihan,
daftar berpoin yang menggantikan paragraf, dan bagian boilerplate semacam "Tantangan dan Prospek
Masa Depan".

**Ambang ritme.** Koefisien variasi panjang kalimat harus **≥ 0,35**. Kalimat AI cenderung seragam
panjangnya, dan angka inilah yang menangkapnya.

## C. Isi

Setiap klaim dapat dilacak ke angka, berkas, atau sumber. Rujukan hanya yang benar ada dan sudah
diverifikasi; jangan mengarang DOI, halaman, atau statistik sekolah. Istilah teknis didefinisikan
saat pertama muncul tanpa disederhanakan berlebihan.

## Dua aturan yang saya perlakukan sebagai khusus dokumen

Saya sampaikan terbuka ke dia, bukan diputuskan diam-diam:

- **`**` dan backtick** ditandai pemeriksanya sebagai sisa markdown. Benar untuk prosa yang masuk
  PDF. Di jendela obrolan markdown justru dirender dan membantu keterbacaan.
- **`anda` dan `kita`** ditandai sebagai suara penulis. Tepat untuk dokumen formal. Dalam
  percakapan dengan dia saya memakai `kamu`, dan `kita` merujuk kerja bersama yang nyata.

Selebihnya berlaku penuh, termasuk di jendela obrolan.

**Why:** surat rekomendasi dan esai lamaran dibaca panitia penerimaan yang melihat ribuan berkas
per musim dan sudah mengenali pola ini pada 2026, jadi tulisan yang terbaca sebagai mesin
merugikan Tristan langsung. Audit di proyek `general-ai` menemukan tulisan saya sendiri memakai
`bukan X, melainkan Y` lima puluh kali. Di sini saya menulis tiga surat rekomendasi yang memakai
mesin retorika yang sama, sehingga ketiganya terbaca sebagai satu tangan. Saya rawan terhadap pola
ini dan tidak boleh mengandalkan kesan sendiri.

**How to apply:** untuk dokumen, email, surat, dan lampiran, jalankan pemeriksanya sebelum
menyerahkan. Untuk jawaban obrolan yang panjang, periksa terhadap daftar A. Saat menulis beberapa
dokumen yang seolah dari orang berbeda, beri tiap orang irama kalimat yang berbeda, bukan hanya
isi yang berbeda. Sumber risetnya:
Wikipedia "Signs of AI writing"; Kobak dkk. 2024 arXiv 2406.07016; Liang dkk. ICML 2024
(meticulous 34,7x, intricate 11,2x); Reinhart dkk. PNAS 2025; Freeburg 2026 arXiv 2603.27006
(em dash per seribu kata: GPT-4.1 10,62, Claude Opus 4.6 9,09, manusia 3,23). Lihat juga
[[prose-no-ai-tics]], [[tristan-email-register]], dan [[tristan-email-structure]].
