
![cover](https://books.google.com/books/content?id=hkfEzgEACAAJ&printsec=frontcover&img=1&zoom=1&source=gbs_api)



**Title:** "A PHILOSOPHY OF SOFTWARE DESIGN"  
**Author**: "John K. Ousterhout"  
**Publisher**: null  
**Published**: 2021  

Tentu, ini ringkasan terstruktur dari buku "A Philosophy of Software Design" oleh John Ousterhout:

---

# 📖 A Philosophy of Software Design

## Prinsip/Inti Pokok Buku
- **Kurangi Kompleksitas Secara Maksimal:** Tujuan utama desain perangkat lunak adalah meminimalkan kompleksitas agar sistem mudah dipahami, diubah, dan dipelihara.
- **Modul yang "Dalam" (Deep Modules):** Desainlah modul dengan fungsionalitas yang kuat dan beragam (banyak fungsionalitas) tetapi memiliki antarmuka (interface) yang sangat sederhana. Ini disebut "informasi tersembunyi" (information hiding).
- **Antarmuka yang Sederhana:** Antarmuka suatu modul harus intuitif, mudah digunakan, dan tidak membebani pengguna (developer lain yang memakai modul tersebut) dengan detail implementasi internal.
- **Lapisan (Layered Design):** Susun sistem dalam lapisan-lapisan yang jelas, di mana setiap lapisan hanya berinteraksi dengan lapisan di bawahnya. Ini meningkatkan modularitas dan pemisahan tanggung jawab.
- **Komentar Menjelaskan "Apa", Bukan "Bagaimana":** Komentar harus menjelaskan *mengapa* sesuatu dilakukan dan *apa* yang dilakukannya, bukan *bagaimana* implementasinya (karena itu sudah jelas dari kode). Komentar membantu mengatasi kompleksitas.
- **"Fewer Features" (Lebih Sedikit Fitur):** Hindari menambahkan fitur yang tidak esensial karena setiap fitur menambah kompleksitas pada sistem secara keseluruhan, baik secara langsung maupun tidak langsung.
- **Desain Generalis (General-Purpose Design):** Pertimbangkan untuk membuat komponen yang cukup general sehingga bisa digunakan kembali di beberapa tempat, tetapi jangan sampai terlalu general hingga menambah kompleksitas yang tidak perlu.
- **Pentingnya Nama yang Jelas:** Beri nama variabel, fungsi, dan kelas yang deskriptif dan mencerminkan tujuannya untuk meningkatkan keterbacaan kode.
- **Refactoring Berkesinambungan:** Desain adalah proses berkelanjutan. Jangan takut untuk merestrukturisasi kode (refactor) saat pemahaman Anda tentang masalah atau solusi berkembang.
- **Hindari Mode "Tactical Programming":** Jangan hanya fokus menyelesaikan masalah saat ini tanpa memikirkan desain jangka panjang. Luangkan waktu untuk berpikir strategis tentang struktur kode.

## Pertanyaan Reflektif
1.  Di bagian mana dari pekerjaan atau proyek Anda saat ini Anda merasakan tingkat kompleksitas yang tinggi, dan bagaimana Anda bisa mengidentifikasinya?
2.  Bagaimana Anda bisa menerapkan konsep "modul dalam" atau "informasi tersembunyi" pada tugas atau sistem yang Anda kelola agar lebih mudah dipahami orang lain?
3.  Apakah Anda cenderung menambahkan terlalu banyak "fitur" atau detail yang sebenarnya tidak esensial dalam proyek Anda? Bagaimana cara Anda menyeleksinya?
4.  Kapan terakhir kali Anda meluangkan waktu untuk merestrukturisasi atau menyederhanakan suatu proses/desain yang sudah ada, dan apa hasilnya?
5.  Bagaimana Anda bisa mengubah fokus dari hanya "menyelesaikan" tugas menjadi "mendesain" solusi yang lebih elegan dan mudah dipelihara di masa depan?

## Potensi Hambatan
1.  **Tekanan Batas Waktu:** Seringkali, tenggat waktu yang ketat mendorong programmer untuk mengambil jalan pintas dan mengabaikan desain yang baik demi fungsionalitas yang cepat jadi.
2.  **Warisan Kode (Legacy Code):** Berurusan dengan sistem atau kode lama yang sudah sangat kompleks dan berantakan membuat penerapan prinsip desain baru terasa mustahil atau terlalu mahal.
3.  **Ketakutan akan Refactoring:** Kekhawatiran akan merusak fungsionalitas yang sudah ada saat mencoba menyederhanakan atau merestrukturisasi kode.
4.  **Kurangnya Pemahaman Tim:** Anggota tim yang berbeda mungkin memiliki tingkat pemahaman atau prioritas yang berbeda terhadap pentingnya desain, menyebabkan inkonsistensi.
5.  **Permintaan Fitur Tanpa Henti:** Tekanan dari pemangku kepentingan untuk terus menambahkan fitur baru tanpa memberi waktu untuk perbaikan desain internal, menyebabkan "scope creep" dan kompleksitas menumpuk.

## Tips Mengatasi Hambatan
1.  **Alokasikan Waktu Desain dan Refactor:** Bernegosiasi dengan manajer untuk mengalokasikan persentase waktu (misalnya, 10-20%) khusus untuk perbaikan desain atau refactoring dalam setiap sprint/proyek.
2.  **Mulai dari yang Kecil:** Jika berhadapan dengan legacy code, identifikasi bagian terkecil dan paling kritis yang bisa Anda refactor menjadi modul yang lebih baik tanpa memengaruhi sistem secara keseluruhan.
3.  **Tulis Tes Otomatis (Automated Tests):** Tes otomatis memberikan jaring pengaman saat refactoring. Jika tes lolos setelah perubahan, Anda tahu bahwa fungsionalitas dasar tidak rusak.
4.  **Edukasi dan Komunikasi:** Secara aktif diskusikan dan edukasi tim tentang manfaat desain yang baik (misalnya, melalui sesi berbagi pengetahuan, code review yang konstruktif) untuk membangun pemahaman bersama.
5.  **Prioritaskan dengan Bijak:** Belajar mengatakan "tidak" atau menunda fitur yang tidak penting. Jelaskan dampak penambahan fitur yang tidak terkendali terhadap pemeliharaan dan kualitas jangka panjang.

## Implementasi di Dunia Nyata
1.  **Developer:** Membuat fungsi utilitas yang memiliki satu tugas spesifik dan jelas, dengan parameter input yang minimal, untuk menghindari duplikasi kode dan meningkatkan modularitas.
2.  **Desainer UI/UX:** Mendesain sistem komponen (Design System) yang modular, di mana setiap komponen (tombol, kartu, form input) memiliki tampilan dan perilaku yang konsisten, mudah digunakan kembali, dan dipahami.
3.  **Content Creator (Blogger/YouTuber):** Merencanakan setiap artikel atau video sebagai "modul" yang membahas satu topik inti secara mendalam, dengan struktur jelas (pendahuluan, poin-poin utama, kesimpulan) yang mudah diikuti oleh audiens.
4.  **Musisi (Produser Musik):** Memisahkan elemen-elemen lagu (bass, drum, melodi, vokal) ke dalam trek atau grup terpisah dalam DAW (Digital Audio Workstation) agar lebih mudah diatur, di-mix, dan dimanipulasi tanpa mengganggu elemen lain.
5.  **Mahasiswa:** Mengatur catatan kuliah berdasarkan bab atau topik utama, dengan setiap bagian berfungsi sebagai "modul" informasi yang mandiri dan saling terkait, mempermudah revisi.
6.  **Freelancer:** Membuat template proposal proyek yang modular, dengan bagian-bagian yang bisa disesuaikan (latar belakang, solusi, estimasi biaya) agar cepat beradaptasi untuk klien yang berbeda.
7.  **Pekerja Kantoran (Manajer Proyek):** Memecah proyek besar menjadi tugas-tugas kecil yang terdefinisi dengan baik, masing-masing dengan penanggung jawab dan output yang jelas, mengurangi kompleksitas keseluruhan proyek.
8.  **Penulis Buku:** Menyusun buku dalam bab-bab yang mandiri namun berurutan, di mana setiap bab fokus pada satu ide atau argumen utama, sehingga pembaca mudah memahami alur pemikiran.
9.  **Koki/Pengelola Dapur:** Menerapkan "mise en place" (semua bahan disiapkan dan diukur sebelum memasak), memisahkan proses persiapan dari proses memasak inti, membuat alur kerja lebih efisien dan mengurangi kesalahan.
10. **Admin Sistem/Jaringan:** Mengatur konfigurasi server dalam file-file terpisah berdasarkan fungsi (misalnya, web server, database, firewall) daripada menumpuk semua dalam satu file besar, mempermudah pemeliharaan dan debugging.

## 📚 Case Story

### Web Developer yang Terjebak "Spaghetti Code"

Rian adalah seorang developer muda di sebuah startup. Dia sangat bersemangat saat pertama kali bergabung, tetapi tak lama kemudian, semangatnya mulai terkikis oleh proyek utama yang sedang ia kerjakan: aplikasi manajemen inventaris. Aplikasi ini sudah ada sejak lama, dan setiap kali ia mencoba menambahkan fitur baru atau memperbaiki bug, rasanya seperti melangkah di lahan ranjau. Kode-kodenya saling terkait tanpa aturan yang jelas, satu perubahan kecil bisa menyebabkan kerusakan di tempat lain. Rian sering menghabiskan waktu berjam-jam hanya untuk memahami apa yang dilakukan sebuah fungsi, yang disebut timnya sebagai "spaghetti code."

Suatu hari, setelah gagal memperbaiki bug kritis selama dua hari penuh, Rian merasa putus asa. Ia mulai membaca buku "A Philosophy of Software Design" yang direkomendasikan seniornya. Perlahan, ia menyadari bahwa masalahnya bukan pada dirinya, melainkan pada desain aplikasi yang sangat kompleks. Ia memutuskan untuk mencoba menerapkan prinsip-prinsip buku tersebut, dimulai dari bagian yang paling sering ia sentuh.

**Poin-poin aksi:**
1.  **Identifikasi Modul Paling Bermasalah:** Rian mulai dengan mengidentifikasi bagian kode yang paling sering diubah dan paling sering menyebabkan bug. Ia menemukan modul "manajemen produk" adalah biang kerok utama.
2.  **Definisikan Antarmuka yang Jelas:** Untuk modul manajemen produk, ia mulai mendefinisikan "apa" yang harus dilakukan modul tersebut (misalnya, menambah produk, mengubah harga, menghapus produk) dan "bagaimana" berinteraksi dengannya, mengabaikan detail internalnya.
3.  **Informasi Tersembunyi (Encapsulation):** Rian merestrukturisasi modul agar detail tentang bagaimana produk disimpan di database atau divalidasi tidak diketahui oleh modul lain yang menggunakannya. Modul lain hanya perlu memanggil `tambahProduk(dataProduk)` tanpa perlu tahu implementasi di baliknya.
4.  **Buat Fungsi Kecil, Jelas, dan Mandiri:** Ia memecah fungsi-fungsi besar dalam modul menjadi fungsi-fungsi yang lebih kecil, masing-masing hanya melakukan satu tugas spesifik (misalnya, `validasiNamaProduk()`, `simpanDataProdukKeDB()`, `kirimNotifikasiProdukBaru()`).
5.  **Tulis Komentar "Mengapa" dan "Apa":** Daripada mengomentari setiap baris kode dengan "ini adalah loop untuk item," Rian menulis komentar di awal fungsi atau kelas yang menjelaskan *tujuan* dari fungsi tersebut dan *mengapa* ia didesain seperti itu.
6.  **Refactoring Secara Bertahap:** Alih-alih merombak semuanya sekaligus, Rian mendedikasikan 1-2 jam setiap hari untuk refactoring bagian kecil dari modul manajemen produk, memastikan semua tes yang ada masih berjalan.
7.  **Prioritaskan Simplicity:** Ketika ada permintaan fitur baru, Rian berdiskusi dengan tim untuk mencari cara paling sederhana untuk mengimplementasikannya, terkadang menunda fitur minor untuk menjaga desain tetap bersih.

**✨ Hasilnya:**
Setelah beberapa minggu, modul manajemen produk Rian yang tadinya "spaghetti code" berubah menjadi struktur yang lebih rapi dan modular. Bug di bagian itu berkurang drastis, dan waktu yang dibutuhkan untuk menambahkan fitur baru atau memperbaiki masalah menyusut signifikan. Rian tidak lagi merasa takut menyentuh kode tersebut. Rekan kerjanya pun mulai memperhatikan perubahan positif ini dan bertanya bagaimana ia melakukannya. Dengan bangga, Rian menjelaskan bahwa ia bukan hanya seorang programmer, tapi juga seorang "desainer perangkat lunak" yang berinvestasi pada kesederhanaan dan kejelasan, sebuah filosofi yang kini ia terapkan di seluruh pekerjaannya.
