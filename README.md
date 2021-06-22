# Lab11Web
Sebelum memulai menggunakan Framework Codeigniter, perlu dilakukan konfigurasi pada webserver. Beberapa ekstensi PHP perlu diaktifkan untuk kebutuhan pengembangan Codeigniter 4. Dengan cara di bawah ini:
Hapus tanda ; (titik koma) pada bagian extension yang akan diaktifkan.
![Screenshot_1](https://user-images.githubusercontent.com/52759649/122889949-743d4300-d36d-11eb-9688-d5a4b965b087.jpg)
Selanjutnya instalasi CodeIgniter 4
Codeigniter dapat didownload dari website https://codeigniter.com/download
Extrak file zip Codeigniter ke direktori htdocs/lab11_php_ci
Ubah nama direktory framework-4.x.xx menjadi ci4
Buka browser dengan alamat http://localhost/lab11_php_ci/ci4/public/
![Screenshot_3](https://user-images.githubusercontent.com/52759649/122891504-c6329880-d36e-11eb-9cb1-2aad8243874a.jpg)
Codeigniter menyediakan CLI, untuk mengaksesnya buka terminal lalu arahkan ke direktori project yang akan dibuat. Kemudian jalankan perintah php spark untuk memanggil CLI codeigniter.
![Screenshot_4](https://user-images.githubusercontent.com/52759649/122891582-d34f8780-d36e-11eb-8da6-96fec3627b15.jpg)
Codeigniter juga menyediakan mode debugging/development yang dapat menampilkan error/kesalahan dalam kode program. Cara mengaktifkannya dengan mengubah nama file env menjadi .env kemudian buka filenya dan ubah nilai CI_ENVIRONMENT menjadi development.
![Screenshot_5](https://user-images.githubusercontent.com/52759649/122892210-67215380-d36f-11eb-8902-7b3e6cf8699f.jpg)
Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode.
![Screenshot_6](https://user-images.githubusercontent.com/52759649/122892288-73a5ac00-d36f-11eb-9c7d-7ef4c3fa32c5.jpg)
![Screenshot_7](https://user-images.githubusercontent.com/52759649/122892618-bcf5fb80-d36f-11eb-9e1d-8f1d115adb2a.jpg)
Membuat Route. Router terletak pada file app/config/Routes.php Untuk mengetahui route yg ada atau telah berjalan dapat menggunakan perintah php spark routes.
![Screenshot_9](https://user-images.githubusercontent.com/52759649/122893156-4279ab80-d370-11eb-8667-cb4cb555d44d.jpg)
Selanjutnya mencoba akses route yang telah dibuat dengan mengakses http://localhost/lab11_php_ci/ci4/public/about
Terjadi error file not found dikarenakan tidak ada file/page untuk halaman contact.
![Screenshot_10](https://user-images.githubusercontent.com/52759649/122893600-ab612380-d370-11eb-94fc-25862bcca10b.jpg)
Membuat Controller, Membuat file page.php di dalam direktori Controller (/app/Controllers)
Kemudian refresh browser maka halaman sudah dapat diakses dan menampilkan hasilnya.
![Screenshot_11](https://user-images.githubusercontent.com/52759649/122894242-38a47800-d371-11eb-8894-7b8f30a5f7a5.jpg)
Auto Routing Secara default fitur autoroute pada Codeiginiter sudah aktif. Untuk mengubah status autoroute dapat mengubah nilai variabelnya. Untuk menonaktifkan ubah nilai true menjadi false.
![Screenshot_12](https://user-images.githubusercontent.com/52759649/122895587-72c24980-d372-11eb-9727-e54f226dd5b2.jpg)
Membuat View Membuat file about.php di dalam direktori View (/app/view/about.php)
![Screenshot_13](https://user-images.githubusercontent.com/52759649/122895692-8ff71800-d372-11eb-8312-33f814bc82c9.jpg)
Membuat Layout Web dengan CSS
Buat file css pada direktori public dengan nama style.css (copy file dari praktikum lab4_layout).
Kemudian buat folder template pada direktori view, lalu buat file header.php dan footer.php
![Screenshot_14](https://user-images.githubusercontent.com/52759649/122896002-d6e50d80-d372-11eb-8c19-9265d58b8f12.jpg)
