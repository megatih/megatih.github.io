---
layout: post
title: Introducing My Prayer Times
subtitle: Prayer times, tahrim guidance, Qibla direction, and calculation transparency
cover-img: /assets/img/my-prayer-times/app-icon.png
thumbnail-img: /assets/img/my-prayer-times/app-icon.png
share-img: /assets/img/my-prayer-times/app-icon.png
tags: [swift, ios, swiftui, widgetkit, notifications, projects, prayer-times, qibla]
description: "Introducing My Prayer Times, a free privacy-focused iPhone and iPad app for Muslims with prayer times, tahrim guidance, Qibla direction, widgets, local notifications, and transparent calculation context."
comments: true
---

I am introducing **My Prayer Times**, a free iPhone and iPad app for Muslims
that shows local prayer times, tahrim guidance, and Qibla direction with clear
calculation context.

There are already many apps that can remind us of our daily prayers and help
us face the Qibla. I created this app because I was interested in the
calculations and falak methods behind prayer times, and because I wanted to
understand how those methods could be presented respectfully and clearly in a
modern app.

As a Muslim in Malaysia, I also have to pay attention to tahrim times. These
intervals are not always shown in prayer apps, and some users may not be fully
aware of them. My Prayer Times brings prayer times and tahrim guidance into
the same daily view, while being careful to say that tahrim information is
timing guidance and not an automated fatwa.

The app is provided free as my amal jariah for Muslim users. I would gladly
welcome suggestions, corrections, and thoughtful feedback to improve it,
inshaAllah.

![My Prayer Times app icon](/assets/img/my-prayer-times/app-icon.png){: .mx-auto.d-block style="max-width: 420px;" }

![The Today dashboard](/assets/img/my-prayer-times/today-dashboard.png){: .mx-auto.d-block style="max-width: 390px;" }

### What the app provides

* **A focused Today tab:** The main screen shows the detected place, local
  date, next prayer, countdown, current tahrim status, and complete daily
  schedule.
* **Prayer-time estimates:** The app calculates Imsak, Subuh, Syuruk, Dhuha,
  Zohor, Asar, Maghrib, and Isyak using the selected convention and current
  coordinates.
* **Tahrim guidance:** For supported Sunni-method presets, it displays
  intervals around Subuh, sunrise, solar noon, Asar, and sunset. For Jafari
  presets, it explains that the app's generic Sunni tahrim model is not
  applied.
* **Qibla direction:** A dedicated Qibla tab calculates the bearing to Makkah
  and combines it with the device compass, heading, accuracy, and north
  reference.
* **Calculation methods:** The app includes 13 authority and convention
  presets, with automatic selection for supported countries and a manual
  choice for users who prefer a specific method.
* **Notifications and widgets:** Optional local notifications are available for
  Subuh, Zohor, Asar, Maghrib, and Isyak. Home Screen widgets and Lock Screen
  accessories show the next prayer, upcoming times, and tahrim context where
  available.
* **Languages:** The app supports English, Bahasa Melayu, and System Default.
* **Privacy:** There are no accounts, advertisements, analytics, or cross-app
  tracking.

### Calculation with humility

The Settings screen includes JAKIM, Muslim World League, Umm al-Qura, Egyptian
Survey, Karachi, ISNA, Kemenag Indonesia, Diyanet, MUIS, Grande Mosquee de
Paris, UOIF / Musulmans de France, University of Tehran, and Leva Qum.

Each preset keeps its calculation parameters together, including twilight
angles, Asar shadow factor, Maghrib rule, fixed Isyak interval where used, and
documented adjustments where applicable. The app also shows whether a method is
a documented convention, an attributed preset, or a compatibility estimate.

This matters because prayer times are not merely numbers on a screen. Official
zone timetables, local terrain, high-latitude conditions, institutional
adjustments, and local religious guidance can produce differences. My Prayer
Times therefore presents coordinate-based estimates and makes the selected
method visible. When a local mosque, scholar, or official religious authority
has a timetable that applies to you, that guidance should take precedence.

My Prayer Times is not affiliated with or endorsed by any authority or
organisation named in the app.

### Privacy and support

Location is used while the app is in use to calculate prayer times and Qibla
direction. The app does not request background location access, does not store
a location history, and does not send prayer schedules, compass readings, or
notification data to the developer.

The widget uses one local snapshot saved by the main app, containing the latest
coordinates, place name, time zone, selected method, language, and save time.
It is used locally by the widget, overwritten when inputs change, and treated
as stale after seven days.

More details are available on the app page, privacy policy, and support page:

<div class="text-center">
  <a href="/my-prayer-times/" class="btn btn-primary btn-lg">Visit the App Page</a>
  <a href="/my-prayer-times/privacy/" class="btn btn-outline-primary btn-lg">Privacy Policy</a>
  <a href="/my-prayer-times/support/" class="btn btn-outline-primary btn-lg">Support</a>
</div>

---

## Bahasa Melayu

Saya ingin memperkenalkan **My Prayer Times**, aplikasi iPhone dan iPad
percuma untuk umat Islam yang memaparkan waktu solat setempat, panduan tahrim
dan arah kiblat bersama konteks pengiraan yang jelas.

Sudah banyak aplikasi yang boleh mengingatkan kita tentang solat harian dan
membantu kita menghadap kiblat. Saya membangunkan aplikasi ini kerana saya
berminat dengan pengiraan dan kaedah falak di sebalik waktu solat, serta ingin
memahami bagaimana kaedah tersebut boleh dipersembahkan dengan hormat dan
jelas dalam aplikasi moden.

Sebagai seorang Muslim di Malaysia, saya juga perlu mengambil perhatian
terhadap waktu tahrim. Selang ini tidak selalu dipaparkan dalam aplikasi waktu
solat, dan sebahagian pengguna mungkin belum begitu menyedarinya. My Prayer
Times menggabungkan waktu solat dan panduan tahrim dalam paparan harian yang
sama, sambil menjelaskan bahawa maklumat tahrim ialah panduan waktu dan bukan
fatwa automatik.

Aplikasi ini disediakan secara percuma sebagai amal jariah saya untuk pengguna
Muslim. Saya sangat mengalu-alukan cadangan, pembetulan dan maklum balas yang
baik untuk memperbaikinya, inshaAllah.

### Apa yang disediakan

* **Tab Hari Ini yang fokus:** Skrin utama menunjukkan tempat yang dikesan,
  tarikh setempat, solat seterusnya, kira detik, status tahrim semasa dan
  jadual harian lengkap.
* **Anggaran waktu solat:** Aplikasi mengira Imsak, Subuh, Syuruk, Dhuha,
  Zohor, Asar, Maghrib dan Isyak menggunakan konvensyen pilihan serta
  koordinat semasa.
* **Panduan tahrim:** Bagi pratetap kaedah Sunni yang disokong, aplikasi
  memaparkan selang sekitar Subuh, matahari terbit, tengah hari suria, Asar
  dan matahari terbenam. Bagi pratetap Jaafari, aplikasi menerangkan bahawa
  model tahrim Sunni umum tidak digunakan.
* **Arah kiblat:** Tab Kiblat khusus mengira bearing ke Makkah dan
  menggabungkannya dengan kompas peranti, arah semasa, ketepatan dan rujukan
  utara.
* **Kaedah pengiraan:** Aplikasi menyediakan 13 pratetap pihak berkuasa dan
  konvensyen, dengan pemilihan automatik untuk negara yang disokong serta
  pilihan manual untuk pengguna yang memilih kaedah tertentu.
* **Pemberitahuan dan widget:** Pemberitahuan setempat pilihan tersedia untuk
  Subuh, Zohor, Asar, Maghrib dan Isyak. Widget Skrin Utama dan aksesori Skrin
  Kunci memaparkan solat seterusnya, waktu akan datang dan konteks tahrim
  apabila tersedia.
* **Bahasa:** Aplikasi menyokong English, Bahasa Melayu dan Lalai Sistem.
* **Privasi:** Tiada akaun, iklan, analitik atau penjejakan merentas aplikasi.

### Pengiraan dengan rendah hati

Skrin Tetapan menyediakan JAKIM, Muslim World League, Umm al-Qura, Egyptian
Survey, Karachi, ISNA, Kemenag Indonesia, Diyanet, MUIS, Grande Mosquee de
Paris, UOIF / Musulmans de France, University of Tehran dan Leva Qum.

Setiap pratetap mengekalkan parameter pengiraannya bersama-sama, termasuk
sudut senja, faktor bayang Asar, peraturan Maghrib, sela tetap Isyak apabila
digunakan dan pelarasan yang didokumenkan jika berkenaan. Aplikasi juga
memaparkan sama ada sesuatu kaedah ialah konvensyen yang didokumenkan,
pratetap yang dinisbahkan atau anggaran keserasian.

Ini penting kerana waktu solat bukan sekadar nombor pada skrin. Jadual rasmi
zon, bentuk muka bumi setempat, keadaan latitud tinggi, pelarasan institusi
dan panduan agama tempatan boleh menghasilkan perbezaan. Oleh itu, My Prayer
Times memaparkan anggaran berasaskan koordinat dan menunjukkan kaedah yang
dipilih. Apabila masjid, ulama atau pihak berkuasa agama rasmi setempat
mempunyai jadual yang terpakai kepada anda, panduan tersebut hendaklah
diutamakan.

My Prayer Times tidak bergabung dengan atau diperakui oleh mana-mana pihak
berkuasa atau organisasi yang dinamakan dalam aplikasi.

### Privasi dan sokongan

Lokasi digunakan semasa aplikasi digunakan untuk mengira waktu solat dan arah
kiblat. Aplikasi tidak meminta akses lokasi latar belakang, tidak menyimpan
sejarah lokasi dan tidak menghantar jadual solat, bacaan kompas atau data
pemberitahuan kepada pembangun.

Widget menggunakan satu petikan setempat yang disimpan oleh aplikasi utama,
mengandungi koordinat terkini, nama tempat, zon waktu, kaedah pilihan, bahasa
dan masa simpanan. Petikan ini digunakan secara setempat oleh widget,
digantikan apabila input berubah dan dianggap lapuk selepas tujuh hari.

Maklumat lanjut tersedia di halaman aplikasi, dasar privasi dan halaman
sokongan:

<div class="text-center">
  <a href="/my-prayer-times/" class="btn btn-primary btn-lg">Halaman Aplikasi</a>
  <a href="/my-prayer-times/privacy/" class="btn btn-outline-primary btn-lg">Dasar Privasi</a>
  <a href="/my-prayer-times/support/" class="btn btn-outline-primary btn-lg">Sokongan</a>
</div>
