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

# Implementasi WebSocket dengan Node.js
Untuk menggunakan WebSocket, kita dapat menggunakan pustaka ws di Node.js. Berikut adalah contoh implementasi sederhana menggunakan WebSocket:
1. Menginstall ws di Node.js
  npm install ws
2. Membuat Server WebSocket
    // server.js
const express = require('express');
const WebSocket = require('ws');

// Inisialisasi Express
const app = express();
const port = 8080;

// Membuat server HTTP dari Express
const server = app.listen(port, () => {
  console.log(`Server berjalan di http://localhost:${port}`);
});

// Membuat WebSocket server
const wss = new WebSocket.Server({ server });

wss.on('connection', (ws) => {
  console.log('Klien terhubung');

  ws.on('message', (message) => {
    console.log(`Pesan dari klien: ${message}`);
    ws.send(`Server menerima: ${message}`);
  });

  ws.on('close', () => {
    console.log('Klien terputus');
  });
});

// Menyajikan file statis (HTML)
app.use(express.static('public'));
