# Analisis Perbaikan

## Permasalahan 1

### Gejala
Container nginx tidak dapat dijalankan dan tidak bisa diakses melalui localhost:8080.

### Penyebab
Terdapat kesalahan penulisan pada file konfigurasi nginx (nginx.conf), yaitu adanya syntax markdown ```nginx yang tidak valid dalam konfigurasi nginx.

### Solusi
Menghapus seluruh syntax markdown ```nginx pada file nginx.conf sehingga file hanya berisi konfigurasi nginx yang valid.

---

## Permasalahan 2

### Gejala
Container database (MySQL) gagal dijalankan dan tidak melakukan inisialisasi tabel.

### Penyebab
File init.sql mengandung syntax markdown ```sql yang menyebabkan error syntax SQL saat proses inisialisasi database.

### Solusi
Menghapus syntax markdown ```sql pada file init.sql sehingga script SQL dapat dieksekusi dengan benar.

---

## Permasalahan 3

### Gejala
Load balancing tidak berjalan dan web server tidak dapat diakses melalui nginx.

### Penyebab
Nginx tidak dapat berjalan karena error konfigurasi sebelumnya, sehingga request tidak dapat diteruskan ke web server.

### Solusi
Memperbaiki konfigurasi nginx.conf dan memastikan upstream ke web1, web2, dan web3 sudah benar.

---

## Permasalahan 4

### Gejala
Data identitas praktikan masih berupa placeholder pada web server.

### Penyebab
Variabel nama dan NIM pada file index.php belum diperbarui.

### Solusi
Mengganti placeholder dengan nama dan NIM asli praktikan pada web1, web2, dan web3.
