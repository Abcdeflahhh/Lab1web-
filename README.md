# Lab1web-

MEMBUAT MODUL PRAKTIKUM PEMROGRAMAN WEB

NAMA : AFLAH ATHALLAH TAMAM KAPUKONG

NIM : 312410280

KELAS : TI.24.A.4

MATKUL : PEMROGRAMAN WEB 1

1. Deklarasi DOCTYPE

<!DOCTYPE html>

Fungsi: Ini adalah deklarasi tipe dokumen (Document Type Declaration) yang memberi tahu browser bahwa dokumen ini menggunakan standar HTML5. DOCTYPE harus berada di baris pertama dan tidak boleh ada spasi atau komentar sebelumnya.

Catatan: Tanpa ini, browser mungkin merender halaman dalam mode "quirks" (kompatibilitas lama), yang bisa menyebabkan tampilan tidak konsisten. Ini adalah elemen wajib untuk HTML modern.

2. Elemen Root <html>

<html lang="en">

Fungsi: Ini adalah elemen root (akar) dari seluruh dokumen HTML. Semua elemen lain harus berada di dalamnya. Atribut lang="en" menentukan bahasa default halaman (dalam hal ini, bahasa Inggris), yang membantu screen reader, mesin pencari, dan SEO.

Catatan: Tag penutupnya adalah </html> di akhir dokumen. Atribut lang sebaiknya disesuaikan dengan konten (misalnya, lang="id" untuk bahasa Indonesia, karena teks di body menggunakan bahasa Indonesia).

3. Elemen <head>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Praktikum1 - HTML DASAR</title>
    <link rel="stylesheet" href="style.css">
</head>

Fungsi: Bagian <head> berisi metadata dan informasi non-visual tentang halaman. Ini tidak ditampilkan di body, tapi penting untuk browser dan mesin pencari.
<meta charset="UTF-8">: Menentukan encoding karakter (UTF-8), yang mendukung karakter internasional seperti aksara Latin, emoji, dll. Ini mencegah masalah tampilan teks aneh.
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Mengoptimalkan tampilan untuk perangkat mobile. width=device-width menyesuaikan lebar layar, dan initial-scale=1.0 mencegah zoom otomatis.
<title>Praktikum1 - HTML DASAR</title>: Judul halaman yang muncul di tab browser atau hasil pencarian. Ini penting untuk SEO dan identifikasi halaman.
<link rel="stylesheet" href="style.css">: Menghubungkan file CSS eksternal (style.css) untuk styling (seperti warna, font, layout). Atribut rel="stylesheet" menandakan ini adalah stylesheet, dan href adalah path file.
Catatan: Semua elemen di <head> bersifat opsional kecuali <title>, tapi direkomendasikan. Tag penutup </head> menutup bagian ini.

4. Elemen <body>

Fungsi: Bagian <body> berisi semua konten yang terlihat oleh pengguna, seperti teks, gambar, link, dan elemen interaktif. Ini adalah "tubuh" utama halaman web.
Catatan: Tag penutup </body> berada di akhir dokumen. Di dalamnya, ada berbagai elemen yang akan saya jelaskan selanjutnya. Secara keseluruhan, body ini mencakup navigasi, heading, paragraf, dan gambar untuk membuat halaman sederhana tentang pembelajaran HTML.

4.1. Navigasi Pertama (<nav>)

<nav>
    <a href="lab1_tag_dasar.html">DASAR HTML</a>
    <a href="lab1_halaman2.html">HALAMAN 2</a>
    <a href="https://www.google.com">HALAMAN EKSTERNAL GOOGLE.COM</a>
</nav>

Fungsi: Elemen <nav> digunakan untuk blok navigasi (menu atau link utama). Di dalamnya, ada tiga elemen <a> (anchor/link):
<a href="lab1_tag_dasar.html">DASAR HTML</a>: Link internal ke file lokal lab1_tag_dasar.html dengan teks "DASAR HTML".
<a href="lab1_halaman2.html">HALAMAN 2</a>: Link internal ke file lokal lab1_halaman2.html dengan teks "HALAMAN 2".
<a href="https://www.google.com">HALAMAN EKSTERNAL GOOGLE.COM</a>: Link eksternal ke situs Google dengan teks "HALAMAN EKSTERNAL GOOGLE.COM". Atribut href menentukan tujuan link (URL atau path file).
Catatan: <nav> bersifat semantik (memberi makna struktural), yang baik untuk aksesibilitas. Link ini akan muncul sebagai menu horizontal atau vertikal tergantung CSS. Tidak ada tag penutup eksplisit untuk setiap <a>, tapi setiap <a> sudah ditutup dengan benar.

4.2. Paragraf dengan Header dan Heading (<p>, <header>, <h1>)

<p>
    <header>
        <h1>
            DAY 1 - BELAJAR HTML
        </h1>
    </header>
</p>

Fungsi:
<p>: Elemen paragraf untuk teks blok. Di sini, ia membungkus header.
<header>: Elemen semantik untuk pengantar atau header halaman (seperti banner atas). Biasanya berisi logo atau judul utama.
<h1>: Heading level 1 (judul utama). Teks "DAY 1 - BELAJAR HTML" akan ditampilkan besar dan bold, menandakan topik utama halaman.
Catatan: Struktur ini tidak ideal secara semantik—<header> sebaiknya berada di luar <p>, karena header adalah elemen independen, bukan bagian dari paragraf. Ini bisa membingungkan screen reader. Sebaiknya gunakan <header><h1>...</h1></header> langsung di body tanpa membungkusnya dalam <p>.

4.3. Paragraf Kedua (<P>)

<P>
    Saya sedang belajar HTML dasar, pada matakuliah Pemrograman Web di Prodi
    Teknik Informatika Universitas Pelita Bangsa. Pelajaran pertama yang kami dapat
    adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar
    HTML
</P>

Fungsi: <P> (sama dengan <p>, meskipun huruf besar—HTML tidak case-sensitive untuk tag) adalah elemen paragraf yang menampilkan teks panjang sebagai blok. Teks ini menjelaskan konteks pembelajaran.
Catatan: Gunakan huruf kecil (<p>) untuk konsistensi. Paragraf ini akan memiliki margin otomatis dari browser untuk pemisahan visual.

4.4. Paragraf dengan Heading Level 2 (<p>, <h2>)

<p>
    <h2>
        HI, Aku Aflah AThallah Tamam Kapukong
    </h2>
</p>

Fungsi:
<p>: Membungkus heading.
<h2>: Heading level 2 (sub-judul). Teks "HI, Aku Aflah AThallah Tamam Kapukong" akan lebih kecil dari <h1> tapi masih menonjol.
Catatan: Lagi-lagi, membungkus <h2> dalam <p> tidak semantik—heading sebaiknya berdiri sendiri. Ini bisa menyebabkan masalah styling atau aksesibilitas.

4.5. Paragraf Ketiga (<p>)

<p>
    Saya merupakan mahasiswa semester 3 di Universitas Pelita Bangsa, Jurusan Teknik Informatika
</p>

Fungsi: Paragraf sederhana dengan teks deskripsi diri. Ditampilkan sebagai blok teks biasa.
Catatan: Struktur yang baik dan sederhana.

4.6. Paragraf dengan Heading Level 3 (<P>, <h3>)

<P>
    <h3>
        LOGO KAMPUS UPB
    </h3>
</P>

Fungsi:
<P>: Membungkus heading.
<h3>: Heading level 3 (sub-sub-judul). Teks "LOGO KAMPUS UPB" menyiapkan konteks untuk gambar berikutnya.
Catatan: Sama seperti sebelumnya, hindari membungkus heading dalam paragraf. Ini lebih baik sebagai <h3> mandiri diikuti gambar.

4.7. Elemen Gambar (<img>)

<img src="UPB.jpg" alt="LOGO Universitas Pelita Bangsa">

Fungsi: <img> menyisipkan gambar. Atribut:
src="UPB.jpg": Path file gambar lokal (harus ada di folder yang sama dengan HTML).
alt="LOGO Universitas Pelita Bangsa": Teks alternatif untuk aksesibilitas (baca screen reader jika gambar gagal dimuat) dan SEO.
Catatan: Gambar akan ditampilkan inline. Jika file UPB.jpg tidak ditemukan, browser akan menampilkan placeholder dengan teks alt. Tambahkan atribut seperti width atau height untuk kontrol ukuran jika diperlukan.

4.8. Navigasi Kedua (<nav>)

<nav>
    <a href="https://pb.ecampus.id/pb/main">Universitas Pelita Bangsa</a>
</nav>

Fungsi: Blok navigasi lain dengan satu link eksternal ke situs e-campus Universitas Pelita Bangsa. <a> berfungsi seperti sebelumnya.
Catatan: Menggunakan <nav> lagi untuk link tunggal mungkin berlebihan; bisa diganti dengan <p> atau elemen lain jika bukan menu utama. Ini menambah link ke bawah halaman.

Kesimpulan Umum
Struktur Keseluruhan: Dokumen ini mengikuti struktur HTML dasar (DOCTYPE > html > head > body), tapi ada isu semantik seperti penempatan <header>, <h1>, <h2>, dan <h3> di dalam <p>. Ini bisa diperbaiki untuk membuat kode lebih bersih dan aksesibel (misalnya, gunakan outline heading yang logis: h1 > h2 > h3).
Tujuan: Halaman ini tampaknya untuk praktikum pembelajaran HTML, menampilkan teks pengenalan, link, dan gambar logo kampus.
Saran Perbaikan:
Validasi kode dengan tools seperti W3C Validator untuk cek kesalahan.
Tambahkan tag penutup yang konsisten (semua sudah ada, tapi perhatikan case).
Gunakan CSS (dari style.css) untuk styling lebih lanjut, seperti membuat nav horizontal.
Pastikan file gambar dan CSS ada di lokasi yang benar agar halaman render sempurna.
