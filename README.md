# Lab2Web
1. Contoh penggunaan CSS dengan menambahkan properti-properti dari Cheat Sheet:
![Screenshot (73)1](https://github.com/user-attachments/assets/a1a99926-ce80-4634-b11e-561f2aa5948d)
![Screenshot (73)1](https://github.com/user-attachments/assets/c1e75ff5-ebb7-4e80-b233-8fedf73ce3bc)

Hasil:
![Screenshot (72)1](https://github.com/user-attachments/assets/69baf694-f15e-443a-8c75-653dadaf34f4)

2. Perbedaan Deklarasi CSS h1 {...} dan #intro h1 {...}:

Deklarasi h1 {...} mengacu pada semua elemen h1 yang ada di dalam dokumen HTML. Setiap elemen h1 di halaman akan mengikuti aturan CSS yang dideklarasikan di dalam blok tersebut.

Deklarasi #intro h1 {...} lebih spesifik. Ini hanya berlaku pada elemen h1 yang ada di dalam elemen dengan id="intro". Jadi, aturan ini tidak akan memengaruhi semua elemen h1, hanya yang berada di dalam elemen yang memiliki ID intro.
Contoh:
![Screenshot (78)1](https://github.com/user-attachments/assets/76c76111-d744-4cb0-be68-5a1bde4e7fdf)

Pada contoh di atas, elemen h1 di dalam #intro akan mengikuti deklarasi dari #intro h1 {...}, sedangkan elemen h1 lainnya mengikuti deklarasi h1 {...}.

3. Jika ada deklarasi CSS yang sama pada internal, eksternal, dan inline, maka urutan prioritas yang ditampilkan pada browser adalah sebagai berikut:

Inline CSS (paling tinggi)
Internal CSS
Eksternal CSS (paling rendah)
Contoh:
![Screenshot (79)1](https://github.com/user-attachments/assets/4c0d3b1e-8837-4d6d-9f05-6f1de23f2dd1)

Hasil:
![Screenshot (75)2](https://github.com/user-attachments/assets/a25c521e-17fa-4356-9cdf-c266beb28a11)

xternal CSS (dari file styles.css) mungkin mengatur paragraf menjadi warna lain, tetapi jika internal CSS mengatur paragraf menjadi color: blue;, dan inline CSS mengatur color: red;, maka inline CSS akan menang, dan teks paragraf akan berwarna merah di browser.

4. Perbedaan Selector ID dan Class:
Jika elemen HTML memiliki ID dan class, ID memiliki prioritas lebih tinggi daripada class. Jadi, jika ada konflik antara aturan CSS ID dan class, aturan yang ditentukan oleh ID akan menang.
Contoh:
![Screenshot (77)1](https://github.com/user-attachments/assets/dbe42439-9e58-4a16-92e4-c05f1504e326)

Hasil:
![Screenshot (75)3](https://github.com/user-attachments/assets/69d5a3c5-1935-482f-8c60-f78b6643f07e)
Pada contoh di atas:

ID #paragraf-1 mendefinisikan warna teks menjadi hijau dan ukuran font menjadi 20px.
Class .text-paragraf mendefinisikan warna teks menjadi biru dan ukuran font menjadi 18px.
Karena ID memiliki prioritas lebih tinggi daripada class, paragraf akan ditampilkan dengan warna hijau dan ukuran font 20px, sesuai dengan aturan ID, meskipun class juga mendeklarasikan properti yang sama.

Kesimpulan: Selector dengan ID lebih spesifik daripada selector dengan class, sehingga aturan pada ID akan mengalahkan class jika keduanya mendeklarasikan properti yang sama.


