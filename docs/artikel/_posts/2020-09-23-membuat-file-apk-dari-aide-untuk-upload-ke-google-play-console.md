---
title: Membuat file APK dari aplikasi AIDE untuk publish ke Google Play Console
description: Berikut langkah yang benar untuk membuat file APK dari aplikasi AIDE agar dapat di-publish ke Google Play Console.
---
# Membuat file APK dari aplikasi AIDE untuk publish ke Google Play Console

AIDE adalah perangkat lunak (software) yang berjalan di Android. Perangkat lunak ini digunakan untuk membuat aplikasi Android dll secara langsung di Android itu sendiri. Alih-alih menggunakan Android Studio, kamu bisa menggunakan perangkat lunak ini untuk belajar membuat aplikasi sederhana.

Berikut ini cara membuat dan menandatangani file APK dari aplikasi AIDE agar dapat diunggah ke Google Play Console. Fungsi penandatanganan aplikasi untuk publish hanya dapat dilakukan dari AIDE Premium. Ingat, jangan pakai yang bajakan. Kalau kamu ingin aplikasi kamu dihargai oleh orang lain, hargai juga karya orang lain. Membajak sama dengan mencuri. Kalau kamu belum punya cukup uang untuk membeli, tunggulah sampai uangmu cukup. Kalau kamu sudah pakai versi premium, yuk lanjut.

* 
{:toc}

## 1. Buka Project

Buka proyek yang akan kamu publish. Pastikan proyek kamu tidak mengandung error. AIDE tidak dapat menandatangani proyek yang masih mengandung error.

## 2. Ubah Build Variants

Sebelum mem-publish aplikasi kamu, pastikan variannya adalah "RELEASE". Untuk mengubah Build Variant, ketuk "More... > Project > Build Variants > release", lalu ketuk OK.

## 3. Publish Project

Ketuk "More... > Project > Publish Project".

Untuk menandatangani APK, kamu harus punya "Keystore". Jika belum punya, ketuk "CREATE KEYSTORE", lalu isi data-data yang diperlukan, lalu ketuk "CREATE". Jika sudah punya keystore, kamu bisa langsung ketuk "EXPORT". Kamu bisa menggunakan keystore yang dibuat dari Android Studio. Masukkan password keystore alias yang barusan kamu buat atau yang sudah kamu punya, lalu ketuk OK.

## 4. Simpan APK dan Keystore

File APK dan keystore kamu disimpan di folder "/storage/emulated/0/AppProjects". File keystore wajib disimpan untuk menandatangani rilis update aplikasi kamu selanjutnya.

Sekarang file APK kamu siap untuk di-publish. Kamu juga bisa mengetes app kamu terlebih dahulu sebelum buru-buru publish. Gimana? mudah aja kan.
