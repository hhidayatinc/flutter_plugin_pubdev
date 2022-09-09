# flutter_plugin_pubdev

#22 | Pengenalan Plugin di Pub.Dev

1. Selesaikan Praktikum tersebut, lalu dokumentasikan dan push ke repository Anda berupa screenshot hasil pekerjaan beserta penjelasannya di file README.md!
![1](images/1.png)
Penjelasan:
- Pada saat langkah 4 terjadi error pada bagian code return AutoSizeText : text. Ini terjadi karena belum ada inisiasi untuk variabel tersebut. Maka diperluka inisiasi terlebih dahulu, seperti pada langkah 5.
Code:
final String text;
const RedTextWidget({Key? key, required this.text}) : super(key: key);
2. Jelaskan maksud dari langkah 2 pada praktikum tersebut!
- Langkah 2 menambahkan plugin baru pada project flutter. Di flutter bisa menambah plugin/package dengan perintah 'flutter pub add nama_plugin'.
Selain itu bisa juga langsung menambahkan pada bagian pubspec.yaml. Namun jika ditambahkan di file tersebut, maka harus menambahkan versi berapa.
3. Jelaskan maksud dari langkah 5 pada praktikum tersebut!
- Langkah 5 menunjukkan inisiasi untuk variabel text. Kemudian menambahkan parameter pada constructor kelas dengan inisiasi variabel text tadi.
const RedTextWidget({Key? key, required this.text}) : super(key: key);
4. Pada langkah 6 terdapat dua widget yang ditambahkan, jelaskan fungsi dan perbedaannya!
- Langkah 6 memiliki 2 widget yang berbeda. Jika pada widget container awal memiliki child yaitu widget RedTextWidget yang tadi sudah dibuat terlebih dahulu. Sedangkan container ke 2 memiliki child yaitu widget Text.
5. Jelaskan maksud dari tiap parameter yang ada di dalam plugin auto_size_text 
- maxLines: berfungsi untuk menentukan panjang text
- minFontSize & maxFontSize: berfungsi untuk menentukan font sekecil dan sebesar mungkin
- stepGranularity: berfungsi untuk mengurasi ukuran fontSize di setiap langkah
- presetFontSizes: berfungsi untuk menentukan ukuran font berapa aja yang diperbolehkan, maka minFontsize, maxFontSize, dan stepGranularity akan di abaikan
- overflowReplacement: berfungsi untuk mencegah text tidak bisa dibaca karena ukuran font yang terlalu kecil
- textAlign: mengatur posisi text, rata kiri, rata kanan, tengah, atau rata kiri kanan

