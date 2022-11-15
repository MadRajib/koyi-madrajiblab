---
layout: post
title: Otomatisasi workflow Flutter dengan CI/CD menggunakan Github Actions 🚀 (dari Github ke PlayConsole)
slug: flutter-ci-cd
---

> Alternatif selain Github Actions adalah menggunakan Gitlab CI/CD. Namun, Codemagic juga menyediakan layanan CI/CD gratis untuk Flutter. Namun, saya lebih suka menggunakan Github Actions karena lebih mudah dan lebih fleksibel dan juga sudah bawaan github jadi tidak perlu ke website lain 🤣🤣.

## Intro

CI/CD digunakan untuk mempermudah developer dalam melakukan proses build, test, dan deploy aplikasi. Dengan CI/CD, developer tidak perlu melakukan build, test, dan deploy secara manual. CI/CD akan melakukan build, test, dan deploy secara otomatis. Dengan CI/CD, developer dapat fokus pada proses development aplikasi, sehingga developer dapat menghemat waktu dan meningkatkan produktivitas.

Dalam guide ini akan dibahas bagaimana cara melakukan CI/CD pada aplikasi Flutter menggunakan Github Actions. 

> Untuk unit test tidak dibahas ya disini hanya fokus ke build dan deploy saja 🤣

## Persiapan
- Punya akun Github dan mengerti dasar-dasarnya (Push, Pull, Fork, PR, dll)
- Project Flutter yang sudah jalan di lokal
- (Opsional) Akun Play Console untuk melakukan deploy secara otomatis ke Play Store

## Langkah (Build & Deploy)



### Buat file workflow

File workflow ini akan berisi konfigurasi untuk melakukan build dan deploy aplikasi Flutter. File workflow ini akan berada di folder `.github/workflows` dengan nama `flutter.yml`. 

- Buat file workflow dengan nama `flutter.yml` di folder `.github/workflows` ( kalau belum ada folder `.github/workflows` silahkan buat dulu )
![image](https://user-images.githubusercontent.com/45744788/202035956-5adda872-9c41-4559-91c0-6941625264eb.png)

- Isi file workflow dengan konfigurasi berikut
{% gist 2ab15baf96e59f73bcad781c993d232b %}

