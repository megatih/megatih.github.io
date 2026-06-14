---
layout: post
title: Introducing My Prayer Times
subtitle: A redesigned daily prayer experience for the app, Home Screen, and Lock Screen
cover-img: /assets/img/my-prayer-times/app-icon.png
thumbnail-img: /assets/img/my-prayer-times/app-icon.png
share-img: /assets/img/my-prayer-times/app-icon.png
tags: [swift, ios, swiftui, widgetkit, notifications, projects, prayer-times, qibla]
description: "Introducing My Prayer Times, a privacy-focused iPhone and iPad app with prayer notifications, Home Screen and Lock Screen widgets, location-aware calculations, tahrim guidance, and live Qibla direction."
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

> **Updated June 15, 2026:** The app now has a redesigned Today dashboard, a
> dedicated Qibla tab, searchable settings, day-phase styling, and small,
> medium, and large Home Screen widgets alongside Lock Screen accessories.

![The redesigned Today dashboard](/assets/img/my-prayer-times/today-dashboard.png){: .mx-auto.d-block style="max-width: 390px;" }

### What My Prayer Times Provides

* **Focused Today dashboard:** The opening tab combines local date and
  location, a prominent next-prayer countdown, current tahrim status, and the
  complete schedule. Day-phase colour and highlighting make the current
  context clear without competing with the times.
* **Coordinate-based prayer times:** The app calculates Imsak, Subuh, Syuruk,
  Dhuha, Zohor, Asar, Maghrib, and Isyak for the detected location and local
  time zone.
* **Location-aware calculation methods:** The app automatically selects a
  matching authority or convention for supported countries and falls back to
  Umm al-Qura University, Makkah elsewhere.
* **Searchable settings:** The Settings screen lets you search and choose from
  13 documented authority or convention presets. A manual choice is stored on
  the device and remains active across launches and location changes.
* **Tahrim guidance:** It presents relevant intervals around Subuh, sunrise,
  solar noon, Asar, and sunset, with explanations and links to official
  references. The app does not apply the generic Sunni interval model to the
  Jafari Tehran and Leva Qum presets.
* **Dedicated Qibla tab:** Qibla direction is calculated geodesically and
  paired with the device compass, with bearing, heading, accuracy, and north
  reference presented together. Sensor updates run only while the tab is
  active.
* **English and Bahasa Melayu:** The interface and explanatory content are
  available in both languages. You can follow the system language or select a
  language in the app.
* **Configurable prayer notifications:** You can enable local notifications
  for Subuh, Zohor, Asar, Maghrib, and Isyak individually. The app schedules
  up to 60 upcoming alerts on the device and refreshes the rolling schedule
  when the app is opened or its calculation inputs change.
* **Widgets designed for every size:** The small Home Screen widget focuses on
  the next prayer, medium adds upcoming times, and large presents the full
  schedule with tahrim context. Rectangular, inline, and circular Lock Screen
  accessories remain available.
* **Reliable foreground refresh:** Returning from the Home Screen or another
  app keeps the last valid prayer schedule and Qibla direction visible. The
  app refreshes a location only when the previous fix is more than five
  minutes old, retries temporary failures, and uses bounded timeouts so the
  interface does not remain stuck waiting for a callback.
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

The app stores calculation, language, and notification preferences on the
device. To support the widget, it also stores one current snapshot containing
the latest coordinates, place name, time zone, selected method, language, and
save time in an Apple App Group shared only by the app and its widget
extension. This snapshot is overwritten when inputs change, is treated as
stale after seven days, and is never uploaded to the developer.

Notifications are local notifications managed by iOS. The app does not use a
remote notification server, request background location access, or perform
cross-app tracking. Because iOS limits pending requests, reopening the app
periodically renews the rolling notification schedule.

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

> **Dikemas kini pada 15 Jun 2026:** Aplikasi kini mempunyai papan pemuka Hari
> Ini yang direka semula, tab Kiblat khusus, Tetapan yang boleh dicari, gaya
> fasa hari serta widget Skrin Utama kecil, sederhana dan besar di samping
> aksesori Skrin Kunci.

### Ciri Utama

* **Papan pemuka Hari Ini:** Tab pembukaan menggabungkan tarikh dan lokasi,
  kira detik solat seterusnya yang jelas, status tahrim semasa dan jadual
  lengkap. Warna fasa hari dan sorotan menunjukkan konteks semasa dengan jelas.
* **Waktu solat berasaskan koordinat:** Aplikasi mengira Imsak, Subuh, Syuruk,
  Dhuha, Zohor, Asar, Maghrib dan Isyak untuk lokasi serta zon waktu yang
  dikesan.
* **Kaedah pengiraan berdasarkan lokasi:** Aplikasi memilih pihak berkuasa atau
  konvensyen yang sepadan secara automatik untuk negara yang disokong dan
  menggunakan Umm al-Qura University, Makkah sebagai pilihan sandaran.
* **Tetapan yang boleh dicari:** Skrin Tetapan membolehkan anda mencari dan
  memilih daripada 13 pratetap pihak berkuasa atau konvensyen. Pilihan manual
  disimpan pada peranti dan kekal digunakan selepas aplikasi dibuka semula atau
  lokasi berubah.
* **Panduan tahrim:** Aplikasi memaparkan selang berkaitan Subuh, matahari
  terbit, tengah hari suria, Asar dan matahari terbenam, berserta penerangan
  serta pautan kepada rujukan rasmi. Model selang Sunni umum tidak digunakan
  untuk pratetap Jaafari Tehran dan Leva Qum.
* **Tab Kiblat khusus:** Arah kiblat dikira secara geodesik dan digabungkan
  dengan kompas peranti. Bearing, arah, ketepatan dan rujukan utara dipaparkan
  bersama, dan penderia hanya dikemas kini ketika tab digunakan.
* **Bahasa Inggeris dan Bahasa Melayu:** Antara muka dan kandungan penerangan
  tersedia dalam kedua-dua bahasa. Anda boleh mengikut bahasa sistem atau
  memilih bahasa dalam aplikasi.
* **Pemberitahuan waktu solat:** Anda boleh mengaktifkan pemberitahuan setempat
  bagi Subuh, Zohor, Asar, Maghrib dan Isyak secara berasingan. Aplikasi
  menjadualkan sehingga 60 makluman akan datang pada peranti dan memperbaharui
  jadual berterusan apabila aplikasi dibuka atau input pengiraan berubah.
* **Widget untuk setiap saiz:** Widget kecil memfokuskan solat seterusnya,
  widget sederhana menambah waktu akan datang, dan widget besar memaparkan
  jadual lengkap bersama konteks tahrim. Aksesori Skrin Kunci segi empat tepat,
  sebaris dan bulat turut tersedia.
* **Penyegaran latar hadapan yang kukuh:** Apabila kembali daripada Skrin Utama
  atau aplikasi lain, jadual solat dan arah kiblat sah yang terakhir kekal
  dipaparkan. Aplikasi hanya menyegarkan lokasi apabila penentuan sebelumnya
  melebihi lima minit, mencuba semula kegagalan sementara dan menggunakan had
  masa supaya antara muka tidak terus menunggu panggil balik.
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

Aplikasi menyimpan pilihan pengiraan, bahasa dan pemberitahuan pada peranti.
Untuk menyokong widget, aplikasi turut menyimpan satu petikan semasa yang
mengandungi koordinat terkini, nama tempat, zon waktu, kaedah pilihan, bahasa
dan masa simpanan dalam App Group Apple yang hanya dikongsi oleh aplikasi dan
sambungan widgetnya. Petikan ini digantikan apabila input berubah, dianggap
lapuk selepas tujuh hari dan tidak pernah dimuat naik kepada pembangun.

Pemberitahuan ialah pemberitahuan setempat yang diuruskan oleh iOS. Aplikasi
tidak menggunakan pelayan pemberitahuan jauh, tidak meminta akses lokasi latar
belakang dan tidak melakukan penjejakan merentas aplikasi. Oleh sebab iOS
mengehadkan permintaan yang belum dihantar, buka semula aplikasi secara
berkala untuk memperbaharui jadual pemberitahuan berterusan.

Maklumat lanjut tentang aplikasi, amalan privasi dan panduan penyelesaian
masalah tersedia melalui pautan di bawah.

<div class="text-center">
  <a href="/my-prayer-times/" class="btn btn-primary btn-lg">Halaman Aplikasi</a>
  <a href="/my-prayer-times/privacy/" class="btn btn-outline-primary btn-lg">Dasar Privasi</a>
  <a href="/my-prayer-times/support/" class="btn btn-outline-primary btn-lg">Sokongan</a>
</div>
