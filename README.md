# **Pemrograman Mobile Pertemuan Minggu 12**

| Nama  :   | Haidar Aly |
| :--------: | :-------: |

| Kelas :  | TI-3F    |
| :--------: | :-------: |

| Absen : |  09  |
| :--------: | :-------: |

| NIM   :  | 2241720258   |
| :--------: | :-------: |

## Praktikum 1

### Soal 1 - Tambahkan nama panggilan Anda pada title app sebagai identitas hasil pekerjaan Anda. Gantilah warna tema aplikasi sesuai kesukaan Anda.

> ```dart
> class MyApp extends StatelessWidget {
>  const MyApp({super.key});
>
>  @override
>  Widget build(BuildContext context) {
>    return MaterialApp(
>      title: 'Stream Haidar',
>      theme: ThemeData(
>        primarySwatch: Colors.deepOrange,
>      ),
>      home: const StreamHomePage(),
>    );
>  }
> }
> ```

### Soal 2 - Tambahkan 5 warna lainnya sesuai keinginan Anda pada variabel colors tersebut.
> ```dart
> class ColorStream {
>   final List<Color> colors = [
>     Colors.blueGrey,
>     Colors.amber,
>     Colors.deepPurple,
>     Colors.lightBlue,
>     Colors.teal,
>     Colors.red,
>     Colors.cyan,
>     Colors.green,
>     Colors.black,
>     Colors.pink,
>   ];
> }
> ```

### Soal 3 - Jelaskan fungsi keyword yield* pada kode tersebut! Apa maksud isi perintah kode tersebut?
> Kode tersebut membuat stream yang menghasilkan nilai setiap satu detik. Nilai yang dihasilkan adalah warna dari daftar `colors` berdasarkan indeks yang dihitung dari waktu `t` modul panjang daftar `colors`. Dengan kata lain, setiap detik, stream akan mengeluarkan warna berikutnya dalam daftar secara berurutan.