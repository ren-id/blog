---
title: Panduan Membuat Blog di Github Pages dengan Custom Domain .my.id
description: Bikin blog di Github Pages itu sebenarnya susah-susah gampang. Kamu mesti banyak belajar.
categories: artikel
---
# Panduan Membuat Blog di Github Pages dengan Custom Domain .my.id

Mau bikin blog pribadi seperti yang sedang kamu lihat ini? Kasih tau _nggak_ ya. Ya udah deh aku kasih tau. Yuk lanjut baca sampai tuntas. Kalau nggak ngeh tanya di kolom komentar aja ya!

* 
{:toc}

## 1. Persiapan

Sebelum memulai, berikut ini adalah persiapan kamu.

- Panduan ini ditujukan buat kamu yang telah memiliki pengetahuan dasar tentang web, seperti HTML dan CSS.
- Selain itu, kamu juga harus memahami tentang server, host, DNS, dan istilah teknis lainnya.

## 2. Memulai

### 2.1. Membeli Domain .my.id

Panduan ini menyarankan untuk membeli domain di [register.domain.id/registrar](https://register.domain.id/registrar) karena dikelola langsung oleh lembaga yang ditunjuk resmi oleh pemerintah.

Berikut langkah-langkah membeli domain.

- Buat akun dengan klik/tap *Register New Account*.
- Pada navigasi sebelah kiri, klik/tap **Domain**, lalu klik/tap **Register**.
- Ketik **nama domain** yang kamu inginkan (misal: **ren.my.id**), lalu submit
- Pilih nama domain **.my.id** kamu.
- Bayar sesuai instruksi (disarankan membayar menggunakan akun virtual).
- Jangan lupa konfirmasi pembayaran kalau kamu membayar secara manual/transfer bank.

Pengelola Nama Domain Indonesia (PANDI) akan mengirimi email konfirmasi jika nama domain kamu sudah aktif.

### 2.2. Membuat Akun Cloudflare

Cloudflare adalah layanan yang dikenal sebagai CDN. Layanan ini menyediakan paket gratis yang memungkinkan pengguna untuk setting DNS. Gunanya untuk mengarahkan pengunjung—yang mengetik nama domain kamu—ke halaman web yang disimpan di Github.

Kunjungi [cloudflare.com](https://cloudflare.com) untuk registrasi.

### 2.3. Membuat Akun Github

Github terkenal dengan layanan berbagi kode sumber untuk proyek-proyek perangkat lunak sumber terbuka.

Github Pages adalah bagian layanan yang memungkinkan pengguna menyimpan kode sumber web di repositori.

Kunjungi [github.com](https://github.com) untuk registrasi.

## 3. Mengaktifkan

Tindakan berikut sebaiknya dilakukan sesuai urutan. Kamu dapat mengabaikannya kalau sudah memiliki pengetahuan tentang itu.

### 3.1. Mengubah Nameserver

Berikut ini langkah-langkah untuk mengubah nameserver.

- Kunjungi [register.domain.id/registrar](https://register.domain.id/registrar)
- Klik/tap **Domain** 》**List**
- Klik/tap ikon menu (3 garis horizontal) di sebelah kanan nama domain.
- Klik/tap **Update**
- Nameserver 1 diisi dengan **amir.ns.cloudflare.com**; Nameserver 2 diisi dengan **dana.ns.cloudflare.com**
- Klik/tap **Submit**

### 3.2. Mengaktifkan Github Pages

Berikut langkah-langkah mengaktifkan Github Pages setelah selesai membuat akun Github.

- Masuk (login) ke github.com
- Klik tombol **New** untuk membuat repositori, ikuti petunjuknya
- Masuk ke repositori yang baru dibuat
- Ketuk tab **Settings**
- Gulir ke bawah dan cari Github Pages
- Klik menu drop-down dan pilih **Branch: master**
- Klik menu drop-down di samping **Branch: master** dan pilih **/(root)**
- Klik tombol **Save**

### 3.3. Mengatur DNS

Ini adalah bagian yang penting. Berikut cara membuat rekaman DNS agar nama domain kamu dapat diarahkan ke Github Pages.

- Masuk (login) ke cloudflare.com
- Klik tombol **Add a Site** untuk menambahkan nama domain yang kamu beli, ikuti petunjuknya
- Klik nama domain yang baru ditambahkan
- Ketuk tab **DNS**
- Klik tombol **Add record** dan tambahkan 4 rekaman **Type A** dengan nilai bidang **IPv4 address** masing-masing diisi: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153. Bidang **Name** diisi **@**, dan klik ikon awan jingga. Klik tombol **Save**.

### 3.4. Menggunakan Custom Domain

- Masuk (login) ke github.com
- Masuk ke repositori
- Ketuk tab **Settings**
- Gulir ke bawah dan cari Github Pages
- Isi bidang **Custom domain** dengan nama domain kamu
- Klik tombol **Save**

### 3.5. Mencoba Akses

Untuk memastikan semua setelan dilakukan dengan benar, buka browser dan ketik nama domain kamu. Jika semuanya benar, seharusnya browser akan menampilkan halaman web standar yang berisi wiki repositori Github kamu.

### 3.6. Membuat Halaman Web

Coba buat file **index.html** dan taruh di repositori Github.

Berikut contoh file **index.html**.

```
<!doctype html>
<html>
<head>
<title>Halo dunia!</title>
</head>
<body>
<h1>Halo dunia!</h1>
<p>Ini adalah sebuah paragraf.</p>
</body>
</html>
```
## 4. Catatan

Membuat web blog di Github Pages mengharuskan kamu untuk membuat templat (layout) secara mandiri. Jadi, kamu harus mempelajari struktur berkas di direktori Github Pages kamu.

[Klik di sini](https://github.com/ren-id/me) untuk melihat contoh struktur berkas blog ini.
