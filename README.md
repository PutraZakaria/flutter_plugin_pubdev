# Pemrograman Mobile Minggu 7

<br>

## Nama: Putra Zakaria Muzaki
## Kelas: TI-3H / 19
## NIM: 2241720220

<br>


### Soal 1: Selesaikan Praktikum tersebut, lalu dokumentasikan dan push ke repository Anda berupa screenshot hasil pekerjaan beserta penjelasannya di file README.md!
![alt](image.png)

### Soal 2: Jelaskan maksud dari langkah 2 pada praktikum tersebut!
Pada langkah 2 dilakukan proses penambahan plugin auto_size_text kedalam pubspec.yaml melalui perintah flutter pub add auto_size_text pada terimnal agar plugin bisa digunakan dalam projek.

### Soal 3: Jelaskan maksud dari langkah 5 pada praktikum tersebut!
Pada langkah 5 terdapat proses pendeklarasian variabel item melalui code final String text; dimana final digunakan untuk mendeklarasikan variabel yang nilainya hanya bisa digunakan sekali. Variabel item akan menyimpan teks yang akan ditampilkan di widget, dan code required this.text menunjukan bahwa variabel ini harus diisikan pada saat memanggil function.

### Soal 4: Pada langkah 6 terdapat dua widget yang ditambahkan, jelaskan fungsi dan perbedaannya!
Fungsi dari dua container yang ditambahkan pada langkah 6 adalah untuk menampilkan teks dengan warna background dan lebar yang berbeda. Perbedaannya dari kedua container tersebut adalah untuk container pertama menggunakan plugin auto_size_text melalui widget RedTextWidget(), sehingga teks akan otomatis menyesuaikan ukurannya jika melebihi batas ruang yang tersedia. Sedangkan untuk container kedua menggunakan Text biasa tanpa menggunakan widget yang akan menampilkan teks dengan ukuran tetap, tanpa penyesuaian otomatis jika teks terlalu panjang.

### Soal 5: Jelaskan maksud dari tiap parameter yang ada di dalam plugin auto_size_text berdasarkan tautan pada dokumentasi ini !
1. key: Parameter ini digunakan untuk mengontrol bagaimana satu widget menggantikan widget lain di dalam pohon widget (widget tree). Sama dengan parameter key di Text.
2. textKey: Menetapkan kunci untuk widget Text yang dihasilkan. Berguna jika Anda perlu mengontrol atau mengidentifikasi widget Text di dalam pohon widget.
3. style: Parameter ini menentukan gaya teks (seperti warna, ukuran font, ketebalan) yang akan digunakan. Jika tidak ditentukan, gaya default akan digunakan.
4. minFontSize: Menentukan ukuran font terkecil yang diizinkan saat teks disesuaikan ukurannya. Jika teks tetap tidak cukup meski ukuran font minimum ini sudah digunakan, maka teks akan diatasi sesuai dengan pengaturan overflow. Ukuran minimum default adalah 12.
5. maxFontSize: Menentukan ukuran font terbesar yang diizinkan untuk auto-sizing teks. Parameter ini berguna untuk membatasi ukuran font ketika pewarisan gaya yang lebih besar tidak diinginkan.
6. stepGranularity: Menentukan seberapa besar langkah perubahan ukuran font saat disesuaikan dengan batas. Misalnya, jika langkah perubahan terlalu besar, maka perubahan ukuran font bisa terlihat kasar.
7. presetFontSizes: Menetapkan ukuran font yang diizinkan secara spesifik. Jika presetFontSizes digunakan, parameter minFontSize, maxFontSize, dan stepGranularity akan diabaikan.
8. group: Menyinkronkan ukuran teks dari beberapa AutoSizeText. Semua AutoSizeText yang ada dalam grup yang sama akan memiliki ukuran yang sama, menyesuaikan dengan ukuran terkecil yang efektif dalam grup tersebut.
9. textAlign: Menentukan bagaimana teks harus disejajarkan secara horizontal. Misalnya, teks bisa diatur sejajar di kiri, tengah, atau kanan.
10. textDirection: Menentukan arah penulisan teks, yang mempengaruhi cara kerja nilai textAlign seperti TextAlign.start dan TextAlign.end. Misalnya, untuk teks bahasa Arab atau Ibrani yang ditulis dari kanan ke kiri.
11. locale: Digunakan untuk memilih font ketika karakter Unicode yang sama dapat dirender berbeda tergantung pada lokalnya.
12. softWrap: Menentukan apakah teks harus terputus di jeda baris lunak. Jika softWrap adalah true, teks akan terbungkus di jeda baris yang lebih lemah.
13. wrapWords: Menentukan apakah kata-kata yang tidak sesuai dalam satu baris harus dibungkus ke baris berikutnya. Defaultnya true untuk berperilaku seperti Text.
14. overflow: Menentukan bagaimana penanganan overflow visual teks. Misalnya, apakah teks yang melebihi batas harus dipotong atau diganti dengan elipsis (...).
15. overflowReplacement: Jika teks melebihi batas dan tidak dapat disesuaikan ukurannya lagi, widget ini akan ditampilkan sebagai pengganti teks yang meluap.
16. textScaleFactor: Mengatur skala font piksel untuk setiap piksel logis. Ini juga mempengaruhi minFontSize, maxFontSize, dan presetFontSizes.
17. maxLines: Menentukan jumlah maksimum baris yang boleh dimiliki oleh teks. Jika tidak ditentukan, teks akan sesuai dengan lebar dan tinggi yang tersedia.
18. semanticsLabel: Label semantik alternatif untuk teks ini, yang digunakan oleh teknologi bantuan seperti screen readers.