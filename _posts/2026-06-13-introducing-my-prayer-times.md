---
layout: post
title: Introducing My Prayer Times
subtitle: Coordinate-based prayer times, tahrim guidance, and Qibla direction
cover-img: /assets/img/my-prayer-times/app-icon.png
thumbnail-img: /assets/img/my-prayer-times/app-icon.png
share-img: /assets/img/my-prayer-times/app-icon.png
tags: [swift, ios, swiftui, projects, prayer-times, qibla]
description: "Introducing My Prayer Times, a privacy-focused iPhone and iPad app for coordinate-based prayer times, tahrim guidance, and Qibla direction."
comments: true
---

I am pleased to introduce **My Prayer Times**, an iPhone and iPad app that
calculates local prayer times, tahrim intervals, and Qibla direction from your
current coordinates.

The project began with a practical question: how can an app provide transparent,
location-aware prayer-time estimates while making the assumptions and limits of
its calculations clear? My Prayer Times answers that question with an on-device
SwiftUI experience built around Malaysian calculation criteria.

![My Prayer Times app icon](/assets/img/my-prayer-times/app-icon.png){: .mx-auto.d-block style="max-width: 420px;" }

### What My Prayer Times Provides

* **Coordinate-based prayer times:** The app calculates Imsak, Subuh, Syuruk,
  Dhuha, Zohor, Asar, Maghrib, and Isyak for the detected location and local
  time zone.
* **Tahrim guidance:** It presents relevant intervals around Subuh, sunrise,
  solar noon, Asar, and sunset, with explanations and links to official
  references.
* **Live Qibla compass:** Qibla direction is calculated geodesically and paired
  with the device compass, using true north when available and a magnetic-north
  fallback when necessary.
* **English and Bahasa Melayu:** The interface and explanatory content are
  available in both languages.
* **Privacy-focused operation:** There are no accounts, advertisements,
  analytics, or cross-app tracking.

### Calculation Approach

Prayer times are calculated from solar positions using Malaysian criteria,
including the relevant twilight angles, the Shafii shadow factor for Asar, and
documented application safety adjustments.

These results are coordinate-based estimates, not replacements for official
zone timetables. The app identifies locations outside Malaysia as local
estimates rather than JAKIM-validated times. Official timetables, local terrain,
device sensors, and high-latitude conditions can produce different results.
My Prayer Times is not affiliated with or endorsed by JAKIM.

### Privacy and Support

Location is used to calculate prayer times and Qibla direction. The app does
not retain a location history or send prayer schedules and compass readings to
developer-operated servers.

You can read more about the app, its privacy practices, and troubleshooting
guidance at the links below.

<div class="text-center">
  <a href="/my-prayer-times/" class="btn btn-primary btn-lg">Visit the App Page</a>
  <a href="/my-prayer-times/privacy/" class="btn btn-outline-primary btn-lg">Privacy Policy</a>
  <a href="/my-prayer-times/support/" class="btn btn-outline-primary btn-lg">Support</a>
</div>

---

## Bahasa Melayu

Saya ingin memperkenalkan **My Prayer Times**, sebuah aplikasi iPhone dan iPad
yang mengira waktu solat setempat, selang tahrim dan arah kiblat berdasarkan
koordinat semasa anda.

Projek ini bermula dengan satu persoalan praktikal: bagaimanakah sebuah aplikasi
dapat menyediakan anggaran waktu solat berdasarkan lokasi secara telus sambil
menerangkan andaian dan batas pengiraannya? My Prayer Times menjawab persoalan
tersebut melalui pengalaman SwiftUI pada peranti yang menggunakan kriteria
pengiraan Malaysia.

### Ciri Utama

* **Waktu solat berasaskan koordinat:** Aplikasi mengira Imsak, Subuh, Syuruk,
  Dhuha, Zohor, Asar, Maghrib dan Isyak untuk lokasi serta zon waktu yang
  dikesan.
* **Panduan tahrim:** Aplikasi memaparkan selang berkaitan Subuh, matahari
  terbit, tengah hari suria, Asar dan matahari terbenam, berserta penerangan
  serta pautan kepada rujukan rasmi.
* **Kompas kiblat langsung:** Arah kiblat dikira secara geodesik dan digabungkan
  dengan kompas peranti, menggunakan utara benar apabila tersedia serta utara
  magnet sebagai pilihan kedua.
* **Bahasa Inggeris dan Bahasa Melayu:** Antara muka dan kandungan penerangan
  tersedia dalam kedua-dua bahasa.
* **Mengutamakan privasi:** Tiada akaun, iklan, analitik atau penjejakan
  merentas aplikasi.

### Pendekatan Pengiraan

Waktu solat dikira daripada kedudukan matahari menggunakan kriteria Malaysia,
termasuk sudut senja yang berkaitan, faktor bayang mazhab Syafii untuk Asar dan
pelarasan ihtiyat aplikasi yang didokumenkan.

Keputusan ini ialah anggaran berasaskan koordinat dan bukan pengganti jadual zon
rasmi. Aplikasi menandakan lokasi di luar Malaysia sebagai anggaran setempat,
bukan waktu yang disahkan oleh JAKIM. Jadual rasmi, bentuk muka bumi setempat,
penderia peranti dan keadaan latitud tinggi boleh menghasilkan keputusan yang
berbeza. My Prayer Times tidak bergabung dengan atau diperakui oleh JAKIM.

### Privasi dan Sokongan

Lokasi digunakan untuk mengira waktu solat dan arah kiblat. Aplikasi tidak
menyimpan sejarah lokasi atau menghantar jadual solat dan bacaan kompas kepada
pelayan yang dikendalikan oleh pembangun.

Maklumat lanjut tentang aplikasi, amalan privasi dan panduan penyelesaian
masalah tersedia melalui pautan di bawah.

<div class="text-center">
  <a href="/my-prayer-times/" class="btn btn-primary btn-lg">Halaman Aplikasi</a>
  <a href="/my-prayer-times/privacy/" class="btn btn-outline-primary btn-lg">Dasar Privasi</a>
  <a href="/my-prayer-times/support/" class="btn btn-outline-primary btn-lg">Sokongan</a>
</div>

