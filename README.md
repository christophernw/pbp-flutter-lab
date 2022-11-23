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

# Tugas 8 PBP

## Identitas
Nama    : Christopher Nathanael Wijaya<br>
NPM     : 2106630044<br>
Kelas   : E

## Jawaban dari Pertanyaan
### Perbedaan `Navigator.push` dan `Navigator.pushReplacement`
`Navigator.push` dan  `Navigator.pushReplacement` sama-sama mem-*push* sebuah *route* baru ke `Navigator` (yang pada dasarnya mirip dengan operasi *push* pada *Stack*). Namun, `Navigator.pushReplacement` akan menghapus *route* sebelumnya setelah *route* yang baru telah selesai *loading* dan sudah digunakan. Sehingga, *route* baru yang dipush dengan `Navigator.pushReplacement` akan menggantikan *route* lama yang sudah ada pada `Navigator`.

### Widget yang Digunakan
Berikut *widget* yang digunakan dan fungsinya:
1. `Scaffold`: *widget* utama yang menjadi struktur *layout* halaman aplikasi dan sebagai
   wadah untuk menampung semua *widget* lainnya pada halaman aplikasi
2. `AppBar`: *widget* yang berfungsi untuk menampilkan *app bar* sebuah halaman aplikasi, umumnya
   diletakkan pada bagian paling atas dari sebuah halaman aplikasi dan dapat berisi *widget* lain
3. `Text`: *widget* yang berfungsi untuk menampilkan teks pada halaman aplikasi
4. `Center`: *widget* yang berfungsi untuk menampilkan *child widget*-nya menjadi di tengah
5. `Column`: *widget* yang berfungsi untuk menampilkan *children widget*-nya secara vertikal
6. `Row`: *widget* yang berfungsi untuk menampilkan *children widget*-nya secara horizontal
7. `MaterialApp`: *widget* yang dijalankan pertama kali ketika eksekusi fungsi `main()` dan berfungsi
   untuk *wrapping* *widget* lain yang diimplementasikan dengan `Material Design` pada halaman aplikasi
8. `Expanded`: *widget* yang digunakan untuk memperluas *children widget* dari `Row`, `Column`, atau `Flex` sedemikian
    sehingga *child* tersebut mengisi tempat kosong yang tersedia
9. `Form`: *widget* yang bermanfaat dalam membungkus beberapa *form field widget* agar menjadi satu kesatuan
10. `TextFormField`: *widget* `TextField` yang terintegrasi dengan `Form`, berfungsi untuk menyediakan *field*
     bagi pengguna untuk memasukkan teks
11. `SizedBox`: *widget* berupa *box* yang bisa ditentukan ukurannya dan biasa digunakan untuk memberi jarak
     antara satu *widget* dengan *widget* lain
12. `DropdownButton`: *widget* tombol yang ketika ditekan oleh pengguna akan menampilkan *dropdown* yang dapat dipilih
13. `Align`: *widget* untuk mengatur posisi *widget* yang menjadi *child*-nya
14. `Padding`: *widget* untuk memberikan *padding* pada *widget* yang menjadi *child*-nya
15. `ListTile`: *widget* yang bersifat *single fixed-height row* yang umumnya digunakan sebagai *children* dari `ListView` atau
*column* untuk `Drawer`
16. `ListView`: *widget* *scrollable* untuk menampilkan *widget-widget* lain yang menjadi *children*-nya
17. `Dialog`: *widget* untuk menampilkan *pop up window* pada halaman aplikasi

### Jenis-Jenis Event yang Ada pada Flutter
Berikut adalah jenis-jenis *event* yang ada pada Flutter:
1. onEnter
2. onExit
3. onHover
4. onFocusChange
5. onTap
6. onPressed
7. onSaved
8. onChanged

### Cara Kerja Navigator Mengganti Halaman pada Flutter
Cara kerja `Navigator` dalam menampilkan halaman (dalam terminologi Flutter, bahasa yang tepat untuk term ini adalah *routes*) dapat diandaikan bekerja seperti struktur data *Stack*. 

Ketika perintah `Navigator.push` diberikan, maka *route* yang hendak di-*push* akan masuk ke atas *stack* `Navigator`. `Navigator` pun akan menampilkan *route* yang ada pada *top of stack*. Jika sebuah *route* baru di-*push* setelah itu, maka *route* baru itulah yang akan ada pada *top of stack* dan akan ditampilkan. *Route* yang sebelumnya ditampilkan akan berada di belakang *route* yang baru saja di-*push*.

Jika hendak menutup halaman/*route* yang ada pada *top of stack*, maka dapat menggunakan perintah `Navigator.pop`. *Route* yang akan mengeluarkan *route* yang sedang berada pada *top of stack*. Kemudian, *route* yang ada pada belakang *route* yang di-*pop* akan berada di *top of stack*, sehingga *route* tersebutlah yang akan ditampilkan ke pengguna.

### Tahap-Tahap Implementasi Checklist
Tahapan yang saya lakukan dalam mengimplementasikan checklist:
1. Membuat file `drawer.dart` yang berisi widget `Drawer` yang akan digunakan pada aplikasi. Drawer ini memiliki child berupa tiga buah `ListTile` yang ketika diklik dapat memindahkan halaman saat ini ke halaman lain.
2. Membuat file `form.dart` yang berisi implementasi halaman form. Pada halaman ini, dibuat suatu *stateless widget* berupa *card* budget yang akan ditampilkan pada halaman `Data Budget`.
3. Membuat suatu *stateful widget* untuk menyediakan form yang akan diisi oleh pengguna terkait detail
budget. Untuk implementasi form ini, widget `Form` digunakan untuk *wrap* tiga field yang diperlukan bagi pengguna
untuk menginput data, yaitu 'Judul', 'Nominal', dan 'Jenis'. Sementara itu, tombol `Simpan` diimplementasikan di luar widget `Form` agar posisinya bisa diatur menjadi di bawah page dengan memanfaatkan widget `Expanded` dan `Align`, di mana alignment akan diatur menjadi `bottomCenter`. Widget yang digunakan untuk memasukkan data 'Judul' dan 'Nominal' adalah `TextFormField`, sedangkan widget yang digunakan untuk memilih jenis budget adalah `DropdownButton`. Selanjutnya, untuk tiap event yang terjadi pada widget tersebut, diterapkan `setState()` untuk meng-*assign* nilai yang dimasukkan pengguna pada field ke variabel yang telah diinisialisasi.
4. Membuat tombol `Simpan`, menggunakan `TextButton`, di mana ketika tombol tersebut ditekan, akan dilakukan validasi input pengguna pada field yang bersesuaian. Jika sudah divalidasi, input dari pengguna akan dijadikan sebagai parameter widget `BudgetCard` seperti yang diimplementasikan pada langkah (2), untuk kemudian dimasukkan ke suatu list. Selanjutnya,untuk memberitahu pengguna bahwa datanya sudah masuk, ditampilkan widget `Dialog` yang berisi teks 'Data telah dimasukkan'.
5. Membuat file `data.dart` untuk menampilkan `BudgetCard` yang sudah dimasukkan ke list seperti yang telah dijelaskan pada langkah (4). Implementasi untuk menampilkan kumpulan `BudgetCard` ini memanfaatkan widget `ListView`.

# Tugas 9 PBP

## Identitas
Nama    : Christopher Nathanael Wijaya<br>
NPM     : 2106630044<br>
Kelas   : E

## Jawaban dari Pertanyaan
### Pengambilan Data JSON tanpa Model
Dapat dilakukan pengambilan data JSON tanpa menggunakan model. Tetapi, hal ini bukan merupakan suatu
*best practice*. Adanya model dapat membuat pengambilan data JSON menjadi lebih terstruktur, dalam hal ini
tiap *field* dari data menjadi properti dari class model tersebut yang sudah ditentukan tipe datanya, sehingga
ketika kita ingin mengakses data untuk *field* tersebut, kita cukup mengakses properti dari class model tersebut.

### Widget yang Digunakan
1. `Scaffold`: *widget* utama yang menjadi struktur *layout* halaman aplikasi dan sebagai
   wadah untuk menampung semua *widget* lainnya pada halaman aplikasi
2. `AppBar`: *widget* yang berfungsi untuk menampilkan *app bar* sebuah halaman aplikasi, umumnya
   diletakkan pada bagian paling atas dari sebuah halaman aplikasi dan dapat berisi *widget* lain
3. `Text`: *widget* yang berfungsi untuk menampilkan teks pada halaman aplikasi
4. `Center`: *widget* yang berfungsi untuk menampilkan *child widget*-nya menjadi di tengah
5. `Column`: *widget* yang berfungsi untuk menampilkan *children widget*-nya secara vertikal
6. `Row`: *widget* yang berfungsi untuk menampilkan *children widget*-nya secara horizontal
7. `MaterialApp`: *widget* yang dijalankan pertama kali ketika eksekusi fungsi `main()` dan berfungsi
   untuk *wrapping* *widget* lain yang diimplementasikan dengan `Material Design` pada halaman aplikasi
8. `Expanded`: *widget* yang digunakan untuk memperluas *children widget* dari `Row`, `Column`, atau `Flex` 
   sehingga *child* tersebut mengisi tempat kosong yang tersedia
9. `Padding`: *widget* untuk memberikan *padding* pada *widget* yang menjadi *child*-nya
10. `ListTile`: *widget* yang bersifat *single fixed-height row* yang umumnya digunakan sebagai *children* dari `ListView` atau
    *column* untuk `Drawer`
11. `ListView`: *widget* *scrollable* untuk menampilkan *widget-widget* lain yang menjadi *children*-nya
12. `FutureBuilder`: *widget* yang terbentuk berdasarkan *snapshot* terbaru dari `Future`.
13. `Card`: *widget* untuk menampilkan informasi tertentu, ditandai dengan adanya *rounded corner* dan *shadow* pada representasi visualnya.
14. `Checkbox`: *widget* untuk menampilkan *input field* berupa *checkbox*.
15. `Container`: *widget* yang digunakan untuk mendekorasi *widget* lain yang menjadi *child*-nya.
16. `Flexible`: *widget* yang mengatur flex dari child `Row`, `Column`, atau `Flex`.

### Mekanisme Pengambilan Data hingga Ditampilkan
Berikut adalah mekanisme pengambilan data hingga ditampillkan:
1. Membuat fungsi `Future` yang akan dipanggil saat menampilkan data dengan `FutureBuilder`.
2. Melakukan *parse* URL yang akan digunakan untuk pengambilan data.
3. Melakukan pengambilan data dengan menggunakan method `get` dari package `http` yang sudah diinstal berdasarkan
URL yang sudah di-*parse* tersebut.
4. Melakukan *decode* terhadap JSON yang sudah diambil agar bisa diakses nilainya secara langsung.
5. Memasukkan data JSON hasil *decode* ke *model class* yang telah dibuat untuk kemudian dimasukkan ke list dengan melakukan
loop di tiap data JSON tersebut.
6. Mengatur list yang berisi *instance* dari *model* tersebut sebagai *return value* dari fungsi `Future`.
7. Menginstansiasi `FutureBuilder` yang menerima parameter `future` berupa fungsi `Future` tersebut dan parameter
`builder` berupa *anonymous function* yang akan mengembalikan *widget* yang akan ditampilkan berdasarkan hasil
kembalian fungsi pada parameter `future` yang juga menjadi parameter `snapshot` pada *anonymous function* tersebut.
8. Mengatur *anonymous function* pada `builder` untuk mengembalikan *widget* yang untuk menampilkan data pada *snapshot*.
9. *Widget* tersebut akan ditampilkan dan berisi data sebagaimana yang didapatkan dari URL yang sudah ditentukan.

### Tahap-Tahap Implementasi Checklist
Tahapan yang saya lakukan dalam mengimplementasikan checklist:
1. Melakukan *refactor* terhadap file-file Dart sebelumnya dengan memindahkan ke direktori yang sesuai.
2. Membuat model class berdasarkan URL Tugas 3 menggunakan `QuickType`. Model tersebut kemudian dimasukkan ke
file `watchlist.dart` dan disimpan pada direktori `model`.
3. Menambahkan `http` package dan mengatur *internet permission* pada proyek.
4. Menambahkan `ListTile` baru pada `drawer.dart` sebagai navigasi ke page `My Watch List`.
5. Membuat file `fetch.dart` yang berisi fungsi untuk melakukan fetch data sebagaimana dijelaskan pada
bagian sebelumnya (Mekanisme Pengambilan Data hingga Ditampilkan) pada poin 1 sampai 6.
6. Membuat file `mywatchlist.dart` yang terhubung dengan `Navigator` pada `Drawer` untuk menampilkan page `My Watch List`.
7. Membuat `stateful widget` yang mengembalikan `Scaffold` sebagai struktur utama page. Pada `Scaffold` tersebut, terdapat
parameter `appBar` yang berisi judul page, parameter `drawer` yang berisi menu drawer sebagaimana pada file `drawer.dart`, dan
parameter `body` yang berisi `FutureBuilder`.
8. `FutureBuilder` berisi parameter `future` yang merupakan fungsi `Future` yang telah dibuat sebelumnya pada poin 4 dan parameter
`builder` yang berupa *anonymous function* yang akan mengembalikan *widget* yang akan ditampilkan berdasarkan hasil
kembalian fungsi pada parameter `future` yang juga menjadi parameter `snapshot` pada *anonymous function* tersebut.
9. Pada *anonymous function* tersebut, akan dibuat conditionals, jika data snapshot masih null, berarti akan ditampilkan
`CircularProgressIndicator()`. Jika data snapshot tidak null tetapi kosong (tidak ada data), maka akan ditampilkan
widget untuk menunjukkan bahwa tidak ada data. Jika data snapshot tidak null dan tidak kosong (datanya ada), maka akan
ditampilkan data tersebut dalam bentuk `ListView` menggunakan `builder`. 
10. Pada `ListView.builder` akan diatur `itemCount` sebagai jumlah data yang dikembalikan dan `itemBuilder` untuk membentuk
konten dari `ListView` tersebut.
11. `ListView` akan terdiri dari widget `Card` yang berisi judul film dan menambahkan child `InkWell` agar `Card` tersebut
dapat ditekan. Selanjutnya, ketika `Card` terus ditekan page akan berpindah ke page yang berisi detail dari film yang ditekan.
12. Pada `Card` tersebut, juga dilakukan kustomisasi border menjadi warna merah jika belum ditonton dan hijau jika sudah ditonton. 
13. Selain itu, ditambahkan pula `Checkbox` untuk mengubah status apakah suatu film sudah ditonton atau tidak secara lokal.
14. Untuk mengimplementasikan poin 12, dibuat suatu list yang berisi bool apakah suatu film sudah ditonton atau tidak. Selanjutnya,
perubahan status yang dilakukan pada `Checkbox` hanya diterapkan pada list itu saja.
15. Membuat file `watchlist_detail.dart` yang berisi widget untuk menampilkan detail dari film yang ditekan.
16. Membuat `stateless widget` yang menerima parameter `watchListFields` yang berisi data fields dari JSON yang didapatkan dan
parameter `status` yang merupakan status apakah suatu film sudah ditonton atau tidak (dari list yang dibuat pada tahap 13).
17. Pada widget tersebut, akan ditampilkan data yang sudah di-*pass* pada parameternya dalam bentuk `Column`.
18. Selanjutnya, dibuat fungsi untuk mengonversi format tanggal agar dapat ditampilkan dengan rapi.
19. Pada tiap children dari `Column`, akan ditampilkan data terkait film yang bersangkutan dengan menggunakan `Text.rich` dan `TextSpan`
untuk membuat *header* dari tiap field menjadi *bold*.
20. Selanjutnya, ditambahkan `ElevatedButton` di akhir page untuk kembali ke halaman `My Watch List` sebelumnya.
