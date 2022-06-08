Nama : Muhammad Ardi Abdurrahman

Kelas : TI.20.D1

NIM : 312010075

Matkul : Pemograman Web

Untuk mengaktifkan ekstentsi tersebut, melalu XAMPP Control Panel, pada bagian Apache klik Config -> PHP.ini

![1](https://user-images.githubusercontent.com/101821904/172716404-fa3da035-eb92-43b3-9c68-661fcc5a6281.png)
![2](https://user-images.githubusercontent.com/101821904/172716496-bcba590d-e55b-4228-93aa-32a22a351308.png)


Unduh Codeigniter dari website https://codeigniter.com/download Extrak file zip Codeigniter ke direktori htdocs/lab11_ci. Ubah nama direktory framework-4.x.xx menjadi ci4. Buka browser dengan alamat http://localhost/lab11_ci/ci4/public
![3](https://user-images.githubusercontent.com/101821904/172716517-5e36866f-45f4-4c42-b6f8-62540bff0e0d.png)

Menjalankan CLI (Command Line Interface) Codeigniter 4 menyediakan CLI untuk mempermudah proses development. Untuk mengakses CLI buka terminal/command prompt.
![44](https://user-images.githubusercontent.com/101821904/172716557-8788ed2f-215d-40ca-805b-e38b92f8694b.png)

Arahkan lokasi direktori sesuai dengan direktori kerja project dibuat (xampp/htdocs/lab11_ci/ci4/) Perintah yang dapat dijalankan untuk memanggil CLI Codeigniter adalah: php spark
![5](https://user-images.githubusercontent.com/101821904/172716602-3330da3f-0e44-4a3e-bac3-d971f837a25c.png)

Semua jenis error akan ditampilkan sama. Untuk memudahkan mengetahui jenis errornya, maka perlu diaktifkan mode debugging dengan mengubah nilai konfigurasi pada environment variable CI_ENVIRINMENT menjadi development.
![6](https://user-images.githubusercontent.com/101821904/172716655-c468ea33-5b14-4049-8aeb-fd138fc10bf1.png)
![7](https://user-images.githubusercontent.com/101821904/172716679-da471983-d325-4343-928b-bfaa178cd278.png)

Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode.
![8](https://user-images.githubusercontent.com/101821904/172716711-eb6a5add-2494-4789-a341-f7993f7df7cb.png)

Struktur Direktori Untuk lebih memahami Framework Codeigniter 4 perlu mengetahui struktur direktori dan file yang ada. Buka pada Windows Explorer atau dari Visual Studio Code -> Open Folder.
![9](https://user-images.githubusercontent.com/101821904/172716765-07e86a0f-c5e4-43f9-9c0c-f517e0c38013.png)

Router terletak pada file app/config/Routes.php
![10](https://user-images.githubusercontent.com/101821904/172716802-a042adef-5ef5-42b0-a27d-2b44446640e1.png)

Membuat Route Baru. Tambahkan kode berikut di dalam Routes.php $routes->get('/about', 'Page::about'); $routes->get('/contact', 'Page::contact'); $routes->get('/faqs', 'Page::faqs');
![11](https://user-images.githubusercontent.com/101821904/172716847-33753c3d-02ec-439d-a5ec-58ebaf7ed504.png)

php spark routes
![12](https://user-images.githubusercontent.com/101821904/172716885-6df07c1f-65ad-44b5-8795-d762dfffcc7e.png)
![13](https://user-images.githubusercontent.com/101821904/172716935-ef4e904c-d513-46aa-b956-ecb54b73c14d.png)

Membuat Controller
![14](https://user-images.githubusercontent.com/101821904/172716998-74b35b3c-e61d-4f0c-83b1-3e28bc11bf52.png)

Hasil browser
![15](https://user-images.githubusercontent.com/101821904/172717036-58cc4bd9-5cc1-4728-a377-f7ecaf1eaae2.png)

Tambahkan method baru pada Controller Page seperti berikut.
![16](https://user-images.githubusercontent.com/101821904/172717070-882bbb58-f29e-4968-8acc-d10fdb97df2c.png)

![17](https://user-images.githubusercontent.com/101821904/172717095-ffd8a5fd-f962-4d40-9bf3-2008d28a54c0.png)

Membuat View Selanjutnya adalam membuat view untuk tampilan web agar lebih menarik. Buat file baru dengan nama about.php pada direktori view (app/view/about.php) kemudian isi kodenya seperti berikut.
![18](https://user-images.githubusercontent.com/101821904/172717169-506568f1-a436-44c5-a8bb-4194c065675b.png)

Ubah method about pada class Controller Page menjadi seperti berikut:
![19](https://user-images.githubusercontent.com/101821904/172717201-abb6c7f5-81d4-4a58-9ed3-ca12b22f8213.png)

Hasil browser
![20](https://user-images.githubusercontent.com/101821904/172717226-785254a9-0204-4787-82cb-e2025a4698f1.png)

Buat file css pada direktori public dengan nama style.css (copy file dari praktikum lab4_layout. Kita akan gunakan layout yang pernah dibuat pada praktikum 4.
![a](https://user-images.githubusercontent.com/101821904/172717577-6ca0aa7d-a177-420e-a187-ef131b50416b.png)

Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php File app/view/template/header.php
![21](https://user-images.githubusercontent.com/101821904/172717682-0ec630eb-9235-44d5-a15c-6da6df32bcee.png)

File app/view/template/footer.php
![22](https://user-images.githubusercontent.com/101821904/172717851-3cf5d0d2-3d84-46c9-93c3-42cb1ab614e1.png)
![23](https://user-images.githubusercontent.com/101821904/172717889-6e86037f-c258-47a8-b887-48f9ff6f1c2e.png)

Pertanyaan dan Tugas Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.
![24](https://user-images.githubusercontent.com/101821904/172717928-c42bc05d-f64d-431a-bc23-41f9ad650f5c.png)

About
![25](https://user-images.githubusercontent.com/101821904/172717992-2db9206a-7e5b-4db7-a794-1599b2306292.png)
