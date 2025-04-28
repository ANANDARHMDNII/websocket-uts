| Variable           |             Isi            |
| -------------------|----------------------------|
| Nama           |        ANANDA RAHMADANI     |
| NIM            |          312310461         |
| Kelas          |          TI.23.A.5         |
| Mata Kuliah    |     Pemrograman Web2     |
### WebSocket: Solusi Komunikasi Real-Time untuk Web Modern
# Pendahuluan
Di dunia web modern, aplikasi yang mengandalkan komunikasi real-time sangat populer, mulai dari aplikasi chat, permainan multiplayer, hingga notifikasi langsung. Salah satu teknologi yang memungkinkan hal ini adalah WebSocket.
WebSocket menyediakan kanal komunikasi dua arah yang terbuka antara klien dan server, memungkinkan data dipertukarkan secara cepat dan efisien tanpa perlu membuat koneksi baru berulang kali.

# Apa Itu WebSocket?
WebSocket adalah protokol komunikasi yang memungkinkan komunikasi dua arah yang terbuka dan terus-menerus antara klien dan server melalui koneksi TCP. Ini sangat berguna untuk aplikasi yang membutuhkan pengiriman data secara cepat dan terus-menerus, seperti chat online, notifikasi real-time, dan game multiplayer.
Berbeda dengan HTTP yang bersifat request-response, WebSocket memungkinkan data dikirim kapan saja tanpa perlu permintaan baru dari klien.

# Contoh Implementasi WebSocket dengan Express + ws
Sekarang kita akan membuat implementasi WebSocket menggunakan Express untuk server dan ws untuk WebSocket. Ini memungkinkan kita untuk menggabungkan kemampuan Express dalam menangani HTTP dengan WebSocket untuk komunikasi real-time.

  1. Instalasi Dependencies
  Instalasi package yang diperlukan:
  ![Screenshot 2025-04-28 110017](https://github.com/user-attachments/assets/e29d7eff-c5eb-47d4-a15f-e447414a23c5)
  2. Membuat Server Express + WebSocket
    Langkah 1: Buat file server server.js
     ![image](https://github.com/user-attachments/assets/7e38a88f-f274-4d37-90ad-2190ba43e43f)
 3. Membuat Klien WebSocket
Buat file public/client.html di dalam folder public:
     ![image](https://github.com/user-attachments/assets/3760ad85-18d6-442a-a6a1-7520b2b208d8)
  ![image](https://github.com/user-attachments/assets/dc7bb855-8b17-4374-b09c-8ddf559a55ae)

# Cara Menjalankan
  1. Jalankan server Express + WebSocket:
  2. Buka browser dan akses http://localhost:8080/client.html.
  3. Ketik pesan di input dan klik Kirim. Pesan akan langsung dikirim ke server dan      server akan membalasnya.
     ![Screenshot 2025-04-28 135633](https://github.com/user-attachments/assets/25ff533f-5054-46ee-a2e8-c42addc2cdd9)
  ![Screenshot 2025-04-28 131816](https://github.com/user-attachments/assets/2b4e36b2-9b3d-4a17-a708-d3a01c46458b)

# Kesimpulan
WebSocket adalah solusi sempurna untuk aplikasi web yang membutuhkan komunikasi real-time. Dengan kemampuan komunikasi dua arah yang terbuka dan efisien, WebSocket sangat cocok digunakan untuk aplikasi chat, game multiplayer, notifikasi real-time, dan banyak aplikasi lainnya.
Dengan menggunakan kombinasi Express dan WebSocket, kita bisa membangun aplikasi yang tidak hanya responsif, tetapi juga efisien dalam hal penggunaan sumber daya dan latensi.

   ## TERIMAKASIH
 
