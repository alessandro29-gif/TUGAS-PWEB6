# TUGAS PWEB LATIHAN DROPDOWN JAVASCRIPT
5025251095_Alessandro Almaz Filemon

Link Website: https://registrasimatakuliah5025251095.netlify.app

Pendahuluan
Tugas ini bertujuan membangun sistem Registrasi Mata Kuliah interaktif yang menerapkan struktur HTML, penataan layout dan tampilan dengan CSS, serta manipulasi DOM dan logika interaktif menggunakan JavaScript. Terdapat bagian form registrasi untuk mengisi data mahasiswa serta pilihan mata kuliah menggunakan elemen dropdown <select>, di mana sistem melakukan validasi input dan menampilkan pesan danger berwarna merah jika terdapat kesalahan atau data yang belum lengkap. Terdapat pula bagian tabel atau daftar mata kuliah yang telah diregistrasikan/dipilih, lengkap dengan fitur pencarian, tombol edit dan hapus, dan pagination untuk mengatur jumlah tampilan data per halaman. 

Struktur
index.html sebagai struktur utama halaman
style.css sebagai pengatur keseluruhan layouting dan tampilan visual
app.js sebagai pengatur data, validasi form, penambahan, pengubahan, penghapusan, pencarian, serta fungsi dropdown dan pagination

# HTML
Terdapat elemen header yang memuat judul portal registrasi mata kuliah, navigasi utama, serta profil pengguna. Elemen main memuat judul halaman dan tata letak berbasis card/section, yaitu Form Registrasi Mata Kuliah untuk menginput data mahasiswa serta memilih mata kuliah melalui dropdown, serta section Daftar Registrasi untuk melihat data yang masuk lengkap dengan kolom pencarian, badge informasi total data, dan pagination. Elemen footer berisi informasi hak cipta dan keterangan portal akademik.

# Cuplikan Kode HTML
<img width="572" height="563" alt="image" src="https://github.com/user-attachments/assets/bafa8082-a52a-42c7-a218-58de01b9bace" />
<img width="748" height="404" alt="image" src="https://github.com/user-attachments/assets/b01bf07d-d193-4da2-ac95-0953a12d6ce4" />

# Java Script
Data registrasi disimpan dalam array objek di memori browser. Fungsi render() bertugas untuk menampilkan baris data pada tabel berdasarkan hasil pencarian dan halaman aktif, serta memperbarui badge jumlah data dan tombol pagination. Beberapa fungsi utama meliputi:
- Form Submit & Validasi: Memproses input form, memastikan pilihan dropdown terisi dengan benar dan data sesuai ketentuan.
- Edit dan Delete: Tombol Edit mengisi kembali form dengan data yang dipilih (termasuk pilihan dropdown) untuk diubah, sedangkan tombol Delete menghapus data dari daftar dengan konfirmasi.
- Search: Fitur pencarian real-time untuk memfilter data berdasarkan kata kunci yang mengetik pengguna.
- Dropdown & Pagination: Mengatur fungsionalitas pilihan dropdown mata kuliah dan membagi tampilan data per halaman (pagination).

# Cuplikan Kode JavaScript (Validasi Dropdown & Submit):
<img width="626" height="559" alt="image" src="https://github.com/user-attachments/assets/693572e3-1d68-44e4-879d-ef7a64b1dbc0" />
<img width="481" height="553" alt="image" src="https://github.com/user-attachments/assets/0edf5135-8c2f-43d6-bfeb-71ba23fa9129" />

# CSS
Bagian CSS pada file style.css dirancang untuk mengatur tampilan visual secara konsisten:
- Reset & CSS Variables: Menghilangkan margin/padding bawaan browser serta mendefinisikan variabel warna global (seperti --primary, --danger, --border, dan --radius) agar konsisten di seluruh komponen.
- Navbar: Menggunakan Flexbox (display: flex) dengan justify-content: space-between untuk mengatur tata letak navigasi atas agar rapi dan responsif.
- Layout Utama (CSS Grid): Menggunakan Grid dua kolom proporsional (kolom form di kiri dan tabel data di kanan) dengan max-width agar posisinya berada di tengah layar.
- Card & Form Component: Setiap section dibungkus dalam wadah bergaya card (dengan padding, border-radius, dan box-shadow). Elemen input dan dropdown dilengkapi pseudo-class :focus serta styling kelas error berwarna merah untuk validasi.
- Table & Actions: Mengatur perapian border tabel, tata letak tombol aksi (edit/delete), serta pagination menggunakan Flexbox agar selaras.

# Cuplikan Kode CSS:
<img width="563" height="575" alt="image" src="https://github.com/user-attachments/assets/339dad41-cee8-4c33-84a1-5b15dfe6d697" />
<img width="531" height="577" alt="image" src="https://github.com/user-attachments/assets/7fad995e-fd8d-49fe-8d80-eb792ee8b993" />

# Dokumentasi Tampilan
Laptop:
<img width="596" height="623" alt="image" src="https://github.com/user-attachments/assets/ec9cf20b-0b8f-4849-8362-23c96eda6e72" />

HP:
<img width="151" height="661" alt="image" src="https://github.com/user-attachments/assets/20240611-af4d-4953-a638-2014587dd640" />

# Kesimpulan
Aplikasi Registrasi Mata Kuliah dengan Dropdown dan JavaScript ini berhasil dibangun dengan fungsionalitas yang baik. HTML menyediakan struktur halaman, CSS mempercantik tampilan secara responsif, dan JavaScript menghadirkan interaktivitas penuh mulai dari validasi dropdown, manajemen data (tambah, ubah, hapus), pencarian, hingga pagination. Data saat ini disimpan hanya sementara di memori browser.
