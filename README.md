# Program-Searching-Aditya-Dinata
Nama : Aditya Dinata

NIM : 2209116062

Kelas : Sistem Informasi B 2022

Program Searching Aditya Dinata

Program ini adalah program untuk mencari indeks dari beberapa elemen yang terdapat dalam sebuah list menggunakan dua jenis algoritma pencarian, yaitu Jump Search dan Fibonacci Search. List yang digunakan dalam program ini adalah sebagai berikut: ["Arsel", "Avivah", "Daiva", ["Wahyu", "Wibi"]].

Program ini menggunakan dua metode searching yaitu Jump Search dan Fibonacci Search.

Pertama, program akan menampilkan daftar data yang akan dicari indeksnya yaitu Arsel, Avivah, Daiva, Wahyu, dan Wibi. Kemudian pengguna diminta untuk memilih metode searching yang akan digunakan. Jika pengguna memilih metode Jump Search, program akan melakukan pencarian indeks menggunakan fungsi jump_search yang ada dalam program. Fungsi ini menggunakan metode Jump Search yang bekerja dengan cara membagi data menjadi beberapa blok dan mencari data pada setiap blok. Jika pengguna memilih metode Fibonacci Search, program akan melakukan pencarian indeks menggunakan fungsi fibonacci_search yang ada dalam program. Fungsi ini menggunakan metode Fibonacci Search yang bekerja dengan cara menggunakan deret fibonacci untuk mencari indeks dari data yang dicari.

Setelah itu, program akan menampilkan hasil pencarian indeks dari setiap data yang dicari menggunakan metode yang telah dipilih. Jika data ditemukan, program akan menampilkan indeksnya. Selanjutnya, program akan menampilkan daftar data kembali dan meminta pengguna untuk menekan Enter untuk kembali ke menu utama. Jika pengguna memilih untuk keluar dari program, program akan berhenti.

Library yang Digunakan

os: digunakan untuk membersihkan console setiap kali program dijalankan.

time: digunakan untuk memberikan jeda atau delay antara satu output dengan output lainnya.

math: digunakan untuk melakukan operasi matematika, seperti menghitung akar kuadrat dengan fungsi sqrt().

Fungsi dan Algoritma yang Digunakan

Fungsi jump()

Fungsi ini digunakan untuk melakukan pencarian indeks dari elemen yang ada di dalam list menggunakan algoritma Jump Search.

Algoritma Jump Search

Inisialisasi variabel jump dengan nilai akar kuadrat panjang list.
Dapatkan indeks kanan dengan meminimumkan antara panjang list - 1 dan kiri + jump - 1.
Lakukan pencarian data dengan melompati jump indeks indeks dari kiri ke kanan hingga data yang dicari tidak lebih besar dari data pada indeks kanan atau sudah melebihi panjang list.
Jika data yang dicari berada di antara indeks kiri dan kanan, maka lakukan pencarian linear dari indeks kiri hingga indeks kanan untuk mendapatkan indeks dari data yang dicari.
Jika data yang dicari tidak ditemukan, kembalikan nilai -1.

Fungsi fib()

Fungsi ini digunakan untuk melakukan pencarian indeks dari elemen yang ada di dalam list menggunakan algoritma Fibonacci Search.

Algoritma Fibonacci Search

Inisialisasi variabel fib1 dengan nilai 1 dan fib2 dengan nilai 0.
Lakukan iterasi untuk mendapatkan nilai bilangan fibonacci terdekat yang lebih besar atau sama dengan panjang list.
Inisialisasi variabel offset dengan -1.
Lakukan pencarian data dengan membandingkan data pada indeks yang merupakan penjumlahan antara offset dan bilangan fibonacci terdekat yang lebih kecil dari atau sama dengan panjang list, dan perbandingan data pada indeks tersebut dengan data yang dicari.

Jika data yang dicari lebih kecil dari data pada indeks tersebut, maka lanjutkan pencarian dengan mengurangi nilai bilangan fibonacci terdekat sebelumnya, dan jika data yang dicari lebih besar dari data pada indeks tersebut, maka lanjutkan pencarian dengan mengurangi nilai bilangan fibonacci terdekat sebelumnya dan menambahkan nilai offset dengan bilangan fibonacci terdekat sebelumnya.

Jika data yang dicari ditemukan pada indeks yang valid, kembalikan nilai indeks tersebut.
Jika data yang dicari tidak ditemukan, kembalikan nilai -1.

Fungsi mulai()

Fungsi ini digunakan untuk menampilkan menu dan meminta input dari pengguna untuk memilih jenis algoritma pencarian yang akan digunakan. Program akan terus berjalan dan menampilkan menu hingga pengguna memilih untuk keluar dari program.
