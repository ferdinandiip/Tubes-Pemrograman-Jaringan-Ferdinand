# Tubes-Pemrograman-Jaringan-Ferdinand

Nama   : Ferdinand Dwi

NIM    : 1203220138

# Soal UTS
Berikan saya code server dan client
Buatlah sebuah permainan yang menggunakan soket dan protokol UDP. Permainannya cukup sederhana, dengan 1 server dapat melayani banyak klien (one-to-many). Setiap 10 detik, server akan mengirimkan kata warna acak dalam bahasa Inggris kepada semua klien yang terhubung. Setiap klien harus menerima kata yang berbeda (unik). Selanjutnya, klien memiliki waktu 5 detik untuk merespons dengan kata warna dalam bahasa Indonesia. Setelah itu, server akan memberikan nilai feedback 0 jika jawabannya salah dan 100 jika benar. Ketika client memasukan jawaban dengan bahasa indonesia akan mengeluarkan output ("Jawaban benar! Nilai: 100")


syarat UTS :
• Kerjakan dengan menggunakan bahasa pemrograman python
• Menggunakan protokol UDP
• Code untuk server dan client dikumpulkan di github repository masing masing
• Pada readme.md silahkan beri penjelaskan how code works. 
• Test case : 1 server 10 client.
• Pastikan memahami soal.
• Silahkan kumpulkan link github repository di assignment ini.JANGAN TELAT ! 


# Jawaban
1. Server :Server ini dibuat menggunakan modul Socket Python dengan protokol UDP. Konfigurasi server memungkinkan server untuk mendengarkan koneksi masuk dari klien pada alamat IP “localhost” dan port 12345. Ketika server menerima koneksi dari klien, server membaca data yang dikirim oleh klien. Data ini diasumsikan berupa warna yang dikirim dalam format string. Dengan satu server, kita dapat melayani banyak klien secara bersamaan. Setiap 10 detik, server akan mengirimkan kata warna acak dalam bahasa Inggris kepada semua klien yang terhubung. Klien memiliki waktu 5 detik untuk merespons dengan kata warna dalam bahasa Indonesia. Setelah itu, server akan memberikan nilai feedback: 0 jika jawaban klien salah dan 100 jika jawaban klien benar. Program ini merupakan contoh sederhana server UDP yang mengirimkan data secara berkala. Perlu diingat bahwa protokol UDP tidak menjamin pengiriman data yang handal, sehingga program ini cocok untuk skenario di mana kehilangan data dapat diterima.


2. Client : 
