
![cover](https://books.google.com/books/content?id=HmrDHwgkbPsC&printsec=frontcover&img=1&zoom=1&edge=curl&source=gbs_api)



**Title:** "REFACTORING: IMPROVING THE DESIGN OF EXISTING CODE"  
**Author**: "Martin Fowler"  
**Publisher**: Addison-Wesley  
**Published**: 2012-03-09  

# 📖 Refactoring: Improving the Design of Existing Code

## ℹ️ One-liner Summary
Buku ini mengajarkan cara membuat kode yang sudah ada jadi lebih rapi dan mudah diubah, tanpa mengubah cara kerjanya, agar pengembangan ke depan jadi lebih cepat dan mudah.

## Prinsip/Inti Pokok Buku
- Refactoring adalah proses mengubah struktur internal kode (merapikan, menyederhanakan) tanpa mengubah perilaku eksternalnya (fungsionalitasnya tetap sama).
- Tujuan utama refactoring adalah meningkatkan desain kode agar lebih mudah dipahami, dikelola, diubah, dan diperluas di masa depan.
- Refactoring harus dilakukan dalam langkah-langkah yang sangat kecil, sering, dan terkontrol untuk meminimalkan risiko dan memudahkan *debugging*.
- Pentingnya memiliki *test suite* yang kuat dan otomatis sebelum dan saat refactoring untuk memastikan fungsionalitas tidak rusak.
- Refactoring membantu developer menemukan dan menghilangkan "code smells" (indikator masalah dalam desain kode, seperti metode yang terlalu panjang atau duplikasi kode).
- Ini adalah bagian integral dari proses pengembangan perangkat lunak, bukan tugas terpisah yang dilakukan sesekali.
- Dengan rajin refactoring, biaya pengembangan jangka panjang akan berkurang karena kode menjadi lebih bersih, lebih mudah dipelihara, dan kurang rentan terhadap bug.

## Pertanyaan Reflektif
- Kapan terakhir kali Anda sengaja mengalokasikan waktu untuk merapikan bagian kode yang sudah berfungsi, alih-alih langsung melompat ke fitur baru?
- Apakah Anda cenderung menunda perbaikan kecil pada struktur kode dengan pikiran "nanti saja kalau ada waktu luang", padahal waktu luang itu jarang datang?
- Bagaimana reaksi Anda saat menemukan bagian kode yang sulit dipahami atau diubah? Apakah Anda langsung mencari jalan pintas atau mencoba memahami dan memperbaikinya?
- Seberapa yakin Anda dengan *test suite* yang Anda miliki saat ini untuk menangkap potensi bug jika Anda melakukan perubahan struktural besar pada codebase?
- Apakah Anda merasa nyaman untuk mengubah atau merestrukturisasi kode yang ditulis orang lain (atau bahkan kode Anda sendiri yang sudah lama), ataukah Anda takut merusak sesuatu?

## Potensi Hambatan
- **Takut merusak fungsionalitas yang sudah berjalan:** Kekhawatiran bahwa perubahan kecil pada struktur kode dapat menyebabkan bug tak terduga yang sulit ditemukan.
- **Tekanan *deadline* dan kurangnya waktu:** Merasa dikejar target fitur baru sehingga tidak ada waktu yang dialokasikan untuk "memperbaiki" kode yang sudah berfungsi.
- **Ketidakpastian harus mulai dari mana:** Codebase yang besar dan kompleks membuat bingung bagaimana memulai refactoring tanpa merasa kewalahan.
- **Kurangnya pemahaman tentang *code smells*:** Tidak dapat mengenali indikator atau pola dalam kode yang menunjukkan adanya masalah desain dan perlu diperbaiki.
- **Resistensi dari tim atau manajemen:** Persepsi bahwa refactoring adalah pemborosan waktu yang tidak langsung menghasilkan fitur baru atau nilai bisnis yang terlihat.

## Tips Mengatasi Hambatan
- **Mulai dengan tes:** Sebelum refactoring, pastikan Anda memiliki tes yang mencakup bagian kode yang akan diubah. Jika belum ada, tulis tesnya terlebih dahulu.
- **Alokasikan waktu kecil setiap hari:** Sisihkan 15-30 menit setiap hari (atau setiap kali menyentuh kode) untuk melakukan refactoring kecil dan bertahap.
- **Pilih area kecil yang jelas:** Mulai dengan satu fungsi, kelas, atau modul yang spesifik dan jelas-jelas bermasalah, lalu selesaikan satu per satu.
- **Pelajari *code smells* dasar:** Kenali beberapa pola umum seperti *Long Method*, *Duplicate Code*, atau *Large Class* untuk memandu Anda menemukan area refactoring.
- **Komunikasikan manfaatnya:** Jelaskan kepada tim atau manajemen bahwa refactoring mengurangi bug, mempercepat pengembangan fitur di masa depan, dan meningkatkan produktivitas jangka panjang.

## 🔥 Implementasi di Dunia Nyata
- **Developer:** Mengubah nama variabel dari `x` menjadi `customerAccount` agar kode lebih mudah dibaca dan dipahami.
- **Desainer UI/UX:** Mengorganisir ulang layer-layer pada file desain (Figma/Sketch) agar lebih rapi dan mudah diakses oleh desainer lain.
- **Content Creator:** Menstrukturkan ulang folder aset media (gambar, video) berdasarkan kategori atau tanggal agar cepat menemukan bahan yang dibutuhkan.
- **Musisi:** Mengelompokkan trek-trek dalam *Digital Audio Workstation* (DAW) menjadi grup yang logis (misal: "Drums", "Vocals") agar proses mixing lebih efisien.
- **Mahasiswa:** Merapikan catatan kuliah dengan membuat indeks, ringkasan per bab, atau memisah materi menjadi topik-topik kecil.
- **Freelancer:** Menstandarisasi template proposal dan invoice agar konsisten, profesional, dan cepat saat mengirim ke klien baru.
- **Pekerja Kantoran:** Mengatur ulang struktur folder *share drive* kantor agar semua dokumen proyek mudah ditemukan oleh seluruh anggota tim.
- **Penulis:** Mengedit ulang draf tulisan untuk menghilangkan kalimat berulang atau merestrukturisasi paragraf agar alur cerita lebih koheren.
- **Admin Sistem/DevOps:** Mengoptimalkan skrip otomatisasi yang bertele-tele agar lebih ringkas dan mudah dipelihara.
- **Manajer Proyek:** Memecah tugas-tugas besar dalam *project plan* menjadi subtugas yang lebih kecil dan terukur agar lebih mudah dikelola.

## 📚 Case Story

- **Judul Cerita: Maya, Si Pengembang Aplikasi yang Berani Berubah**

- **Paragraf Pembuka**
  Maya adalah seorang pengembang aplikasi *mobile* di sebuah *startup* yang sedang berkembang pesat. Ia bangga dengan fitur-fitur yang berhasil diluncurkannya, namun ada satu hal yang terus menghantuinya: kode dasar aplikasinya yang semakin lama semakin berantakan. Metode-metode yang panjang, duplikasi kode di sana-sini, dan ketergantungan antar bagian yang tidak jelas membuat setiap penambahan fitur baru terasa seperti berjudi. Maya sering menghabiskan waktu berjam-jam hanya untuk melacak bug atau memahami kode yang ia tulis sendiri beberapa bulan lalu, membuatnya merasa lelah dan kurang produktif.

- **Langkah Aksi**
  1.  **Mengakui Masalah dan Komitmen:** Maya membaca buku tentang *refactoring* dan menyadari bahwa ia perlu mengubah pendekatannya. Ia berkomitmen untuk menerapkan prinsip-prinsip tersebut secara bertahap.
  2.  **Membangun Jaring Pengaman (Tests):** Sebelum menyentuh kode inti yang rumit, ia menghabiskan beberapa hari untuk menulis *unit test* dan *integration test* yang komprehensif untuk memastikan semua fungsionalitas penting bekerja sesuai harapan. Ini memberinya rasa aman.
  3.  **Memilih Target Kecil:** Ia tidak mencoba merombak seluruh aplikasi sekaligus. Maya memilih satu modul kecil yang sering menimbulkan masalah (misalnya, modul otentikasi pengguna) sebagai area pertama untuk di-*refactor*.
  4.  **Langkah-langkah Mikro:** Ia mulai dengan perubahan sangat kecil: mengganti nama variabel yang ambigu, memecah metode yang terlalu panjang menjadi beberapa metode yang lebih pendek dan spesifik, atau memindahkan bagian kode yang tidak pada tempatnya. Setelah setiap perubahan kecil, ia segera menjalankan semua tes untuk memastikan tidak ada yang rusak.
  5.  **Mengenali "Code Smells":** Maya mulai terlatih mengenali *code smells* seperti *Duplicate Code* atau *Large Class*. Setiap kali ia menemukannya saat mengerjakan fitur baru, ia meluangkan waktu sejenak untuk memperbaikinya sebelum melanjutkan.
  6.  **Budaya "Clean Code":** Ia mulai membagikan pengetahuannya tentang refactoring kepada timnya, mendorong mereka untuk mengadopsi kebiasaan yang sama dan melakukan *code review* dengan fokus pada kebersihan kode.

- **✨ Hasilnya**
  Dalam beberapa bulan, kode aplikasi Maya mulai bertransformasi. Modul-modul menjadi lebih terorganisir, mudah dibaca, dan jauh lebih stabil. Waktu yang ia habiskan untuk mencari dan memperbaiki bug berkurang drastis. Penambahan fitur baru yang tadinya memakan waktu berhari-hari kini bisa diselesaikan lebih cepat dan dengan percaya diri. Maya tidak lagi merasa cemas saat memodifikasi kode lama; justru, ia menikmati proses membersihkan dan menyempurnakan karyanya. Timnya pun menjadi lebih produktif dan kolaboratif, karena semua orang kini lebih mudah memahami dan bekerja dengan kode yang sama.

## Urutan Penerapan (Dari Paling Penting)
1.  **Memastikan adanya Test Suite yang Kuat:** Ini adalah fondasi utama. Tanpa serangkaian tes otomatis yang solid, setiap upaya refactoring akan sangat berisiko karena Anda tidak akan tahu apakah perubahan Anda merusak fungsionalitas yang ada. Tes berfungsi sebagai jaring pengaman.
2.  **Lakukan Refactoring dalam Langkah-langkah Sangat Kecil:** Perubahan besar rawan bug dan sulit dilacak. Dengan membuat perubahan kecil dan bertahap, Anda meminimalkan risiko, mempermudah identifikasi masalah, dan menjaga kode tetap dalam keadaan bekerja.
3.  **Refactoring Secara Terus-menerus dan Sering:** Jadikan refactoring sebagai kebiasaan sehari-hari, bukan proyek besar yang dilakukan sesekali. Setiap kali Anda menyentuh kode untuk menambah fitur atau memperbaiki bug, luangkan waktu sejenak untuk merapikannya.
4.  **Fokus pada *Code Smells*:** Belajar mengenali indikator-indikator masalah dalam kode (misalnya metode yang terlalu panjang, duplikasi kode). Ini memberikan panduan tentang apa yang perlu di-*refactor* dan memprioritaskan upaya Anda.
5.  **Meningkatkan Keterbacaan dan Kejelasan Kode:** Tujuan akhir refactoring adalah membuat kode lebih mudah dipahami oleh siapa pun (termasuk diri Anda di masa depan). Prioritaskan kejelasan nama, struktur, dan arsitektur kode.

## Jika Hanya Menerapkan 1 Hal dari Buku Ini
**Selalu memastikan bahwa Anda memiliki *test suite* yang solid sebelum menyentuh kode yang akan di-*refactor*, bahkan jika itu berarti Anda harus menulis tesnya terlebih dahulu.**

Contoh penerapan sangat sederhana: Jika Anda ingin memisahkan logika dari sebuah fungsi yang panjang menjadi dua fungsi yang lebih kecil, pertama tulis tes yang menguji semua skenario *input* dan *output* dari fungsi asli tersebut. Setelah semua tes hijau, barulah Anda mulai memodifikasi dan memecah fungsi tersebut sedikit demi sedikit, sambil terus menjalankan tes untuk memastikan tidak ada fungsionalitas yang rusak.

## ⭐️ Takeaway Utama (Golden Nuggets)
- **Tes adalah Jaring Pengaman Anda:** Jangan berani refactor tanpa tes otomatis yang kuat; mereka adalah kunci untuk mengubah kode dengan percaya diri dan aman.
- **Refactor Sedikit, Sering, dan Terus-menerus:** Kebersihan kode adalah proses berkelanjutan, bukan proyek sekali jadi. Rajinlah merapikan kode dalam langkah-langkah kecil.
- **Desain yang Baik Tumbuh, Bukan Dibuat Sempurna dari Awal:** Dengan refactoring, Anda secara iteratif membentuk dan meningkatkan desain kode Anda seiring waktu, daripada mencoba merencanakannya dengan sempurna di muka.

## 📣 Quotes / Kutipan Penting
- "Any fool can write code that a computer can understand. Good programmers write code that humans can understand." — Martin Fowler
- "Refactoring is the process of changing a software system in such a way that it does not alter the external behavior of the code yet improves its internal structure." — Martin Fowler
- "The first step to refactoring is to get a solid test suite in place." — Martin Fowler
