---
layout: page
title: My Prayer Times
subtitle: A focused daily prayer dashboard, complete widgets, notifications, and Qibla direction
permalink: /my-prayer-times/
---

My Prayer Times is an iPhone and iPad app that calculates local prayer times,
tahrim intervals, and Qibla direction from your current coordinates.

The app automatically selects a documented prayer-time authority or convention
for supported countries, with Umm al-Qura University, Makkah as the fallback.
You can override the automatic choice in Settings, and the manual selection
remains active across launches and location changes.

- No account, advertising, analytics, or tracking
- A redesigned Today dashboard with day-phase colour, next-prayer focus, and the complete schedule
- Location-based calculations for local prayer times
- 13 selectable authority and convention presets
- Automatic matching for supported countries with an Umm al-Qura fallback
- Searchable method selection, persistent manual choices, and transparent calculation parameters
- A dedicated Qibla tab with bearing, heading, accuracy, and north-reference status
- System, English, and Bahasa Melayu language choices
- Configurable local notifications for the five obligatory prayers
- Small, medium, and large Home Screen widgets plus Lock Screen accessories
- Resilient foreground location refresh without background location access
- Designed for iOS 17 and later

![The redesigned Today dashboard in My Prayer Times](/assets/img/my-prayer-times/today-dashboard.png){: .mx-auto.d-block style="max-width: 390px;" }

## Today and Qibla

The **Today** tab puts the information needed throughout the day first: the
current location and date, the next prayer and live countdown, the active
tahrim status, and a complete prayer schedule with the current or upcoming
event highlighted. Its background and accents adapt to the current part of the
day while preserving system contrast, Dynamic Type, and familiar SwiftUI
navigation.

Tahrim guidance is available in a compact, expandable section. Calculation
method, language, and notification controls remain available from Settings,
with a searchable method picker for the 13 included presets.

The **Qibla** tab gives the compass its own focused space. It shows the Qibla
bearing, current device heading, compass accuracy, and whether true or magnetic
north is being used. Compass updates are active only while this tab is in use.

## Notifications

Notifications are optional and are requested only after you turn them on in
Settings. Subuh, Zohor, Asar, Maghrib, and Isyak can each be enabled or
disabled independently.

The app schedules up to 60 local notification requests using the current
location, time zone, calculation method, and selected language. Delivery is
managed by iOS and may not occur at the exact calculated second. Reopen the
app periodically to renew the rolling schedule, and reopen it after travelling
or changing a calculation setting.

No remote notification service or developer-operated notification server is
used.

## Home Screen and Lock Screen widgets

The widgets use the same day-phase styling and information hierarchy as the
app while making purposeful use of each size:

- **Small:** the next prayer and live countdown at a glance.
- **Medium:** the next prayer plus the upcoming prayer sequence.
- **Large:** the complete daily schedule, next-prayer emphasis, and current
  tahrim guidance.
- **Lock Screen:** rectangular, inline, and circular next-prayer accessories.

Open the main app once to provide the widget with a current location and
calculation setting. The app stores one widget snapshot in its private App
Group. The widget stops using a snapshot after seven days and asks you to open
the app to refresh it. After travelling, open the app so the widget can use
the new location and time zone. Tapping a Home Screen widget opens the Today
tab.

## Foreground location behavior

The app requests location only while it is in use. When you return from the
Home Screen or another app, it keeps the last valid schedule and Qibla
direction visible. A new location is requested only when the previous fix is
more than five minutes old.

Temporary Core Location failures are retried, and location and geocoding
requests have bounded timeouts. If a refresh cannot complete, the previous
valid result remains available rather than being replaced by an indefinite
loading state.

## Available calculation methods

The app includes JAKIM, Muslim World League, Umm al-Qura, Egyptian Survey,
Karachi, ISNA, Kemenag Indonesia, Diyanet, MUIS, Grande Mosquee de Paris,
UOIF / Musulmans de France, University of Tehran, and Leva Qum.

The active method is displayed in the Prayer Times section. Each preset
controls its applicable twilight angles, Asar shadow factor, Maghrib rule,
fixed Isyak interval, and documented adjustments. Diyanet and Grande Mosquee
de Paris are labelled as compatibility estimates, and Jafari presets do not
display the app's generic Sunni tahrim intervals.

All displayed times remain coordinate-based estimates. Current official zone,
locality, mosque, or religious-authority timetables take precedence when a
difference matters.

[Privacy Policy](/my-prayer-times/privacy/) ·
[Support](/my-prayer-times/support/)

## Bahasa Melayu

My Prayer Times ialah aplikasi iPhone dan iPad yang mengira waktu solat
setempat, selang tahrim dan arah kiblat berdasarkan koordinat semasa anda.

Aplikasi memilih pihak berkuasa atau konvensyen waktu solat yang didokumenkan
secara automatik untuk negara yang disokong, dengan Umm al-Qura University,
Makkah sebagai pilihan sandaran. Anda boleh menukar pilihan automatik dalam
Tetapan, dan pilihan manual kekal digunakan selepas aplikasi dibuka semula
atau lokasi berubah.

- Tiada akaun, iklan, analitik atau penjejakan
- Papan pemuka Hari Ini dengan warna fasa hari, fokus solat seterusnya dan jadual lengkap
- Pengiraan berdasarkan lokasi untuk waktu solat setempat
- 13 pratetap pihak berkuasa dan konvensyen
- Padanan automatik bagi negara yang disokong dengan sandaran Umm al-Qura
- Pemilihan kaedah yang boleh dicari, pilihan manual yang kekal serta parameter pengiraan yang telus
- Tab Kiblat khusus dengan bearing, arah peranti, ketepatan dan status rujukan utara
- Pilihan bahasa Sistem, Bahasa Inggeris dan Bahasa Melayu
- Pemberitahuan setempat yang boleh dikonfigurasi bagi lima waktu solat fardu
- Widget Skrin Utama kecil, sederhana dan besar serta aksesori Skrin Kunci
- Penyegaran lokasi latar hadapan yang kukuh tanpa akses lokasi latar belakang
- Direka untuk iOS 17 dan lebih baharu

![Papan pemuka Hari Ini yang direka semula](/assets/img/my-prayer-times/today-dashboard.png){: .mx-auto.d-block style="max-width: 390px;" }

## Hari Ini dan Kiblat

Tab **Hari Ini** mengutamakan maklumat yang diperlukan sepanjang hari: lokasi
dan tarikh semasa, solat seterusnya dengan kira detik langsung, status tahrim
aktif serta jadual solat lengkap dengan waktu semasa atau akan datang
diserlahkan. Latar dan warna aksen berubah mengikut fasa hari sambil
mengekalkan kontras sistem, Dynamic Type dan navigasi SwiftUI yang lazim.

Panduan tahrim tersedia dalam bahagian padat yang boleh dikembangkan. Tetapan
kaedah pengiraan, bahasa dan pemberitahuan kekal mudah dicapai, termasuk
pemilih kaedah yang boleh dicari bagi 13 pratetap.

Tab **Kiblat** menyediakan ruang khusus untuk kompas. Ia memaparkan bearing
Kiblat, arah semasa peranti, ketepatan kompas dan sama ada utara benar atau
utara magnet digunakan. Kemas kini kompas hanya aktif ketika tab ini digunakan.

## Pemberitahuan

Pemberitahuan adalah pilihan dan kebenaran hanya diminta selepas anda
mengaktifkannya dalam Tetapan. Subuh, Zohor, Asar, Maghrib dan Isyak boleh
diaktifkan atau dinyahaktifkan secara berasingan.

Aplikasi menjadualkan sehingga 60 permintaan pemberitahuan setempat menggunakan
lokasi, zon waktu, kaedah pengiraan dan bahasa pilihan semasa. Penyampaian
diuruskan oleh iOS dan mungkin tidak berlaku tepat pada saat yang dikira. Buka
semula aplikasi secara berkala untuk memperbaharui jadual berterusan, dan buka
semula selepas perjalanan atau perubahan tetapan pengiraan.

Tiada perkhidmatan pemberitahuan jauh atau pelayan pemberitahuan yang
dikendalikan oleh pembangun digunakan.

## Widget Skrin Utama dan Skrin Kunci

Widget menggunakan gaya fasa hari dan hierarki maklumat yang sama seperti
aplikasi, dengan kandungan yang disesuaikan untuk setiap saiz:

- **Kecil:** solat seterusnya dan kira detik langsung.
- **Sederhana:** solat seterusnya bersama urutan waktu yang akan datang.
- **Besar:** jadual harian lengkap, penekanan solat seterusnya dan panduan
  tahrim semasa.
- **Skrin Kunci:** aksesori segi empat tepat, sebaris dan bulat.

Buka aplikasi utama sekali untuk memberikan lokasi semasa dan tetapan
pengiraan kepada widget. Aplikasi menyimpan satu petikan widget dalam App Group
peribadinya. Widget berhenti menggunakan petikan selepas tujuh hari dan meminta
anda membuka aplikasi untuk menyegarkannya. Selepas perjalanan, buka aplikasi
supaya widget menggunakan lokasi dan zon waktu baharu. Menekan widget Skrin
Utama membuka tab Hari Ini.

## Pengendalian lokasi latar hadapan

Aplikasi hanya meminta lokasi semasa sedang digunakan. Apabila anda kembali
daripada Skrin Utama atau aplikasi lain, jadual sah terakhir dan arah kiblat
kekal dipaparkan. Lokasi baharu hanya diminta apabila penentuan sebelumnya
melebihi lima minit.

Kegagalan sementara Core Location akan dicuba semula, manakala permintaan
lokasi dan geokod mempunyai had masa. Jika penyegaran tidak dapat diselesaikan,
keputusan sah sebelumnya kekal tersedia dan tidak digantikan dengan keadaan
memuat yang berterusan.

## Kaedah pengiraan yang tersedia

Aplikasi menyediakan JAKIM, Muslim World League, Umm al-Qura, Egyptian Survey,
Karachi, ISNA, Kemenag Indonesia, Diyanet, MUIS, Grande Mosquee de Paris,
UOIF / Musulmans de France, University of Tehran dan Leva Qum.

Kaedah aktif dipaparkan dalam bahagian Waktu Solat. Setiap pratetap mengawal
sudut senja, faktor bayang Asar, peraturan Maghrib, sela tetap Isyak dan
pelarasan yang berkenaan. Diyanet dan Grande Mosquee de Paris dilabel sebagai
anggaran keserasian, manakala pratetap Jaafari tidak memaparkan selang tahrim
Sunni umum aplikasi.

Semua waktu yang dipaparkan kekal sebagai anggaran berasaskan koordinat.
Jadual semasa yang rasmi bagi zon, kawasan, masjid atau pihak berkuasa agama
hendaklah diutamakan apabila terdapat perbezaan.

[Dasar Privasi](/my-prayer-times/privacy/) ·
[Sokongan](/my-prayer-times/support/)

My Prayer Times is not affiliated with or endorsed by any authority or
organisation named in the app.
