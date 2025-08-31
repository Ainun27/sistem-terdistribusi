# 💬 Real-Time Distributed Discussion App

Aplikasi diskusi interaktif **real-time** berbasis arsitektur terdistribusi yang dikembangkan menggunakan **Flask**, **Flask-SocketIO**, dan protokol **WebSocket**.  
Sistem ini memungkinkan banyak pengguna untuk berdiskusi dalam satu ruang bersama secara langsung (real-time), menyerupai ruang diskusi virtual seperti kanal pada platform Discord.  

---

## 📌 Latar Belakang
Penggunaan **WebSocket** sangat krusial dalam pengembangan aplikasi ini karena memungkinkan komunikasi **dua arah yang persisten** antara klien dan server, tanpa perlu polling tradisional.  
Hal ini mengurangi latensi, menekan overhead jaringan, serta menjadikannya solusi tepat untuk aplikasi **event-driven** dan **real-time**.  

Selain itu, sistem ini menerapkan **dua server aplikasi** yang dapat beroperasi independen dengan dukungan **bridge Apache2**. Komponen bridge berfungsi sebagai load balancer sekaligus mekanisme **failover**, sehingga pengguna tidak merasakan gangguan ketika salah satu server down.

---

## 🎯 Tujuan
1. Membangun aplikasi diskusi real-time berbasis sistem terdistribusi.  
2. Mengimplementasikan WebSocket untuk komunikasi dua arah yang efisien.  
3. Mengaktifkan modul Apache sebagai bridge untuk menghubungkan dua server aplikasi.  

---

## 🌟 Manfaat
1. Memahami prinsip kerja sistem terdistribusi dalam konteks aplikasi diskusi.  
2. Meningkatkan keamanan dan efisiensi komunikasi data real-time.  
3. Memberikan solusi **high availability** dengan failover otomatis.  

---

## 🛠️ Alat & Bahan
- **Server**: Ubuntu, Flask, Flask-SocketIO  
- **Client**: Python, Socket.IO, Browser (Firefox/Chrome)  
- **Tools**: Virtual Environment, pip, editor teks  

---

## 🏗️ Arsitektur Sistem
- **2 Server Aplikasi** → Menangani koneksi pengguna & komunikasi WebSocket.  
- **Bridge (Apache2)** → Mengelola load balancing + failover otomatis.  
- **Client** → Mengakses aplikasi via browser dengan komunikasi WebSocket.  

⚡ Arsitektur ini memastikan komunikasi tetap lancar walaupun salah satu server mati (high availability).  

---

## 🌐 Keterbatasan
Saat ini aplikasi hanya bisa diakses dalam **jaringan lokal (LAN)**.  
Untuk akses eksternal, perlu pengembangan lebih lanjut pada konfigurasi jaringan & keamanan.  

---

## 📄 Dokumentasi Lengkap
- 📌 Notion: [Konfigurasi Diskusi Real-Time](https://www.notion.so/KONFIGURASI-DISKUSI-REAL-TIME-217c784027c1806a81b6f6dfd58ebb12)

---

## 👨‍💻 Pengembang
- Ainun Dwi Permana 
- Dita Tiara Putri 
- Nur Laila  
- Suci Maolia 

---

✍️ *Proyek ini merupakan hasil implementasi pembelajaran sistem terdistribusi. Ide dan rancangan utama berasal dari Ainun Dwi Permana (terinspirasi dari aplikasi real-time serupa), sedangkan pengembangan teknis dilakukan secara kolaboratif bersama tim.*
