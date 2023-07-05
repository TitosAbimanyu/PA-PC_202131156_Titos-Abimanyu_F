
# Remove Background Menggunakan OpenCV

## Dasar Teori
### I. Landasan Teori
Salah satu teknik penting dalam pengolahan gambar dan pengenalan objek adalah penghapusan latar belakang gambar. Kami memperkenalkan metode penghapusan latar belakang menggunakan library OpenCV, yang merupakan library sumber terbuka yang menawarkan berbagai fungsi dan algoritma untuk pengolahan gambar. Makalah ini juga menjelaskan langkah-langkah yang diperlukan untuk menggunakan algoritma pemrosesan citra yang tersedia dalam OpenCV, dan kami juga memberikan contoh implementasi kode yang dapat digunakan untuk menghapus latar belakang.

### II. Pejelasan
Penghapusan latar belakang gambar adalah proses menghilangkan piksel-piksel yang mewakili latar belakang dari gambar. Hal ini berguna dalam berbagai aplikasi seperti pengenalan objek, penggabungan gambar, dan augmentasi data. OpenCV adalah library yang populer dalam pemrosesan gambar dan menyediakan berbagai algoritma dan fungsi yang dapat digunakan untuk menghapus latar belakang gambar.

OpenCV adalah open source C++ library untuk image processing dan computer vision. Secara teori OpenCV digunakan seperti meniru cara kerja sistem visual manusia yaitu dengan melihat objek melalui "penglihatan/mata" dan citra pada objek tersebut diteruskan ke otak untuk memproses sehingga mengerti objek apa yang tampak pada pandangan mata manusia. OpenCV merupakan salah satu cabang Artificial intellegent (kecerdasan buatan) yang digunakan untuk pengembangan atau analisis isi suatu gambar. Menghitung jumlah obyek dalam sebuah wadah menggunakan cara yang manual membuang waktu cukup lama, terutama jika obyek tersebut bergerak atau makhluk hidup. Kesalahan dalam menghitung akan sering terjadi dan dapat merugikan salah satu pihak, maka dibutuhkan aplikasi yang dapat menghitung jumlah obyek bergerak lebih mudah dan menghemat waktu. Dengan memanfaatkan teknologi Android, user dapat menggunakan aplikasi dimana saja. Program ini ditunjukan pada penjual ikan atau nelayan yang menjual ikan dalam jumlah yang besar dan menghitung ikan satu persatu bukanlah pilihan, mereka pun menjualnya dengan mempertimbangkan berat dan memperkirakan perkilonya berisi sekian ikan hingga tidak adanya kepastian berapa jumlah ikan yang dibeli. Kesalahan dalam menghitung dapat merugikan salah satu pihak dari penjual maupun pembeli. Oleh karena itu dilakukan penelitian untuk membantu masalah tersebut dengan merancang suatu aplikasi counting objek bergerak dengan menggunakan OpenCV pada Smartphone.

## Penjelasan Program
### Metode Penghapusan Latar Belakang menggunakan OpenCV
Dalam metode ini, kami menggunakan pendekatan berbasis perbedaan citra (image differencing) untuk mengidentifikasi piksel-piksel yang mewakili latar belakang. Langkah-langkahnya adalah sebagai berikut:
   a. Membaca gambar asli dan gambar latar belakang.
   b. Mengubah gambar ke ruang warna yang sesuai (misalnya, RGB atau HSV).
   c. Menghitung perbedaan absolut antara gambar asli dan gambar latar belakang.
   d. Melakukan thresholding pada perbedaan absolut untuk mendapatkan gambar biner yang menunjukkan piksel-piksel yang berbeda.
   e. Mengaplikasikan operasi morfologi seperti dilasi dan erosi untuk membersihkan gambar biner.
   f. Menggunakan hasil gambar biner sebagai mask untuk menghapus latar belakang pada gambar asli.

#### Implementasi Kode
Berikut adalah contoh implementasi kode dalam bahasa pemrograman Python menggunakan library OpenCV:

import cv2
def remove_background(image_path, background_path):

    # Membaca gambar asli dan gambar latar belakang
    image = cv2.imread(image_path)
    background = cv2.imread(background_path)

    # Mengubah gambar ke ruang warna yang sesuai

    # Menghitung perbedaan absolut antara gambar asli dan gambar latar belakang

    # Melakukan thresholding pada perbedaan absolut

    # Melakukan operasi morfologi untuk membersihkan gambar biner

    # Menggunakan hasil gambar biner sebagai mask untuk menghapus latar belakang pada gambar asli

    # Menampilkan gambar hasil

    # Memanggil fungsi remove_background dengan gambar asli dan gambar latar belakang
    remove_background('gambar_asli.jpg', 'gambar_latar_belakang.jpg')

![image](https://github.com/TitosAbimanyu/PA-PC_202131156_Titos-Abimanyu_F/assets/114853614/7f465f13-b499-4638-a7d3-176da3a0785b)


## Kesimpulan
Penghapusan latar belakang gambar merupakan teknik yang penting dalam bidang pengolahan gambar. Dalam makalah ini, kami memperkenalkan metode penghapusan latar belakang menggunakan library OpenCV dalam bahasa pemrograman Python. Kami menjelaskan langkah-langkah yang diperlukan untuk menghapus latar belakang gambar menggunakan algoritma pemrosesan citra yang tersedia dalam OpenCV. Implementasi kode yang diberikan memberikan contoh bagaimana teknik ini dapat diterapkan dalam praktik. Metode ini dapat digunakan dalam berbagai aplikasi yang membutuhkan penghapusan latar belakang gambar.
