# Tubes-Pemrograman-Jaringan-Ferdinand

Nama   : Ferdinand Dwi

NIM    : 1203220138

# Soal UTS
Berikan saya code server dan client
Buatlah sebuah permainan yang menggunakan soket dan protokol UDP. Permainannya cukup sederhana, dengan 1 server dapat melayani banyak klien (one-to-many). Setiap 10 detik, server akan mengirimkan kata warna acak dalam bahasa Inggris kepada semua klien yang terhubung. Setiap klien harus menerima kata yang berbeda (unik). Selanjutnya, klien memiliki waktu 5 detik untuk merespons dengan kata warna dalam bahasa Indonesia. Setelah itu, server akan memberikan nilai feedback 0 jika jawabannya salah dan 100 jika benar. Ketika client memasukan jawaban dengan bahasa indonesia akan mengeluarkan output ("Jawaban benar! Nilai: 100")


# How code works
1. Server :
   
   •  Server ini dibuat menggunakan modul Socket Python dengan protokol UDP. Konfigurasi server memungkinkan server untuk mendengarkan koneksi masuk dari klien pada alamat IP “localhost” dan port 12345. Ketika server menerima koneksi dari klien, server membaca data yang dikirim oleh klien. Data ini diasumsikan berupa warna yang dikirim dalam format string. Dengan satu server, kita dapat melayani banyak klien secara bersamaan. Setiap 10 detik, server akan mengirimkan kata warna acak dalam bahasa Inggris kepada semua klien yang terhubung. Klien memiliki waktu 5 detik untuk merespons dengan kata warna dalam bahasa Indonesia. Setelah itu, server akan memberikan nilai feedback: 0 jika jawaban klien salah dan 100 jika jawaban klien benar. Program ini merupakan contoh sederhana server UDP yang mengirimkan data secara berkala. Perlu diingat bahwa protokol UDP tidak menjamin pengiriman data yang handal, sehingga program ini cocok untuk skenario di mana kehilangan data dapat diterima.

![image](https://github.com/ferdinandiip/Tubes-Pemrograman-Jaringan-Ferdinand/assets/162901297/db9f5cf4-8338-4e0a-91f7-549a553fa84f)

![image](https://github.com/ferdinandiip/Tubes-Pemrograman-Jaringan-Ferdinand/assets/162901297/5f636e9c-6788-406a-8613-41fc63150dc0)

2. Client :
   
   •  Program ini adalah bagian dari aplikasi client yang menggunakan protokol UDP untuk berkomunikasi dengan server. Saat dijalankan, client membuat soket UDP dan mengirim pesan "connect" ke server untuk memulai koneksi. Selanjutnya, dalam loop tak terbatas, client terus menerima data dari server, yang merupakan warna dalam bahasa Inggris. Setelah menerima warna, client meminta pengguna untuk memasukkan warna yang sesuai dalam bahasa Indonesia. Setelah pengguna memberikan respons, client membandingkan respons tersebut dengan terjemahan warna yang diterima menggunakan kamus yang telah ditentukan. Jika respons pengguna sesuai, client mencetak "Jawaban benar! Nilai: 100", dan jika tidak, mencetak "Jawaban salah. Nilai: 0". Program ini terus berjalan, menerima warna dari server, meminta input dari pengguna, dan memberikan respons berdasarkan input tersebut.
![Screenshot 2024-04-27 092418](https://github.com/ferdinandiip/Tubes-Pemrograman-Jaringan-Ferdinand/assets/162901297/2004f28f-9e7f-4f9d-bdd4-63f129da0d1e)
![image](https://github.com/ferdinandiip/Tubes-Pemrograman-Jaringan-Ferdinand/assets/162901297/bc234b83-0f9a-45ef-93b7-642ac749ab94)





   
