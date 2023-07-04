
# Removal_Background

Perkenalkan nama saya Muhammad Reviansyah Danendra Putra NIM 202131160, disini saya akan menjelaskan apa yang telah saya buat, berikut adalah penjelasan nya : 

Import library: Pertama, saya mengimport library cv2 untuk OpenCV dan numpy sebagai np untuk manipulasi array. Kemudian Fungsi remove_background: Fungsi ini menerima image_path sebagai parameter, yang merupakan path file gambar yang ingin dihapus latar belakangnya. Dan Membaca gambar: Saya membaca gambar menggunakan fungsi cv2.imread dan mengonversi format warna dari BGR (default OpenCV) ke RGB menggunakan cv2.cvtColor. Konversi menjadi grayscale: Gambar RGB dikonversi menjadi citra grayscale menggunakan cv2.cvtColor.

Ambang citra (Thresholding): Menggunakan metode Otsu, saya mengambil nilai ambang untuk memisahkan objek dari latar belakang. Hasilnya disimpan dalam threshold. Operasi opening: Menggunakan operasi morfologi opening untuk menghilangkan noise pada gambar menggunakan cv2.morphologyEx. Temukan kontur objek: Menggunakan cv2.findContours, saya menemukan kontur objek pada gambar yang telah diolah.

Buat mask kosong: Saya membuat mask kosong dengan ukuran yang sama dengan gambar asli. Gambar kontur objek pada mask: Menggunakan cv2.drawContours, saya menggambar kontur objek pada mask yang telah dibuat sebelumnya. Terapkan mask ke gambar asli: Dengan menggunakan operasi bitwise AND (cv2.bitwise_and), saya menerapkan mask ke gambar asli untuk menghapus latar belakang.

Tampilkan gambar hasil: Menggunakan cv2.imshow, saya menampilkan gambar hasil dalam jendela. Simpan gambar hasil: Hasilnya disimpan dalam format PNG menggunakan cv2.imwrite. Nama file hasil disesuaikan dengan result_path yang ditentukan.Contoh penggunaan: Terakhir, saya memanggil fungsi remove_background dengan menyediakan path file gambar yang ingin diproses

Dengan menggunakan metode segmentasi berdasarkan perbedaan citra, kode tersebut menghasilkan gambar dengan latar belakang yang dihapus dan menyimpan gambar hasil dalam format PNG sesuai dengan ketentuan yang berikan.


