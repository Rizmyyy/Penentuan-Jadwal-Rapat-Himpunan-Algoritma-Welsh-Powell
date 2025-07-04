# Penentuan-Jadwal-Rapat-Himpunan-Algoritma-Welsh-Powell
Repositori ini menyajikan implementasi solusi penjadwalan menggunakan Algoritma Welsh-Powell dan teori graf. Proyek ini bertujuan untuk mengoptimalkan penentuan waktu rapat himpunan mahasiswa dengan menganalisis dan memodelkan konflik jadwal mata kuliah.
# Penentuan Jadwal Rapat Himpunan Menggunakan Algoritma Welsh-Powell Berbasis Pewarnaan Graf

## Deskripsi Proyek
Proyek ini mengimplementasikan Algoritma Welsh-Powell untuk menyelesaikan permasalahan penjadwalan rapat himpunan mahasiswa. Dengan memanfaatkan konsep pewarnaan graf dari matematika diskrit, proyek ini bertujuan untuk menemukan slot waktu yang optimal dan bebas konflik untuk rapat, berdasarkan data jadwal perkuliahan yang kompleks. Pendekatan ini dirancang untuk meningkatkan efisiensi dan objektivitas dalam proses penjadwalan.

## Latar Belakang Masalah
Himpunan mahasiswa memiliki peran krusial di kampus sebagai wadah aspirasi dan pengembangan diri. [cite_start]Namun, penentuan jadwal rapat sering kali terkendala oleh bentrok jadwal kuliah anggota dari berbagai semester dan kelas[cite: 21, 22]. [cite_start]Penjadwalan manual memakan waktu, rentan kesalahan, dan dapat menyebabkan partisipasi rendah[cite: 23, 24]. [cite_start]Untuk mengatasi ini, dibutuhkan pendekatan sistematis dan efisien, di mana teori graf, khususnya pewarnaan graf, terbukti efektif dalam masalah penjadwalan seperti penyusunan jadwal perkuliahan[cite: 25, 26, 27, 28].

## Metodologi Penelitian
Penelitian ini mengikuti langkah-langkah sebagai berikut:
1.  [cite_start]**Identifikasi Masalah**: Menemukan kendala dalam penyusunan jadwal rapat himpunan mahasiswa, yaitu kesulitan menentukan waktu yang bebas bentrok dengan jam kuliah[cite: 103, 104, 105].
2.  [cite_start]**Studi Pustaka**: Mengkaji literatur untuk menemukan metode yang relevan, yaitu pewarnaan graf (graph coloring), yang dapat menghindari konflik penjadwalan[cite: 107, 108, 109].
3.  [cite_start]**Pengumpulan Data**: Mengumpulkan data primer berupa pembagian jadwal perkuliahan mahasiswa Informatika, serta data sekunder dari jurnal dan buku[cite: 95, 96, 97]. [cite_start]Data yang dikumpulkan meliputi mata kuliah, durasi, dan hari perkuliahan[cite: 112, 113, 114].
4.  **Analisis Data & Pembentukan Graf**: Mengonversi data jadwal kuliah ke dalam bentuk graf. [cite_start]Setiap mata kuliah yang berpotensi konflik direpresentasikan sebagai simpul (vertex), dan hubungan antar mata kuliah yang tidak dapat terjadi bersamaan direpresentasikan sebagai sisi (edge)[cite: 116, 117, 118]. [cite_start]Graf ini kemudian direpresentasikan dalam bentuk matriks ketetanggaan[cite: 119]. [cite_start]Batas jam rapat ditetapkan pukul 18.00 WIB, dan hanya program studi Informatika yang digunakan[cite: 139, 140].
5.  [cite_start]**Pewarnaan Graf**: Menerapkan Algoritma Welsh-Powell pada graf yang telah dibentuk[cite: 121]. [cite_start]Setiap warna mewakili satu slot waktu yang berbeda, dan pewarnaan dilakukan sedemikian rupa agar tidak ada dua simpul yang terhubung memiliki warna yang sama (tidak ada bentrok jadwal)[cite: 123].
6.  [cite_start]**Penetapan Jadwal Rapat & Kesimpulan**: Menganalisis hasil pewarnaan graf untuk menemukan slot waktu kosong minimal 2 jam yang tersedia sebelum pukul 18:00 WIB[cite: 376, 383].
## Cara Menjalankan Kode
Untuk menjalankan kode di repositori ini, Anda memerlukan lingkungan Python dengan library yang spesifik. Direkomendasikan menggunakan Google Colab atau Jupyter Notebook.

### Prasyarat
Pastikan Anda memiliki Python (versi 3.x direkomendasikan) terinstal. Anda dapat menginstal library yang dibutuhkan menggunakan `pip`:
```bash
pip install networkx matplotlib pandas
Langkah-langkah
Klon Repositori:

Bash

git clone [https://github.com/Rizmyyy/Penentuan-Jadwal-Rapat-Himpunan-Algoritma-Welsh-Powell.git](https://github.com/Rizmyyy/Penentuan-Jadwal-Rapat-Himpunan-Algoritma-Welsh-Powell.git)
cd Penentuan-Jadwal-Rapat-Himpunan-Algoritma-Welsh-Powell
Buka Jupyter Notebook/Google Colab:

Jupyter Notebook: Jalankan jupyter notebook dari terminal di direktori root repositori, lalu navigasikan ke src/.

Google Colab: Unggah file .ipynb dari direktori src/ ke Google Drive Anda, lalu buka dengan Google Colab.

Jalankan Notebook: Buka graph_visualization.ipynb dan graph_coloring_and_analysis.ipynb secara berurutan dan jalankan setiap sel kode.

Hasil Penting
Dari analisis dan pewarnaan graf menggunakan Algoritma Welsh-Powell, ditemukan bahwa 

Hari Jumat pukul 15:00 - 18:00 WIB merupakan satu-satunya waktu yang memenuhi kriteria (minimal 2 jam dan sebelum pukul 18:00 WIB) dan tidak bertabrakan dengan jadwal kuliah lima kelas yang dianalisis (2 INF A, B, C dan 4 INF A, B). Waktu ini ditetapkan sebagai waktu resmi untuk pelaksanaan rapat rutin himpunan.
