🛑 Robot Penghindar Manusia Berbasis YOLO
Proyek ini merupakan sistem robot cerdas yang mampu mendeteksi dan menghindari manusia secara otomatis menggunakan model deteksi objek YOLO (You Only Look Once).

📌 Deskripsi Proyek
Robot ini dirancang untuk bergerak secara otonom dan menghindari keberadaan manusia di sekitarnya demi menjaga keamanan atau privasi. Sistem memanfaatkan model YOLOv5, YOLOv8, dan YOLOv11 untuk melakukan deteksi manusia secara real-time melalui kamera yang terpasang pada robot.

Setelah manusia terdeteksi, robot akan:

Menganalisis posisi manusia

Mengubah arah atau jalur untuk menghindari tabrakan atau interaksi

Tetap berada dalam jalur aman dan efisien

🔧 Teknologi yang Digunakan
Python

YOLOv5, YOLOv8, YOLOv11 (.pt model terlampir)

OpenCV untuk pengolahan gambar

Jupyter Notebook (main.ipynb) untuk pengujian dan pengembangan

Hardware robot (seperti Raspberry Pi + kamera + motor driver) [opsional tergantung implementasi]

🧠 Model Deteksi yang Digunakan
Model YOLO yang digunakan:

yolov5s.pt

yolov5su.pt

yolov8n.pt

yolo11l.pt

yolo11n.pt

yolo11s.pt

Model ini telah dilatih untuk mendeteksi keberadaan manusia dengan akurasi tinggi.

📂 Struktur Folder
bash
Copy
Edit
.
├── BNU5/                   # Folder tambahan (mungkin berisi notebook/tools)
├── .gitignore
├── main.ipynb             # Notebook utama untuk menjalankan deteksi
├── yolo11l.pt             # Model deteksi YOLOv11 (large)
├── yolo11n.pt             # Model deteksi YOLOv11 (nano)
├── yolo11s.pt             # Model deteksi YOLOv11 (small)
├── yolov5s.pt             # YOLOv5s pretrained
├── yolov5su.pt            # YOLOv5s hasil update/training
├── yolov8n.pt             # YOLOv8 nano
📄 Dokumentasi Lengkap
Untuk penjelasan lebih detail tentang konsep, metode, dan pengujian sistem, silakan lihat dokumentasi lengkap di Google Drive:

📎 Dokumentasi Robot Penghindar Manusia :
[https://drive.google.com/file/d/1AzDlB6s3XTBVsAl3H7hDty0vNzaM6mb-/view?usp=drive_link](url)
