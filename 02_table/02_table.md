# 2. Membuat Tabel di MySQL

Sebelum membuat tabel, perlu diketahui bahwa setiap
kolom di tabel memiliki berbagai macam tipe data. Di
antaranya yang paling umum adalah:

1. ```VARCHAR```: untuk tipe data teks
2. ```INT```: untuk tipe data bilangan
3. ```TEXT```: mirip seperti VARCHAR, hanya saja tidak memiliki batasan
4. ```DATETIME```: tipe data untuk menunjukkan waktu

Untuk tipe data VARCHAR, Anda harus memasukkan panjang
karakter yang dapat diterima oleh tabelnya, misalnya:

```VARCHAR(100)```

Untuk membuat tabel sederhana, Anda dapat
menjalankan perintah berikut:

```
CREATE TABLE nama_tabel
(
    nama_kolom1 TIPE_DATA,
    nama_kolom2 TIPE_DATA,
    dst...
);
```

Contohnya:

```
CREATE TABLE mahasiswa
(
    nim VARCHAR(12),
    nama_mhs VARCHAR(100),
    program_studi_mhs VARCHAR(100)
);
```

Jika Anda ingin menghapus tabel, Anda bisa
menjalankan perintah:

```DROP TABLE mahasiswa;```