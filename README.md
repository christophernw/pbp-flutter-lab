# Tugas 7 PBP

## Identitas
Nama    : Christopher Nathanael Wijaya<br>
NPM     : 2106630044<br>
Kelas   : E

## Jawaban dari Pertanyaan
### Stateless dan Stateful Widget
*Stateless widget* merupakan *widget* yang statis atau tidak dapat diubah *state*-nya sekali di-*built*. Contoh nya adalah `Text` dan `Icon` <br>

*Stateful widget* merupakan *widget* yang dinamis atau dapat berubah-ubah *state*-nya dalam
sekali *built*. Contoh nya adalah `CheckBox`, `RadioButton`, dan `TextField`.

### Widget yang Digunakan
Pada proyek ini, berikut *widget* yang saya gunakan dan fungsinya:
1. `Scaffold`: *widget* utama yang menjadi struktur *layout* halaman aplikasi dan sebagai 
wadah untuk menampung semua *widget* lainnya pada halaman aplikasi
2. `AppBar`: *widget* yang berfungsi untuk menampilkan *app bar* sebuah halaman aplikasi, umumnya
diletakkan pada bagian paling atas dari sebuah halaman aplikasi dan dapat berisi *widget* lain
3. `Text`: *widget* yang berfungsi untuk menampilkan teks pada halaman aplikasi
4. `Center`: *widget* yang berfungsi untuk menampilkan *child widget*-nya menjadi di tengah
5. `Column`: *widget* yang berfungsi untuk menampilkan *children widget*-nya secara vertikal
6. `Row`: *widget* yang berfungsi untuk menampilkan *children widget*-nya secara horizontal
7. `FloatingActionButton`: *widget* yang berfungsi untuk menampilkan tombol yang dapat mengeksekusi suatu
fungsi tertentu ketika ditekan oleh pengguna
8. `Icon`: *widget* yang berfungsi untuk menampilkan *icon* tertentu yang sudah *predefined*
9. `MaterialApp`: *widget* yang dijalankan pertama kali ketika eksekusi fungsi `main()` dan berfungsi 
untuk *wrapping* *widget* lain yang diimplementasikan dengan `Material Design` pada halaman aplikasi

### setState()
`setState()` memberitahu *framework* akan perubahan *state*, *framework* akan merespon dengan meng-*update* *state* lalu me-*render* ulang *widget* tersebut. Pada tugas 7 ini, variabel `_counter` diubah dalam `setState`.

### Const dan Final
*Keyword* `final` berfungsi untuk menandai bahwa nilai dari suatu variabel tidak akan pernah berubah selama
jalannya aplikasi dan tidak ada operasi yang dapat mengubah nilai tersebut. Dengan menggunakan *keyword* `final`,
proses assignment untuk suatu variabel terjadi pada masa *run-time*. Sementara itu, konsep dari *keyword* `const`
mirip dengan `final`, hanya saja `const` akan membuat variabel menjadi *compile-time constant*, atau proses
*assignment* pada variabel tersebut akan terjadi pada masa *compile-time*.

### Tahap-Tahap Implementasi Checklist
Tahapan yang saya lakukan dalam mengimplementasikan checklist:
1. Membuat suatu proyek baru dengan nama `counter_7`.
2. Mengubah `title` pada `MyHomePage` menjadi "Program Counter".
3. Membuat fungsi `_decrementCounter()` pada `_MyHomePageState` yang berfungsi untuk mengurangi *counter* selama belum bernilai 0.
4. Membuat *floating action button* tambahan untuk mengurangi *counter*. dan melakukan modifikasi pada `FloatingActionButton` tersebut dengan mengatur `onPressed` dengan fungsi yang sesuai.
5. Melakukan modifikasi pada `Container` untuk `floatingActionButton` dengan menambahkan *padding*.
6. Membuat fungsi yang menampilkan `Text` yang muncul jika *counter* bernilai ganjil ataupun genap dan menambahkan parameter `style` pada *widget* `Text` dengan nilai `TextStyle(color: Colors.blue)` atau `TextStyle(color: Colors.red)`
7. Menambahkan `if (_counter != 0)` sebelum `FloatingActionButton` untuk menghilangkan `FloatingActionButton` dari layar jika *counter* bernilai 0.
8. Menambahkan parameter `textDirection` dengan nilai `TextDirection.rtl` untuk *reverse* urutan tampilan tombol, agar ketika tombol *decrement* hilang, tombol *increment* tidak berubah tempat.
9. Melakukan `add`, `commit`, dan `push` ke GitHub.
