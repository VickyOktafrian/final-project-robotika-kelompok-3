# 🛑 Robot Penghindar Manusia Berbasis YOLO

Proyek ini merupakan sistem robot cerdas yang mampu mendeteksi dan menghindari manusia secara otomatis menggunakan model deteksi objek YOLO (You Only Look Once).

## 📌 Deskripsi Proyek

Robot ini dirancang untuk bergerak secara otonom dan menghindari keberadaan manusia di sekitarnya demi menjaga keamanan atau privasi. Sistem memanfaatkan model YOLOv5, YOLOv8, dan YOLOv11 untuk melakukan deteksi manusia secara real-time melalui kamera yang terpasang pada robot.

### Cara Kerja Robot

Setelah manusia terdeteksi, robot akan:
1. 🔍 Menganalisis posisi manusia
2. 🔄 Mengubah arah atau jalur untuk menghindari tabrakan atau interaksi
3. ✅ Tetap berada dalam jalur aman dan efisien

## 🔧 Teknologi yang Digunakan

- **Python** - Bahasa pemrograman utama
- **YOLOv5, YOLOv8, YOLOv11** - Model deteksi objek (.pt model terlampir)
- **OpenCV** - Pengolahan gambar dan computer vision
- **Jupyter Notebook** - Environment pengembangan dan testing
- **Hardware Robot** - Raspberry Pi + kamera + motor driver (opsional)

## 🧠 Model Deteksi YOLO

Model YOLO yang tersedia dalam proyek ini:

| Model | Ukuran | Deskripsi |
|-------|--------|-----------|
| `yolov5s.pt` | Small | YOLOv5 versi ringan |
| `yolov5su.pt` | Small Updated | YOLOv5 hasil training/update |
| `yolov8n.pt` | Nano | YOLOv8 versi paling ringan |
| `yolo11l.pt` | Large | YOLOv11 versi besar (akurasi tinggi) |
| `yolo11n.pt` | Nano | YOLOv11 versi ringan |
| `yolo11s.pt` | Small | YOLOv11 versi sedang |

Model-model ini telah dilatih untuk mendeteksi keberadaan manusia dengan akurasi tinggi.

## 📂 Struktur Proyek

```
.
├── BNU5/                   # Folder tambahan (notebook/tools pendukung)
├── .gitignore             # File pengaturan Git
├── main.ipynb             # 📓 Notebook utama untuk menjalankan deteksi
├── yolo11l.pt             # 🤖 Model YOLOv11 Large
├── yolo11n.pt             # 🤖 Model YOLOv11 Nano
├── yolo11s.pt             # 🤖 Model YOLOv11 Small
├── yolov5s.pt             # 🤖 Model YOLOv5 Small
├── yolov5su.pt            # 🤖 Model YOLOv5 Small Updated
├── yolov8n.pt             # 🤖 Model YOLOv8 Nano
└── README.md              # 📖 Dokumentasi proyek
```

## 🚀 Cara Menjalankan

### Prerequisites

Pastikan Anda telah menginstall:
- Python 3.7+
- Jupyter Notebook
- OpenCV
- PyTorch
- Ultralytics YOLO

### Instalasi Dependencies

```bash
pip install torch torchvision
pip install opencv-python
pip install ultralytics
pip install jupyter
```

### Menjalankan Proyek

1. Clone repository ini
2. Buka `main.ipynb` menggunakan Jupyter Notebook
3. Jalankan sel-sel kode secara berurutan
4. Pastikan kamera terhubung dengan baik
5. Pilih model YOLO yang ingin digunakan

## 🎯 Fitur Utama

- ✅ Deteksi manusia real-time menggunakan multiple model YOLO
- ✅ Sistem penghindaran otomatis
- ✅ Interface yang mudah digunakan melalui Jupyter Notebook
- ✅ Support multiple model YOLO (v5, v8, v11)
- ✅ Optimized untuk berbagai ukuran hardware

## 📊 Performa Model

| Model | Kecepatan | Akurasi | Penggunaan RAM | Rekomendasi |
|-------|-----------|---------|----------------|-------------|
| YOLOv11n | ⚡⚡⚡ | ⭐⭐ | Rendah | Raspberry Pi |
| YOLOv11s | ⚡⚡ | ⭐⭐⭐ | Sedang | PC Standard |
| YOLOv11l | ⚡ | ⭐⭐⭐⭐⭐ | Tinggi | PC High-end |

## 🔗 Dokumentasi Lengkap

Untuk penjelasan lebih detail tentang konsep, metode, dan pengujian sistem, silakan lihat dokumentasi lengkap:

📎 **[Dokumentasi Robot Penghindar Manusia](https://drive.google.com/file/d/1AzDlB6s3XTBVsAl3H7hDty0vNzaM6mb-/view?usp=drive_link)**

## 🤝 Kontribusi

Kontribusi sangat diterima! Silakan:
1. Fork repository ini
2. Buat branch fitur baru (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📝 Lisensi

Proyek ini menggunakan lisensi MIT. Lihat file `LICENSE` untuk detail lengkap.

## 👨‍💻 Author

**Irsyad Fadhil Makarim**
**Mikhail Shams Afzal Karim** 
**Albi Akhsanul Hakim**
**Kalfin Syah Kilau Mayya**
**Muhamad Vicky Oktafrian**

## 🙏 Acknowledgments

- Tim Ultralytics untuk model YOLO
- OpenCV community
- Kontributor open source lainnya
