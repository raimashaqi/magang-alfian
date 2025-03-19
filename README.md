<center><h1>Maintenance</h1></center>

## Content

- [Introduction](#Introduction)
- [Quickstart](#Quickstart) (Maintenance)
- [Installation](#Installation)
- [How to Run](#How-To-Run)
- [Technology](#Techonology)
- [Folder Structure](#Folder-Structure)

## Introduction 

# Threat Detector

Website layanan deteksi ancaman yang dibangun dengan *Python* dan *Flask*.

---

## 📋 Prasyarat

Pastikan perangkat kamu telah terinstall:

- *Python* versi *3.x* atau lebih tinggi
- *Virtual Environment* untuk Python
- *XAMPP* (untuk menjalankan web server di localhost)
- *Code Editor* (disarankan *Visual Studio Code* atau *PyCharm*)
- *Terminal/Command Prompt*

*Jika belum menginstall XAMPP, kamu bisa mengunduhnya (https://www.apachefriends.org/).*

---

## 🚀 Cara Instalasi

1. *Pastikan Python terinstall*:
   - Unduh Python (https://www.python.org/downloads/), pastikan versi 3.x atau lebih tinggi.
2. *Clone Repository*:
   - bash
   git clone -b main https://github.com/Syndrom2211/magang-alfian.git

3. *Gunakan Virtual Environment*:
   - Buat environment dengan perintah: 
     ```bash
     python -m venv nama_environment_kamu
     ```
     Lihat dokumentasi lebih lanjut (https://docs.python.org/3/library/venv.html).

4. *Install dependencies*:
   - Setelah environment aktif, install dependencies dengan perintah:
     ```bash
     pip install -r requirements.txt
     ```

5. *Install XAMPP*:
   - Unduh XAMPP (https://www.apachefriends.org/) dan jalankan server web di localhost.

---

## 💻 Cara Menjalankan Aplikasi

1. *Jalankan server XAMPP*:
   - Buka XAMPP Control Panel dan aktifkan Apache dan MySQL.

2. *Buat database*:
   - Buat database baru bernama `yuk_mari` di phpMyAdmin

3. *Aktifkan virtual environment*:
   - Di terminal, jalankan perintah:
     ```bash
     source venv/Scripts/Activate
     ```
     atau di terminal Windows:
     ```bash
     .\venv\Scripts\Activate
     ```

4. *Jalankan aplikasi*:
   - Di terminal jalankan:
    python ./run.py

5. *Akses aplikasi*:
   - Buka browser dan akses aplikasi di: 
     (http://localhost:1337)

6. *Stop aplikasi dan server*:
   - Tekan `Ctrl + C` untuk menghentikan aplikasi dan server.
  
7. *Akun Demo*
   - Username : admin@example.com
   - Password : password321

---

## 🛠️ Teknologi yang Digunakan

- *Flask*
- *Python*
- *SQLAlchemy*
- *MySQL*

---

## 📁 Struktur Folder



## Folder Structure
```
app/
│── models
│   │── log.py (maintenance)          
│   │── payload.py (maintenance)
│   │── user.py (maintenance)
│── routes
│   │── auth.py (maintenance)          
│   │── logs.py (maintenance)
│   │── main.py (maintenance)
│── static/  
│   │── img/ (maintenance)          
│   │── backup/ (maintenance)                 
│   │── css/ (maintenance)          
│   │── js/ (maintenance)
│   │── payload/
│── templates/
│   │── account_settings.html (maintenance)
│   │── buy.html (maintenance)
│   │── client.html (maintenance)
│   │── dashboard.html (maintenance)
│   │── login.html (maintenance)
│   │── export.html (maintenance)
│   │── import.html (maintenance)
│   │── resetpass.html (maintenance)
│   │── testing.html (maintenance)
── utils
│   │── __init__.py (maintenance)          
│   │── config.py (maintenance)
│   │── idsServer.py (maintenance)
│── logs.txt
env/
README.md
requirements.txt
run.py


---

## ✏️ Cara Mengedit

### 1️⃣ Komponen

- Buka folder `app/`.
- Edit file komponen yang diinginkan, seperti `run.py` atau `idsServer.py`.

### 2️⃣ Styling

- Buka folder `static/css/`.
- Edit file CSS untuk styling global.

### 3️⃣ Payload

- Buka folder `static/payload/`.
- Edit file payload sesuai kebutuhan aplikasi.

### 4️⃣ Database

- Buat atau ubah data di `phpMyAdmin` menggunakan database `yuk_mari`.

---

## 🔧 Troubleshooting

### 1️⃣ Jika terjadi error saat instalasi:

```bash
pip install --force-reinstall -r requirements.txt
