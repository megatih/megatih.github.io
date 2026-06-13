---
layout: post
title: Introducing My Prayer Times
subtitle: Location-aware prayer calculation methods, tahrim guidance, and Qibla direction
cover-img: /assets/img/my-prayer-times/app-icon.png
thumbnail-img: /assets/img/my-prayer-times/app-icon.png
share-img: /assets/img/my-prayer-times/app-icon.png
tags: [swift, ios, swiftui, projects, prayer-times, qibla]
description: "Introducing My Prayer Times, a privacy-focused iPhone and iPad app with location-aware prayer calculation methods, tahrim guidance, and Qibla direction."
comments: true
---

I am pleased to introduce **My Prayer Times**, an iPhone and iPad app that
calculates local prayer times, tahrim intervals, and Qibla direction from your
current coordinates.

The project began with a practical question: how can an app provide transparent,
location-aware prayer-time estimates while making the assumptions and limits of
its calculations clear? My Prayer Times answers that question with an on-device
SwiftUI experience that keeps the selected calculation convention and its
limitations visible.

![My Prayer Times app icon](/assets/img/my-prayer-times/app-icon.png){: .mx-auto.d-block style="max-width: 420px;" }

### What My Prayer Times Provides

* **Coordinate-based prayer times:** The app calculates Imsak, Subuh, Syuruk,
  Dhuha, Zohor, Asar, Maghrib, and Isyak for the detected location and local
  time zone.
* **Location-aware calculation methods:** The app automatically selects a
  matching authority or convention for supported countries and falls back to
  Umm al-Qura University, Makkah elsewhere.
* **Manual method selection:** A Settings screen lets you choose from 13
  documented authority or convention presets. A manual choice is stored on the
  device and remains active across launches and location changes.
* **Tahrim guidance:** It presents relevant intervals around Subuh, sunrise,
  solar noon, Asar, and sunset, with explanations and links to official
  references. The app does not apply the generic Sunni interval model to the
  Jafari Tehran and Leva Qum presets.
* **Live Qibla compass:** Qibla direction is calculated geodesically and paired
  with the device compass, using true north when available and a magnetic-north
  fallback when necessary.
* **English and Bahasa Melayu:** The interface and explanatory content are
  available in both languages.
* **Privacy-focused operation:** There are no accounts, advertisements,
  analytics, or cross-app tracking.

### Calculation Methods

The Settings screen includes presets for JAKIM, Muslim World League, Umm
al-Qura, Egyptian Survey, Karachi, ISNA, Kemenag Indonesia, Diyanet, MUIS,
Grande Mosquee de Paris, UOIF / Musulmans de France, University of Tehran, and
Leva Qum.

Each preset keeps its Fajr and Isha rules, Asar shadow factor, sunrise and
Maghrib criteria, and documented minute adjustments together. The calculator
also supports Umm al-Qura's fixed 90-minute Isyak interval and the delayed
Maghrib criteria used by the Tehran and Leva Qum presets.

When Automatic by Location is enabled, the app selects a documented national
default for Malaysia, Saudi Arabia, Egypt, Pakistan, the United States, Canada,
Indonesia, Turkiye, Singapore, France, and Iran. Other countries use Umm
al-Qura as the fallback. The active authority or convention is displayed above
the prayer-time list.

These results are coordinate-based estimates, not replacements for official
zone or locality timetables. Some named methods are widely used software
conventions rather than complete official algorithms. Diyanet and Grande
Mosquee de Paris are explicitly labelled as compatibility estimates because
their published schedules include rules that a simple angle preset cannot
fully reproduce. Official timetables, local terrain, device sensors, and
high-latitude conditions can produce different results.

My Prayer Times is not affiliated with or endorsed by any authority or
organisation named in the app.

### Privacy and Support

Location is used to calculate prayer times and Qibla direction. The app does
not retain a location history or send prayer schedules and compass readings to
developer-operated servers.

The app stores only the selected automatic or manual calculation setting and
the selected authority identifier in iOS preferences. It does not store a
location history.

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
konvensyen pengiraan yang dipilih serta batasnya dengan jelas.

### Ciri Utama

* **Waktu solat berasaskan koordinat:** Aplikasi mengira Imsak, Subuh, Syuruk,
  Dhuha, Zohor, Asar, Maghrib dan Isyak untuk lokasi serta zon waktu yang
  dikesan.
* **Kaedah pengiraan berdasarkan lokasi:** Aplikasi memilih pihak berkuasa atau
  konvensyen yang sepadan secara automatik untuk negara yang disokong dan
  menggunakan Umm al-Qura University, Makkah sebagai pilihan sandaran.
* **Pemilihan kaedah manual:** Skrin Tetapan membolehkan anda memilih daripada
  13 pratetap pihak berkuasa atau konvensyen. Pilihan manual disimpan pada
  peranti dan kekal digunakan selepas aplikasi dibuka semula atau lokasi
  berubah.
* **Panduan tahrim:** Aplikasi memaparkan selang berkaitan Subuh, matahari
  terbit, tengah hari suria, Asar dan matahari terbenam, berserta penerangan
  serta pautan kepada rujukan rasmi. Model selang Sunni umum tidak digunakan
  untuk pratetap Jaafari Tehran dan Leva Qum.
* **Kompas kiblat langsung:** Arah kiblat dikira secara geodesik dan digabungkan
  dengan kompas peranti, menggunakan utara benar apabila tersedia serta utara
  magnet sebagai pilihan kedua.
* **Bahasa Inggeris dan Bahasa Melayu:** Antara muka dan kandungan penerangan
  tersedia dalam kedua-dua bahasa.
* **Mengutamakan privasi:** Tiada akaun, iklan, analitik atau penjejakan
  merentas aplikasi.

### Kaedah Pengiraan

Skrin Tetapan menyediakan pratetap JAKIM, Muslim World League, Umm al-Qura,
Egyptian Survey, Karachi, ISNA, Kemenag Indonesia, Diyanet, MUIS, Grande
Mosquee de Paris, UOIF / Musulmans de France, University of Tehran dan Leva
Qum.

Setiap pratetap mengekalkan peraturan Fajar dan Isyak, faktor bayang Asar,
kriteria Syuruk dan Maghrib serta pelarasan minit yang didokumenkan sebagai
satu set. Pengira turut menyokong sela tetap Isyak 90 minit bagi Umm al-Qura
dan kriteria Maghrib lewat bagi pratetap Tehran dan Leva Qum.

Apabila Automatik mengikut Lokasi diaktifkan, aplikasi memilih konvensyen
kebangsaan yang didokumenkan untuk Malaysia, Arab Saudi, Mesir, Pakistan,
Amerika Syarikat, Kanada, Indonesia, Turkiye, Singapura, Perancis dan Iran.
Negara lain menggunakan Umm al-Qura sebagai pilihan sandaran. Pihak berkuasa
atau konvensyen aktif dipaparkan di atas senarai waktu solat.

Keputusan ini ialah anggaran berasaskan koordinat dan bukan pengganti jadual zon
atau kawasan rasmi. Sesetengah kaedah yang dinamakan ialah konvensyen perisian
yang digunakan secara meluas dan bukannya algoritma rasmi yang lengkap.
Diyanet dan Grande Mosquee de Paris dilabel sebagai anggaran keserasian kerana
jadual terbitannya merangkumi peraturan yang tidak dapat dihasilkan sepenuhnya
oleh pratetap sudut ringkas. Jadual rasmi, bentuk muka bumi setempat, penderia
peranti dan keadaan latitud tinggi boleh menghasilkan keputusan yang berbeza.

My Prayer Times tidak bergabung dengan atau diperakui oleh mana-mana pihak
berkuasa atau organisasi yang dinamakan dalam aplikasi.

### Privasi dan Sokongan

Lokasi digunakan untuk mengira waktu solat dan arah kiblat. Aplikasi tidak
menyimpan sejarah lokasi atau menghantar jadual solat dan bacaan kompas kepada
pelayan yang dikendalikan oleh pembangun.

Aplikasi hanya menyimpan tetapan pengiraan automatik atau manual dan pengecam
pihak berkuasa yang dipilih dalam keutamaan iOS. Aplikasi tidak menyimpan
sejarah lokasi.

Maklumat lanjut tentang aplikasi, amalan privasi dan panduan penyelesaian
masalah tersedia melalui pautan di bawah.

<div class="text-center">
  <a href="/my-prayer-times/" class="btn btn-primary btn-lg">Halaman Aplikasi</a>
  <a href="/my-prayer-times/privacy/" class="btn btn-outline-primary btn-lg">Dasar Privasi</a>
  <a href="/my-prayer-times/support/" class="btn btn-outline-primary btn-lg">Sokongan</a>
</div>
