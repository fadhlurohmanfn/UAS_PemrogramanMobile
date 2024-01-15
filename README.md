
<h1> MyApp</h1>

```
Nama    : Fadhlurohman Fatikh Navintino
Nim     : 312210368
Kelas   : TI.22.A4
Dosen   : Donny Maulana, S.Kom., M.M.S.I.
Link YT : [![UAS](https://img.youtube.com/vi/Gd9qLynNj5Y/0.jpg)](https://youtu.be/Gd9qLynNj5Y?si=3RP6WpyV2mSwqVnb)
```

## 1. **Splash Launcer**

- Kelas SplashActivity:
   - SPLASH_DELAY: Waktu penundaan layar pembuka (3000 milidetik).
- Metode onCreate:
   - Atur tampilan ke layout R.layout.activity_splash.
   - Sembunyikan status bar untuk tampilan layar penuh.
   - Gunakan Handler untuk penundaan sebelum beralih ke menu.
   - Metode openMenu:
- Buat Intent untuk pindah ke DashboardActivity.
- Mulai aktivitas baru dan tutup SplashActivity.

## 2. **Home Dashboard**

- Metode onCreate:
   - Atur tampilan ke layout R.layout.activity_dashboard.
   - Temukan semua elemen CardView dalam layout.
   - Set Click Actions untuk Setiap CardView:
- Atur tindakan klik untuk setiap CardView dengan membuat dan memulai intent untuk aktivitas terkait saat CardView diklik.
- Navigasi:
   - HelloCard: ke HelloActivity
   - FibonacciCard: ke FibonacciActivity
   - NewsCard: ke ScrollingIcecold
   - ChatCard: ke OneActivity
   - AlarmCard: ke AlarmActivity
   - MapsCard: ke MapActivity
   - FragmentCard: ke ViewPagerActivity
   - CountCard: ke MainActivity

## 3. **Hello**

- Turunan dari AppCompatActivity.
- Override metode onCreate untuk menetapkan tata letak (layout) ke R.layout.activity_hello.
- Override Metode onCreateOptionsMenu:
   - Membuat menu pada aktivitas.
   - Inflate menu dari file R.menu.activity_menu.
   - Override Metode onOptionsItemSelected


## 4. **Count**

- Variabel Kelas:
   - mShowCount: Sebuah objek TextView untuk menampilkan jumlah perhitungan.
   - currentCount: Sebuah variabel untuk menyimpan nilai perhitungan saat ini.
- Metode onCreate:
   - Inisialisasi tata letak (layout) dari aktivitas menggunakan R.layout.activity_main.
   - Inisialisasi TextView dengan ID show_count.

## 5. **News**

- Metode onCreate:
   - Dipanggil saat aktivitas dibuat.
   - Inisialisasi tata letak (layout) dari aktivitas menggunakan R.layout.activity_scrollicecold.
- Kelas ScrollingIcecold mewarisi dari AppCompatActivity.
- Metode onCreate mengatur layout aktivitas ke activity_scrollicecold.xml.

## 6. **Alarm**

- Penjelasan Tambahan:
   - Waktu alarm diatur menggunakan TimePicker.
   - Jika toggle diaktifkan, alarm diatur menggunakan AlarmManager.setRepeating, dan akan berbunyi secara terus menerus hingga toggle dimatikan.
   - Waktu alarm diatur untuk memastikan bahwa alarm diatur untuk hari berikutnya jika waktu yang ditentukan sudah lewat pada hari yang sama.

## 7. **Fibonacci**

- Variabel Kelas:
   - fibMinus1, fibMinus2, currentFib: Variabel yang menyimpan nilai deret Fibonacci.
   - showCount: Objek TextView untuk menampilkan nilai deret Fibonacci.
   - n: Variabel untuk menyimpan indeks deret Fibonacci.
   - limit: Batas nilai deret Fibonacci.
   - mLimitInput: Objek EditText untuk mengambil input batas nilai.

## 8. **Chat**

- Output Penjelasan:
   - launchSecondActivity: Memulai SecondActivity dan mengirimkan pesan yang diambil dari mMessageEditText sebagai ekstra ke intent.
   - onActivityResult: Dipanggil saat aktivitas kedua (SecondActivity) memberikan hasil balasan.
   - Jika hasilnya RESULT_OK, tampilkan balasan di mReplyTextView dan buat mReplyHeadTextView terlihat.

## 9. **Maps**

- Output Penjelasan:
- onCreate:
   - Menginisialisasi tata letak (layout) dari aktivitas.
   - Menetapkan nilai latitude dan longitude sebagai contoh.
   - Membuat objek Uri dari koordinat lokasi.
   - Memanggil metode showMap untuk menampilkan peta.

## 10. **Movie**

1. Tab Activity:

Menggunakan TabLayout dan ViewPager untuk mengorganisir konten film dalam tab.
Menggunakan adapter Halaman untuk mengelola konten dalam ViewPager.

2. Fragment:

Menggunakan fragment untuk menampilkan daftar film dalam kategori "Action", "Fantasy", dan "Romantic".
Menggunakan OnClickListener untuk memulai aktivitas Exoplayer1Activity ketika gambar film diklik.
