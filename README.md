# TUGAS PWEB LATIHAN DROPDOWN & KODE POS JAVASCRIPT

# TUGAS DROPDOWN

5025251095_Alessandro Almaz Filemon

Link Website: https://registrasimatakuliah5025251095.netlify.app

# Pendahuluan

Tugas ini bertujuan membangun sistem Registrasi Mata Kuliah interaktif yang menerapkan struktur HTML, penataan layout dan tampilan dengan CSS, serta manipulasi DOM dan logika interaktif menggunakan JavaScript. Terdapat bagian form registrasi untuk mengisi data mahasiswa serta pilihan mata kuliah menggunakan elemen dropdown `<select>`, di mana sistem melakukan validasi input dan menampilkan pesan danger berwarna merah jika terdapat kesalahan atau data yang belum lengkap. Terdapat pula bagian tabel atau daftar mata kuliah yang telah diregistrasikan/dipilih, lengkap dengan fitur pencarian, tombol edit dan hapus, dan pagination untuk mengatur jumlah tampilan data per halaman.

# Struktur

- `index.html` sebagai struktur utama halaman
- `style.css` sebagai pengatur keseluruhan layouting dan tampilan visual
- `app.js` sebagai pengatur data, validasi form, penambahan, pengubahan, penghapusan, pencarian, serta fungsi dropdown dan pagination

# HTML

Terdapat elemen header yang memuat judul portal registrasi mata kuliah, navigasi utama, serta profil pengguna. Elemen main memuat judul halaman dan tata letak berbasis card/section, yaitu Form Registrasi Mata Kuliah untuk menginput data mahasiswa serta memilih mata kuliah melalui dropdown, serta section Daftar Registrasi untuk melihat data yang masuk lengkap dengan kolom pencarian, badge informasi total data, dan pagination. Elemen footer berisi informasi hak cipta dan keterangan portal akademik.

# Cuplikan Kode HTML

<img width="572" height="563" alt="image" src="https://github.com/user-attachments/assets/bafa8082-a52a-42c7-a218-58de01b9bace" />

<img width="748" height="404" alt="image" src="https://github.com/user-attachments/assets/b01bf07d-d193-4da2-ac95-0953a12d6ce4" />

# Java Script

Data registrasi disimpan dalam array objek di memori browser. Fungsi `render()` bertugas untuk menampilkan baris data pada tabel berdasarkan hasil pencarian dan halaman aktif, serta memperbarui badge jumlah data dan tombol pagination. Beberapa fungsi utama meliputi:

- **Form Submit & Validasi:** Memproses input form, memastikan pilihan dropdown terisi dengan benar dan data sesuai ketentuan.
- **Edit dan Delete:** Tombol Edit mengisi kembali form dengan data yang dipilih (termasuk pilihan dropdown) untuk diubah, sedangkan tombol Delete menghapus data dari daftar dengan konfirmasi.
- **Search:** Fitur pencarian real-time untuk memfilter data berdasarkan kata kunci yang mengetik pengguna.
- **Dropdown & Pagination:** Mengatur fungsionalitas pilihan dropdown mata kuliah dan membagi tampilan data per halaman (pagination).

# Cuplikan Kode JavaScript (Validasi Dropdown & Submit)

<img width="626" height="559" alt="image" src="https://github.com/user-attachments/assets/693572e3-1d68-44e4-879d-ef7a64b1dbc0" />

<img width="481" height="553" alt="image" src="https://github.com/user-attachments/assets/0edf5135-8c2f-43d6-bfeb-71ba23fa9129" />

# CSS

Bagian CSS pada file `style.css` dirancang untuk mengatur tampilan visual secara konsisten:

- **Reset & CSS Variables:** Menghilangkan margin/padding bawaan browser serta mendefinisikan variabel warna global (seperti `--primary`, `--danger`, `--border`, dan `--radius`) agar konsisten di seluruh komponen.
- **Navbar:** Menggunakan Flexbox (`display: flex`) dengan `justify-content: space-between` untuk mengatur tata letak navigasi atas agar rapi dan responsif.
- **Layout Utama (CSS Grid):** Menggunakan Grid dua kolom proporsional (kolom form di kiri dan tabel data di kanan) dengan `max-width` agar posisinya berada di tengah layar.
- **Card & Form Component:** Setiap section dibungkus dalam wadah bergaya card (dengan `padding`, `border-radius`, dan `box-shadow`). Elemen input dan dropdown dilengkapi pseudo-class `:focus` serta styling kelas error berwarna merah untuk validasi.
- **Table & Actions:** Mengatur perapian border tabel, tata letak tombol aksi (edit/delete), serta pagination menggunakan Flexbox agar selaras.

# Cuplikan Kode CSS

<img width="563" height="575" alt="image" src="https://github.com/user-attachments/assets/339dad41-cee8-4c33-84a1-5b15dfe6d697" />

<img width="531" height="577" alt="image" src="https://github.com/user-attachments/assets/7fad995e-fd8d-49fe-8d80-eb792ee8b993" />

# Dokumentasi Tampilan

**Laptop:**

<img width="596" height="623" alt="image" src="https://github.com/user-attachments/assets/ec9cf20b-0b8f-4849-8362-23c96eda6e72" />

**HP:**

<img width="151" height="661" alt="image" src="https://github.com/user-attachments/assets/20240611-af4d-4953-a638-2014587dd640" />

# Kesimpulan

Aplikasi Registrasi Mata Kuliah dengan Dropdown dan JavaScript ini berhasil dibangun dengan fungsionalitas yang baik. HTML menyediakan struktur halaman, CSS mempercantik tampilan secara responsif, dan JavaScript menghadirkan interaktivitas penuh mulai dari validasi dropdown, manajemen data (tambah, ubah, hapus), pencarian, hingga pagination. Data saat ini disimpan hanya sementara di memori browser.

# TUGAS KODE POS

Link Website: https://kodepos5025251095.netlify.app

# Pendahuluan

Tugas ini bertujuan membangun sistem Pencarian Kode Pos Indonesia interaktif yang menerapkan struktur HTML, penataan layout dan tampilan dengan CSS, serta manipulasi DOM dan logika interaktif menggunakan JavaScript. Terdapat bagian form pencarian yang terdiri dari tiga elemen dropdown `<select>` bertingkat, yaitu Provinsi, Kabupaten/Kota, dan Kecamatan, di mana pilihan pada dropdown berikutnya akan menyesuaikan dengan pilihan dropdown sebelumnya. Sistem melakukan validasi input dan menampilkan pesan danger berwarna merah jika terdapat dropdown yang belum dipilih. Terdapat pula bagian hasil pencarian yang menampilkan kode pos dari kecamatan yang dipilih dalam bentuk card.

# Struktur

- `index.html` sebagai struktur utama halaman
- `css/style.css` sebagai pengatur keseluruhan layouting dan tampilan visual
- `js/app.js` sebagai pengatur data kode pos, validasi form, dropdown bertingkat, serta penampilan hasil pencarian

# HTML

Terdapat elemen header yang memuat nama portal Kode Pos Indonesia dan navigasi utama. Elemen hero memuat judul halaman beserta keterangan singkat cara penggunaan. Elemen main memuat tata letak berbasis card/section, yaitu Form Cari Kode Pos untuk memilih Provinsi, Kabupaten/Kota, dan Kecamatan melalui dropdown, serta section Hasil Pencarian untuk menampilkan kode pos yang ditemukan lengkap dengan teks informasi status pencarian. Dropdown Kabupaten/Kota dan Kecamatan awalnya berstatus `disabled` sampai dropdown sebelumnya dipilih. Elemen footer berisi keterangan hak cipta portal pencarian kode pos.

# Cuplikan Kode HTML

<img width="683" height="644" alt="image" src="https://github.com/user-attachments/assets/84f91f9e-6820-4f5f-b484-3e7964674a65" />

# Java Script

Data kode pos disimpan dalam objek bersarang (nested object) di dalam file `app.js` dengan struktur Provinsi → Kabupaten/Kota → Kecamatan → Kode Pos. Data ini dibaca melalui `Object.keys()` untuk mengisi pilihan pada setiap dropdown. Beberapa fungsi utama meliputi:

- **Dropdown Bertingkat:** Event `change` pada dropdown Provinsi mengisi pilihan Kabupaten/Kota, lalu event `change` pada Kabupaten/Kota mengisi pilihan Kecamatan. Fungsi `isiOpsi()` dipakai untuk membangun elemen `<option>` secara dinamis, sedangkan `resetKota()` dan `resetKecamatan()` mengembalikan dropdown ke kondisi awal dan menonaktifkannya kembali.
- **Validasi:** Fungsi `validate()` memastikan ketiga dropdown sudah dipilih. Jika belum, fungsi `setError()` menampilkan pesan berwarna merah dan menambahkan kelas `invalid` pada form group terkait.
- **Tampilkan Hasil:** Fungsi `tampilkanHasil()` mengambil kode pos dari data berdasarkan pilihan pengguna, lalu menampilkannya dalam card hasil. Jika data tidak ditemukan, akan muncul pesan bahwa hasil pencarian tidak ditemukan.
- **Keamanan Output:** Fungsi `esc()` meng-escape teks sebelum disisipkan ke HTML agar tidak terbaca sebagai tag.
- **Kosongkan Form:** Tombol Kosongkan Form mereset form, mengembalikan dropdown ke kondisi awal, menghapus pesan error, serta mengosongkan hasil pencarian.

# Cuplikan Kode JavaScript (Dropdown Bertingkat & Validasi)

<img width="746" height="667" alt="image" src="https://github.com/user-attachments/assets/08d6d064-f9a3-461b-a015-4eccf7915d0e" />


# CSS

Bagian CSS pada file `style.css` dirancang untuk mengatur tampilan visual secara konsisten:

- **Reset & CSS Variables:** Menghilangkan margin/padding bawaan browser serta mendefinisikan variabel warna global (seperti `--azure`, `--french`, `--danger`, `--border`, dan `--radius`) agar konsisten di seluruh komponen.
- **Navbar:** Menggunakan Flexbox (`display: flex`) dengan `justify-content: space-between` untuk mengatur tata letak navigasi atas agar rapi dan responsif.
- **Hero Section:** Menggunakan latar `linear-gradient` bernuansa biru dengan konten dibatasi `max-width` agar berada di tengah layar.
- **Layout Utama (CSS Grid):** Menggunakan `display: grid` untuk menyusun card form dan card hasil secara vertikal dengan jarak `gap` yang konsisten, serta Grid tiga kolom (`1fr 1fr 1fr`) untuk menata ketiga dropdown sejajar.
- **Card & Form Component:** Setiap section dibungkus dalam wadah bergaya card (dengan `padding`, `border-radius`, dan `box-shadow`). Elemen dropdown dilengkapi pseudo-class `:focus` dan `:disabled`, serta styling kelas `invalid` berwarna merah untuk validasi.
- **Result Card:** Hasil pencarian ditampilkan dengan Grid `repeat(auto-fill, minmax(260px, 1fr))` sehingga card menyesuaikan lebar layar.
- **Responsive:** Menggunakan `@media (max-width: 760px)` untuk mengubah tiga kolom dropdown menjadi satu kolom pada layar kecil, serta `@media (max-width: 650px)` untuk menyesuaikan padding navbar dan card.

# Cuplikan Kode CSS

<img width="518" height="615" alt="image" src="https://github.com/user-attachments/assets/99c9124c-18a4-442d-a76e-34a2f7e87fb6" />


# Dokumentasi Tampilan

**Laptop:**

<img width="1279" height="692" alt="image" src="https://github.com/user-attachments/assets/70dba6c6-edee-4232-bea9-5e22cbe89c1c" />
<img width="1278" height="701" alt="image" src="https://github.com/user-attachments/assets/245b6889-2cc4-4533-a951-b7c1436c7379" />

**HP:**

<img width="720" height="1600" alt="image" src="https://github.com/user-attachments/assets/d7017dac-9066-49ee-9351-055f0b696574" />
<img width="720" height="1600" alt="image" src="https://github.com/user-attachments/assets/325db11e-b197-44f1-a16d-206c331ff94d" />


# Kesimpulan

Aplikasi Pencarian Kode Pos dengan Dropdown dan JavaScript ini berhasil dibangun dengan fungsionalitas yang baik. HTML menyediakan struktur halaman, CSS mempercantik tampilan secara responsif, dan JavaScript menghadirkan interaktivitas mulai dari dropdown bertingkat (Provinsi, Kabupaten/Kota, Kecamatan), validasi input, hingga penampilan hasil kode pos. Data saat ini disimpan statis di dalam file JavaScript dan belum terhubung ke database.
