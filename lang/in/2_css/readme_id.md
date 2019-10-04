# Cascade style sheets (CSS)

## Mengapa bernama demikian?

Cascading Style Sheets terutama disebut sebagai CSS, adalah bahasa desain sederhana yang dimaksudkan untuk menyederhanakan proses pembuatan halaman web yang menarik. Menggunakan CSS, Anda dapat mengontrol tata letak halaman web, ukuran font, dan warna, variasi untuk tampilan (untuk perangkat dan ukuran layar yang berbeda) serta berbagai efek lainnya. CSS mudah dipelajari dan dipahami karena memberikan kontrol yang kuat atas penyajian dokumen HTML.

## Sintaks CSS

#### Definisi

File CSS dilambangkan dengan ekstensi `.css` dan biasanya, namanya mengacu pada halaman web yang mereka tangani. Misalnya `about.css` kemungkinan besar akan berisi semua gaya yang ingin Anda terapkan ke halaman about Anda.

CSS memiliki sintaks yang cantik dan ringkas

1) Aturan harus dimasukkan dalam `{}`

2) Mereka mengikuti pola: `properti: nilai;` (di mana `;` hanya diperlukan saat menambahkan beberapa aturan)

Sebagai contoh jika kita memiliki aturan yang hanya menerapkan warna pada teks yang diberikan, tidak perlu menambahkan `;` di akhir baris.

``` CSS
.text-gray {
    color: #323232
}
```
Sebaliknya...

``` CSS
.main-wrapper {
     color: #323232;
     font-size: 16px;
     line-height: 1.6;
     text-decoration: none;
}
```

Setelah mengikuti Anda dapat melihat pada contoh sebelumnya bahwa saya ingin memiliki `main-wrapper` saya

- Warna # 323232 yang seperti abu-abu gelap sedang
- ukuran font 16px
- line-height (yang merupakan ruang yang memisahkan teks secara vertikal di antara garis-garis) dan membantu pemahaman bacaan.
- Dan dekorasi teks diatur ke `tidak ada` (untuk menghapus gaya tambahan seperti garis bawah, garis atas, dll.)

Aturan ini hanya berlaku untuk `. Main-wrapper`, yang merupakan pemilih kelas (kami akan menjelaskan pemilih kelas apa yang lebih lanjut di bagian selanjutnya)

#### Membentuk

Ada dua cara penulisan CSS

- Inline: Itu dianggap praktik buruk karena tidak bisa dibaca oleh manusia.
``` CSS
.main-wrapper { color: #323232; font-size: 16px; line-height: 1.6; text-decoration: none; } 
```
- block: <strong> Sangat dianjurkan </strong> untuk mudah dibaca manusia
``` CSS
.main-wrapper {
     color: #323232;
     font-size: 16px;
     line-height: 1.6;
     text-decoration: none;
}
```
#### Komentar

Komentar dimaksudkan untuk pemahaman kode yang lebih baik, ini adalah bagian dari kode yang tidak dieksekusi oleh komputer, dan dalam CSS ditulis dengan cara berikut:

``` CSS
/ Ini adalah komentar inline dan pendek
.main-wrapper {
   color: #323232;
   font-size: 16px;
   line-height: 1.6;
   text-decoration: none;
}

/* --------------------------------------------------
** Ini adalah komentar besar dan luas itu
** membutuhkan banyak baris untuk dapat dibaca dengan benar.
** --------------------------------------------------
*/
.main-wrapper {
   color: #323232;
   font-size: 16px;
   line-height: 1.6;
   text-decoration: none;
}
```
## Selektor dasar CSS
    Selektor CSS digunakan untuk memilih elemen HTML yang ingin kita gaya.
     Selektor dasar dalam CSS adalah sebagai berikut:
    
     1) Pemilih elemen: Memilih elemen HTML menggunakan namanya.
     2) pemilih ID: Memilih elemen HTML menggunakan atribut id mereka. Penggunaan: Hash (#) diikuti oleh id.
     3) Pemilih kelas: Memilih elemen HTML menggunakan nama kelas mereka. Penggunaan: Periode (.) Diikuti dengan nama kelas.
     4) Pemilih universal: Memilih semua elemen HTML di halaman. Penggunaan: Asterisk (*) digunakan sebagai pemilih universal
### Catatan tentang spesifisitas
    TODO
## Model Kotak
    TODO
