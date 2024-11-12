# tekieemob

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


## TUGAS 7

1. Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget, dan jelaskan perbedaan dari keduanya.

    Dalam Flutter, ada dua jenis widget utama: 

    -  Stateless Widget 
        
        Stateless Widget adalah widget yang tidak memiliki keadaan yang bisa berubah. Artinya, setelah widget ini ditampilkan, ia akan tetap sama dan tidak bisa berubah selama aplikasi berjalan. Jika ingin membuat tampilan yang sederhana dan statis (tidak perlu diperbarui atau diperbarui hanya sekali), maka gunakan stateless widget.

        contoh : Jika kita membuat widget yang hanya menampilkan teks sederhana seperti "Halo, dunia!" dan tidak ada interaksi atau perubahan pada teks tersebut, ini adalah contoh penggunaan stateless widget.

    - Stateful Widget

        Stateful Widget adalah widget yang memiliki keadaan yang bisa berubah seiring waktu atau sebagai hasil dari interaksi pengguna. Dengan kata lain, stateful widget bisa diperbarui kapan saja selama aplikasi berjalan. Jika memiliki elemen yang dinamis atau bisa berubah, maka gunakan stateful widget.

        contoh : Misalkan kita memiliki tombol yang, ketika ditekan, akan mengubah warna atau menambah angka. Karena ada perubahan yang bisa terjadi setiap kali tombol ditekan, maka widget ini harus bisa diubah (dinamis) dan akan menjadi stateful widget.

2. Sebutkan widget apa saja yang kamu gunakan pada proyek ini dan jelaskan fungsinya.

    Pada proyek ini, terdapat beberapa widget utama yang digunakan untuk membangun antarmuka aplikasi. Berikut penjelasan masing-masing widget dan fungsinya:
    
    1. Scaffold
        
        Fungsi: Scaffold adalah widget dasar untuk membangun struktur halaman di Flutter. Ia menyediakan kerangka halaman dengan komponen seperti AppBar, Body, dan FloatingActionButton.
        
        Penggunaan di proyek: Digunakan untuk membuat struktur utama halaman, di mana terdapat AppBar di bagian atas dan body di tengah yang memuat konten utama halaman.

    2. AppBar

        Fungsi: AppBar adalah widget yang berfungsi sebagai bagian atas halaman (bar atas) dan biasanya menampilkan judul atau elemen navigasi.

        Penggunaan di proyek: Menampilkan judul aplikasi "Tekieemob" dengan warna teks putih dan background dari tema aplikasi.


    3. Padding
    
        Fungsi: Padding memberikan jarak atau ruang di sekitar widget lain. Ia sangat berguna untuk mengatur tata letak agar lebih rapi
    
        Penggunaan di proyek: Memberikan ruang di sekitar Column pada body dan juga di sekitar teks selamat datang, agar tampilan lebih tertata dan nyaman dilihat.

    4. Column
    
        Fungsi: Column digunakan untuk menampilkan widget secara vertikal. Ia menyusun widget satu di atas yang lain dari atas ke bawah.
    
        Penggunaan di proyek: Menyusun beberapa widget seperti Row, SizedBox, dan GridView secara vertikal di dalam body halaman.

    5. Row
    
        Fungsi: Row digunakan untuk menampilkan widget secara horizontal. Ia menyusun widget dari kiri ke kanan.
    
        Penggunaan di proyek: Menampilkan tiga InfoCard secara horizontal di bagian atas body.

    6. SizedBox
    
        Fungsi: SizedBox adalah widget yang berfungsi sebagai spacer atau memberikan jarak antar-widget. Ia dapat ditentukan ukurannya (tinggi atau lebar) untuk membuat ruang kosong di antara elemen.
    
        Penggunaan di proyek: Memberikan jarak vertikal antara Row yang berisi InfoCard dan bagian berikutnya di Column.

    7. GridView.count
    
        Fungsi: GridView.count menampilkan widget dalam bentuk grid atau tabel dengan jumlah kolom yang tetap.
    
        Penggunaan di proyek: Menampilkan ItemCard dalam bentuk grid dengan 3 kolom agar tombol-tombol ditampilkan dalam tata letak yang rapi.

    8. Card
    
        Fungsi: Card digunakan untuk membuat kotak dengan bayangan di bawahnya. Ia sering digunakan untuk membuat komponen yang memiliki batas tepi dan sedikit bayangan agar terlihat menonjol.
        
        Penggunaan di proyek: Membangun struktur InfoCard yang menampilkan informasi seperti NPM, Nama, dan Kelas dalam sebuah kotak dengan bayangan.
    
    9. Container
    
        Fungsi: Container adalah widget serbaguna yang bisa digunakan untuk mengatur ukuran, padding, margin, warna, dan dekorasi dari elemen di dalamnya.
        
        Penggunaan di proyek: Membuat kotak dalam Card untuk menampilkan InfoCard dan juga di dalam ItemCard untuk menempatkan ikon dan teks secara rapi di tengah.

    10. Center
        
        Fungsi: Center digunakan untuk menempatkan widget di tengah secara horizontal dan vertikal di dalam parent-nya.
        
        Penggunaan di proyek: Menyusun kolom berisi teks sambutan dan GridView di tengah halaman.

    11. Text
        
        Fungsi: Text menampilkan teks di layar.
        
        Penggunaan di proyek: Menampilkan teks seperti judul di AppBar, teks sambutan, dan informasi di InfoCard dan ItemCard.
    
    12. Icon
    
        Fungsi: Icon digunakan untuk menampilkan ikon (simbol grafis) dari pustaka ikon Flutter.
        
        Penggunaan di proyek: Menampilkan ikon untuk setiap ItemCard, seperti ikon mood, add, dan logout.
    
    13. Material
    
        Fungsi: Material memberikan latar belakang dengan efek material (misalnya warna dan elevasi) yang biasa digunakan pada kartu atau tombol.
        Penggunaan di proyek: Memberikan efek material dengan warna dan sudut melengkung pada ItemCard.     
    
    14. InkWell
        
        Fungsi: InkWell adalah widget yang menambahkan efek ripple (gelombang) ketika elemen di-klik. Ia sering digunakan untuk menambahkan interaksi pada elemen yang bisa ditekan.
        
        Penggunaan di proyek: Menangani interaksi ketika ItemCard ditekan oleh pengguna, dan juga menampilkan SnackBar sebagai respons ketika pengguna menekan tombol.
    
    15. SnackBar
    
        Fungsi: SnackBar menampilkan pesan sementara di bagian bawah layar. Pesan ini sering digunakan untuk memberi tahu pengguna setelah suatu aksi dilakukan.
        
        Penggunaan di proyek: Menampilkan pesan sementara ketika pengguna menekan ItemCard sebagai feedback dari aksi yang dilakukan.

3. Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.

    Dalam Flutter, setState() adalah fungsi yang digunakan dalam Stateful Widgets untuk memperbarui tampilan (UI) ketika data atau variabel tertentu berubah. Fungsi ini memberi tahu framework bahwa ada sesuatu yang berubah dalam state widget, sehingga widget harus diperbarui atau dirender ulang. setState() digunakan untuk memberitahu Flutter bahwa ada perubahan pada variabel di dalam state widget. Ketika setState() dipanggil, Flutter akan merender ulang widget yang bersangkutan dengan memperbarui tampilan sesuai dengan perubahan variabel yang terjadi. Hanya widget yang berada dalam StatefulWidget yang memiliki akses ke fungsi ini, karena widget statis (StatelessWidget) tidak memiliki state yang bisa berubah.
    
    Cara Kerja setState()
    
    Perbarui Nilai Variabel: Di dalam setState(), kita memperbarui nilai dari variabel-variabel tertentu yang ingin diubah.
    Render Ulang UI: Setelah setState() dipanggil, Flutter secara otomatis merender ulang bagian yang terpengaruh oleh variabel yang berubah sehingga tampilan sesuai dengan data terbaru.
    
    Hanya variabel yang berada dalam state dari StatefulWidget yang dapat terdampak dengan fungsi setState(). Variabel-variabel ini harus didefinisikan sebagai bagian dari state (bukan variabel yang bersifat final atau const dalam widget). Hanya perubahan yang terjadi di dalam fungsi setState() yang akan memicu render ulang. Jika variabel diperbarui di luar setState(), Flutter tidak akan merender ulang tampilan.

4. Jelaskan perbedaan antara const dengan final.

    Dalam Dart, const dan final adalah kata kunci yang digunakan untuk mendefinisikan variabel yang nilainya tidak akan berubah setelah diinisialisasi. Namun, ada perbedaan penting dalam cara kerja keduanya:

    - const
        
        const digunakan untuk membuat nilai yang sudah diketahui dan tetap pada waktu kompilasi. Artinya, nilai ini harus bisa dihitung atau ditentukan saat kode dikompilasi, bukan saat aplikasi berjalan. Variabel const tidak bisa diubah setelah ditetapkan, dan objek yang dibuat dengan const bersifat immutabel (tidak dapat diubah). const digunakan ketika kita ingin mendefinisikan nilai yang akan tetap sama di seluruh siklus hidup aplikasi, seperti const pi = 3.14;. Jika ada dua objek const yang identik, Dart akan menyimpannya hanya sekali di memori, sehingga lebih hemat.

        Contoh:

        ```
        const int daysInWeek = 7;
        const double pi = 3.14159;
        ```
        
        Pada contoh di atas, daysInWeek dan pi adalah const, artinya nilainya tetap dan tidak akan berubah selama aplikasi berjalan.

    - final

        final digunakan untuk membuat nilai yang diinisialisasi sekali dan tidak dapat diubah setelah diinisialisasi, tetapi nilainya bisa ditentukan saat runtime (waktu aplikasi berjalan). final cocok digunakan ketika kita ingin mendefinisikan nilai yang hanya akan diketahui saat aplikasi berjalan, seperti waktu sistem atau input pengguna yang ditetapkan sekali dan tidak berubah. Meskipun variabel final tidak bisa diubah, jika nilai yang ditetapkan adalah objek (seperti list atau map), data di dalam objek masih bisa berubah.

        Contoh:

        ```
        final DateTime currentDate = DateTime.now();
        final List<String> cities = ['New York', 'London'];
        ```
            
        Pada contoh di atas currentDate adalah final, karena waktu sistem saat ini hanya bisa diketahui saat aplikasi berjalan. cities adalah final, artinya list cities tidak dapat diubah ke list lain, tetapi elemen di dalam list masih bisa diubah, seperti cities.add('Tokyo');.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist-checklist di atas

    1. Membuat proyek Flutter baru dengan nama tekieemob
    2. Merapikan struktur proyek dengan membuat file baru bernama menu.dart pada direktori tekieemob/lib, mengimpor paket Material Design yang disediakan oleh Flutter di menu.dart serta memindahkan class MyHomePage dan class _MyHomePageState dari main.dart ke menu.dart. Tidak lupa untuk mengimpor modul menu.dart agar main.dart mengenali class MyHomePage
    3. Mengubah tema warna aplikasi pada main.dart dalam MaterialApp
    4. Mengubah sifat widget halaman menu menjadi stateless dengan mengubah "const MyHomePage(title: 'Flutter Demo Home Page')" pada main.dart menjadi "MyHomePage(),". Lalu mengubah sifat widget halaman dari stateful menjadi stateless dengan menghapus semua isi dari class MyHomePage, mengubah extends dari StatefulWidget ke StatelessWidget, menambahkan MyHomePage({super.key}); sebagai constructor class MyHomePage, menghapus seluruh class class _MyHomePageState, serta menambahkan Widget build.

        ```
        class MyHomePage extends StatelessWidget {
            MyHomePage({super.key});

            @override
            Widget build(BuildContext context) {
	            return Scaffold(
	    
	            );
            }
        }
        ```

    5. Membuat card sederhana yang berisi npm, nama, dan kelas dengan cara mendeklarasikan tiga variabel bertipe string yang berisi NPM, nama, dan kelas pada class MyHomePage di menu.dart dan membuat class baru bernama InfoCard pada berkas menu.dart untuk membuat card sederhana yang akan menampilkan informasi NPM, nama, dan kelas.
    6. Membuat button card sederhana dengan icon dengan cara membuat class baru bernama ItemHomepage yang berisi atribut-atribut dari card, membuat list of ItemHomepage yang berisi tombol-tombol yang ingin ditambahkan pada class MyHomePage (tombol-tombol dengan warna berbeda untuk setiap tombol), dan membuat class ItemCard untuk menampilkan tombol-tombol tersebut yang apabila tombol ditekan akan menampilkan snackbar yang berisi pesan "Kamu telah menekan tombol [nama button]".

        ```
        class ItemHomepage {
            final String name;
            final IconData icon;
            final Color color;

            ItemHomepage(this.name, this.icon, this.color);
        }
        ```

        ```
        class MyHomePage extends StatelessWidget {
            ...

            final List<ItemHomepage> items = [
                ItemHomepage("Lihat Daftar Produk", Icons.mood, Colors.brown),
                ItemHomepage("Tambah Produk", Icons.add, Colors.brown.shade700),
                ItemHomepage("Logout", Icons.logout, Colors.brown.shade900),
            ];
            ...
        }
        ```

    7. Mengintegrasikan InfoCard dan ItemCard agar ditampilkan di MyHomePage dengan cara mengubah bagian Widget build() pada class MyHomePage
    8. Melakukan flutter analyze untuk memastikan tidak ada isu-isu pada kode yang dapat mengganggu performa atau fungsionalitas aplikasi.


## TUGAS 8

1. Apa kegunaan const di Flutter? Jelaskan apa keuntungan ketika menggunakan const pada kode Flutter. Kapan sebaiknya kita menggunakan const, dan kapan sebaiknya tidak digunakan?

    Di Flutter, kata kunci const digunakan untuk membuat objek yang nilainya tidak bisa diubah (immutable) dan hanya dibuat satu kali di memori. Ketika kita menandai suatu objek dengan const, Flutter akan menghemat memori dan meningkatkan kinerja aplikasi karena objek tersebut tidak dibuat ulang setiap kali dipanggil, melainkan hanya menggunakan satu instance yang sama. Ini sangat berguna jika kita memiliki widget atau elemen UI yang tidak akan berubah, seperti teks atau ikon statis. Dengan const, kompilator Dart juga dapat melakukan optimalisasi, sehingga aplikasi berjalan lebih cepat.
    
    Penggunaan const sebaiknya diterapkan pada objek yang sifatnya tetap, misalnya teks yang tidak berubah atau padding yang konsisten di berbagai bagian aplikasi. Ini membantu menjaga aplikasi tetap efisien dan rapi. Namun, jika objek tersebut mengandalkan data dinamis yang mungkin berubah selama aplikasi berjalan, seperti data yang bergantung pada status (state) atau variabel yang akan diperbarui, kita tidak perlu menggunakan const. Contohnya, jika kita menampilkan Text yang isinya bergantung pada nama pengguna yang bisa berubah, kita cukup menggunakan Text tanpa const. Dengan memahami kapan menggunakan const, kita bisa membuat aplikasi yang lebih ringan dan responsif. 

2. Jelaskan dan bandingkan penggunaan Column dan Row pada Flutter. Berikan contoh implementasi dari masing-masing layout widget ini!

    Di Flutter, Column dan Row adalah widget dasar yang digunakan untuk menyusun elemen UI secara vertikal dan horizontal. Column digunakan untuk menata widget atau elemen secara vertikal, dari atas ke bawah, sementara Row digunakan untuk menata elemen secara horizontal, dari kiri ke kanan. Jadi, jika kita ingin menempatkan elemen-elemen UI dalam satu baris (sejajar), kita menggunakan Row. Sebaliknya, jika kita ingin elemen-elemen tersebut tersusun bertumpuk (di bawah satu sama lain), kita menggunakan Column.

    Misalnya, jika kita ingin menampilkan tiga teks secara vertikal (bertumpuk), kita bisa menggunakan Column seperti ini:

    ```
    Column(
        crossAxisAlignment: CrossAxisAlignment.start,
        children: [
            Text('Name: $_name'),
            Text('Description: $_description'),
            Text('Amount: $_amount'),
        ],
    ),
    ```

    Hasilnya, ketiga teks tersebut akan muncul satu di bawah lainnya.

    Sementara itu, jika kita ingin menampilkan tiga teks secara horizontal (bersebelahan), kita menggunakan Row seperti ini:
    ```
    Row(
        mainAxisAlignment: MainAxisAlignment.spaceEvenly,
        children: [
            InfoCard(title: 'NPM', content: npm),
            InfoCard(title: 'Name', content: name),
            InfoCard(title: 'Class', content: className),
        ],
    ),
    ```
    Dengan Row, ketiga InfoCard akan tampil sejajar dari kiri ke kanan. Perlu diingat, Column dan Row juga bisa dikombinasikan untuk membuat layout yang lebih kompleks. Misalnya, kita bisa meletakkan Row di dalam Column atau sebaliknya, sehingga memungkinkan untuk membuat susunan elemen yang lebih bervariasi dan fleksibel.

3. Sebutkan apa saja elemen input yang kamu gunakan pada halaman form yang kamu buat pada tugas kali ini. Apakah terdapat elemen input Flutter lain yang tidak kamu gunakan pada tugas ini? Jelaskan!

    Pada halaman form yang saya buat dalam tugas ini, saya menggunakan tiga elemen input utama: TextFormField untuk Name, Description, dan Amount. TextFormField ini memungkinkan pengguna memasukkan teks atau angka yang nantinya bisa divalidasi sesuai ketentuan, seperti memastikan nama dan deskripsi memiliki jumlah karakter tertentu dan hanya berisi karakter yang valid, serta memastikan Amount berupa angka. Di samping itu, ada tombol ElevatedButton yang berfungsi sebagai tombol Save untuk menyimpan data yang diisi pada form.

    Flutter sebenarnya menyediakan banyak elemen input lain yang bisa digunakan sesuai kebutuhan. Misalnya, ada DropdownButton untuk menampilkan pilihan dropdown, Checkbox untuk memilih opsi ya atau tidak, Radio untuk memilih satu pilihan dari beberapa opsi, Slider untuk mengatur nilai dengan cara menggeser, dan Switch untuk mengaktifkan atau menonaktifkan sesuatu. Meskipun elemen-elemen tersebut sangat berguna, saya tidak menggunakannya dalam tugas ini karena form yang saya buat hanya membutuhkan input teks dan angka sederhana. Namun, elemen-elemen input lainnya akan sangat membantu untuk form yang lebih kompleks atau membutuhkan pilihan beragam.

4. Bagaimana cara kamu mengatur tema (theme) dalam aplikasi Flutter agar aplikasi yang dibuat konsisten? Apakah kamu mengimplementasikan tema pada aplikasi yang kamu buat?

    Pada aplikasi Flutter, pengaturan tema (Theme) dilakukan agar tampilan aplikasi menjadi konsisten dan mudah diatur. Dengan menggunakan tema, kita bisa menentukan warna-warna utama (seperti warna utama dan warna aksen), font, serta gaya elemen UI lainnya yang diterapkan di seluruh aplikasi. Dalam kode saya, tema diatur melalui ThemeData pada properti theme di dalam MaterialApp. Di sini, saya mengatur colorScheme dengan menggunakan ColorScheme.fromSwatch, yang memungkinkan saya untuk memilih primarySwatch dengan warna coklat (Colors.brown) sebagai warna utama, dan warna aksen menggunakan Colors.brown[600]. Dengan cara ini, semua bagian aplikasi yang mengikuti tema utama akan otomatis menyesuaikan ke warna coklat yang konsisten tanpa perlu menentukannya satu per satu.

    Menggunakan tema seperti ini sangat membantu agar aplikasi tetap seragam dan mudah untuk diperbarui jika suatu saat kita ingin mengganti gaya atau warna. Sebagai contoh, jika saya ingin mengganti warna tema utama, saya cukup mengganti primarySwatch, dan seluruh aplikasi akan mengikuti perubahan tersebut. Pada aplikasi yang saya buat, saya mengimplementasikan tema dengan cara ini agar aplikasi memiliki tampilan yang seragam dan terlihat profesional.

5. Bagaimana cara kamu menangani navigasi dalam aplikasi dengan banyak halaman pada Flutter?

    Dalam aplikasi Flutter yang memiliki banyak halaman, navigasi ditangani menggunakan widget Navigator. Navigator berfungsi sebagai pengelola tumpukan halaman (stack), sehingga kita bisa menambah halaman baru di atas halaman saat ini atau menggantinya. Pada program saya, saya menggunakan Navigator.push dan Navigator.pushReplacement. Ketika Navigator.push digunakan, halaman baru akan ditambahkan di atas halaman saat ini, sehingga pengguna bisa kembali ke halaman sebelumnya dengan tombol "Back". Misalnya, ketika saya menekan item menu "Tambah Produk," Navigator.push membuka halaman ProductEntryFormPage di atas halaman sebelumnya.

    Sementara itu, Navigator.pushReplacement digunakan untuk mengganti halaman saat ini dengan halaman baru, tanpa menyimpan halaman lama di tumpukan. Contohnya, saat saya memilih "Halaman Utama," Navigator.pushReplacement mengganti halaman dengan MyHomePage, sehingga pengguna tidak bisa kembali ke halaman sebelumnya menggunakan tombol "Back." Selain itu, saya juga menggunakan Navigator.pop untuk menutup dialog atau halaman saat ini dan kembali ke halaman sebelumnya. Dengan cara ini, navigasi antarhalaman dalam aplikasi bisa diatur dengan rapi dan mudah, membuat aplikasi lebih nyaman digunakan.