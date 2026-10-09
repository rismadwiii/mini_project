# mini_project
Mini Project: OCR Nomor Ijazah dan Deteksi Tanda Tangan

Deskripsi

Mini-project ini bertujuan untuk menerapkan pengolahan citra pada gambar ijazah untuk membaca nomor ijazah menggunakan Optical Character Recognition (OCR) dan mendeteksi keberadaan tanda tangan kepala sekolah.

Sistem menggunakan beberapa metode peningkatan kualitas citra untuk membantu proses pembacaan karakter. Selain itu, dilakukan thresholding dan operasi morphology untuk mendukung proses deteksi tanda tangan.

Tujuan

Menerapkan teknik image enhancement pada citra ijazah.

Membaca nomor ijazah menggunakan OCR.

Mendeteksi keberadaan tanda tangan kepala sekolah.

Membandingkan hasil OCR menggunakan nilai Character Error Rate (CER).

Metode

1. Image Enhancement

Metode yang digunakan:

Grayscale

CLAHE

Histogram Equalization

Contrast Stretching

2. Optical Character Recognition (OCR)

Tesseract OCR digunakan untuk mengenali karakter pada area nomor ijazah yang telah dipotong secara manual.

3. Deteksi Tanda Tangan

Proses deteksi tanda tangan meliputi:

Grayscale

Global Thresholding

Otsu Thresholding

Morphological Opening dan Closing

Analisis piksel foreground untuk menentukan status tanda tangan.

4. Evaluasi OCR

Evaluasi dilakukan menggunakan Character Error Rate (CER) untuk membandingkan hasil OCR dengan teks acuan. Semakin rendah nilai CER, semakin baik hasil pembacaan karakter.

Hasil Pengujian

Pada pengujian citra yang dilakukan, metode Grayscale, CLAHE, dan Contrast Stretching menghasilkan CER sebesar 0,0000. Sementara itu, Histogram Equalization menghasilkan OCR kosong dengan CER sebesar 1,0000.

Pada pengujian deteksi tanda tangan, sembilan citra berlabel PRESENT berhasil terdeteksi sebagai PRESENT. Pengujian ini belum mencakup citra tanpa tanda tangan.

Teknologi

Python

OpenCV

NumPy

Pandas

Pytesseract

Tesseract OCR

Dataset

Dataset terdiri dari sembilan citra ijazah dengan variasi kualitas, antara lain:

High Quality

Low Contrast

Blurred

High Noise

Low Resolution

Faded atau Underexposed

Color Shift

JPEG Compression Artifacts

Combined Degradation
