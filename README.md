Jimly Asidiq Anwar - 4522210018

# Mini Habit Tracker

Mini Habit Tracker adalah aplikasi Flutter sederhana yang digunakan untuk melacak kebiasaan harian. Aplikasi ini sekaligus menjadi sarana belajar konsep *ephemeral state*, pengelolaan data dinamis, dan interaksi antarmuka pengguna menggunakan komponen-komponen Flutter seperti `StatefulWidget`, `setState()`, `AlertDialog`, dan lainnya.

## Fitur Utama

- Tambah, edit, dan hapus kebiasaan (habit)
- Tandai kebiasaan yang telah dilakukan
- Tampilan teks dicoret jika habit selesai
- Progress bar berdasarkan jumlah habit yang diselesaikan
- Reset semua status habit ke belum selesai
- Tidak menyimpan data secara permanen (*ephemeral*)

## Uji Aplikasi

### 1.	Jalankan aplikasi (flutter run).
![image](https://github.com/user-attachments/assets/c9dcd0f0-bdb4-41bd-a932-9ea82edd7198)

### 2.	Uji Strikethrough: Centang dan batalkan centang habit. Perhatikan teksnya.
![image](https://github.com/user-attachments/assets/9c04849a-c3c4-4d0b-a598-1cb6df776d3b)

### 3.	Uji Tambah Habit:
a. Klik tombol + di AppBar.
![image](https://github.com/user-attachments/assets/5afeda14-451a-48ec-af7f-afe022fa3ae1)
b. Coba simpan tanpa mengisi nama (validasi harus mencegah).
![image](https://github.com/user-attachments/assets/ed1393e9-b547-4f0a-8578-8348e3e1589c)
c.	Isi form dan simpan. Verifikasi habit baru muncul di list.
![image](https://github.com/user-attachments/assets/6b00b412-679b-434c-8a58-9f5438a53452)

### 4.	Uji Edit Habit:
a.	Klik menu tiga titik pada habit, pilih "Edit".
![image](https://github.com/user-attachments/assets/b8add1ce-ed3d-4d8b-b6dc-9153b4af1e9a)
b.	Dialog harus muncul dengan data habit tersebut.
![image](https://github.com/user-attachments/assets/362d0b1b-65dd-4a41-87c7-a80fb3a52929)
c.	Ubah nama/deskripsi dan simpan. Verifikasi perubahan di list.
![image](https://github.com/user-attachments/assets/0fe1954e-8aec-41ae-8ead-15987e206ae0)

### 5.	Uji Hapus Habit:
a.	Klik menu tiga titik pada habit, pilih "Hapus".
![image](https://github.com/user-attachments/assets/c6b84375-c7d0-4ba7-964e-02e54818e8b4)
b.	Dialog konfirmasi harus muncul. Coba batalkan.
![image](https://github.com/user-attachments/assets/01571d2d-f6af-4e58-a8e2-796818316395)
c.	Coba hapus lagi dan konfirmasi. Verifikasi habit hilang dari list.
![image](https://github.com/user-attachments/assets/9c12ba8d-5046-48fe-a8bd-f6b14e98e391)

### 6.	Uji Progress Bar: Pastikan progress di AppBar terupdate setelah menambah, menghapus, atau mencentang habit.
![image](https://github.com/user-attachments/assets/7dda47af-3351-4afd-9f54-90388562f4d3)

### 7.	Uji Reset: Tombol reset harus mengembalikan semua isDone ke false.
![image](https://github.com/user-attachments/assets/fef6d7d8-40a8-47b4-b682-01c3f3a91593)

### 8.	Uji Ephemeral State: Tutup paksa aplikasi dan buka kembali. Semua perubahan (tambah, edit, hapus) seharusnya hilang, dan hanya data dari habits.json yang tampil.
- Sebelum di tutup paksa :
![image](https://github.com/user-attachments/assets/6c6d7e80-d2a3-4951-8559-67d99bd6ba3e)
- Sesudah di tutup paksa :
![image](https://github.com/user-attachments/assets/0fdbdacb-d7ef-434a-ba2c-a6d1b3bb0343)

### 9.	Amati Output print: Perhatikan konsol debug. Kapan saja print('build ${habit.name}') muncul? Bagaimana ini berkaitan dengan aksi Anda (check, add, edit, delete)?
![image](https://github.com/user-attachments/assets/65d08c8f-f4de-4522-8690-b8753805292d)

## Cara Menjalankan Project

### 1. Clone Repository

```bash
git clone https://github.com/adiwp/flutter_projects.git
```

### 2. Masuk ke Direktori Proyek

```bash
cd flutter_projects/mini_habit_tracker
```

### 3. Dapatkan Dependency

```bash
flutter pub get
```

### 4. Jalankan Aplikasi

```bash
flutter run
```
