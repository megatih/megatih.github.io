---
layout: page
title: My Prayer Times
subtitle: Prayer notifications, widgets, location-aware calculations, and Qibla direction
permalink: /my-prayer-times/
---

My Prayer Times is an iPhone and iPad app that calculates local prayer times,
tahrim intervals, and Qibla direction from your current coordinates.

The app automatically selects a documented prayer-time authority or convention
for supported countries, with Umm al-Qura University, Makkah as the fallback.
You can override the automatic choice in Settings, and the manual selection
remains active across launches and location changes.

- No account, advertising, analytics, or tracking
- Prayer overview with local time, next prayer, remaining time, and tahrim status
- Location-based calculations for local prayer times
- 13 selectable authority and convention presets
- Automatic matching for supported countries with an Umm al-Qura fallback
- Persistent manual selection and transparent calculation parameters
- Qibla direction with true-north and magnetic-north handling
- System, English, and Bahasa Melayu language choices
- Configurable local notifications for the five obligatory prayers
- Next Prayer widgets for the Home Screen and Lock Screen
- Resilient foreground location refresh without background location access
- Designed for iOS 17 and later

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

## Next Prayer widgets

The Next Prayer widget is available in small and medium Home Screen sizes and
in rectangular, inline, and circular Lock Screen accessory families. It shows
the next prayer and a live remaining-time countdown.

Open the main app once to provide the widget with a current location and
calculation setting. The app stores one widget snapshot in its private App
Group. The widget stops using a snapshot after seven days and asks you to open
the app to refresh it. After travelling, open the app so the widget can use
the new location and time zone.

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
- Ringkasan solat dengan waktu setempat, waktu seterusnya, baki masa dan status tahrim
- Pengiraan berdasarkan lokasi untuk waktu solat setempat
- 13 pratetap pihak berkuasa dan konvensyen
- Padanan automatik bagi negara yang disokong dengan sandaran Umm al-Qura
- Pilihan manual yang kekal serta parameter pengiraan yang telus
- Arah kiblat dengan pengendalian utara benar dan utara magnet
- Pilihan bahasa Sistem, Bahasa Inggeris dan Bahasa Melayu
- Pemberitahuan setempat yang boleh dikonfigurasi bagi lima waktu solat fardu
- Widget Solat Seterusnya untuk Skrin Utama dan Skrin Kunci
- Penyegaran lokasi latar hadapan yang kukuh tanpa akses lokasi latar belakang
- Direka untuk iOS 17 dan lebih baharu

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

## Widget Solat Seterusnya

Widget Solat Seterusnya tersedia dalam saiz kecil dan sederhana pada Skrin
Utama serta keluarga aksesori segi empat tepat, sebaris dan bulat pada Skrin
Kunci. Widget memaparkan waktu solat seterusnya dan kira detik baki masa secara
langsung.

Buka aplikasi utama sekali untuk memberikan lokasi semasa dan tetapan
pengiraan kepada widget. Aplikasi menyimpan satu petikan widget dalam App Group
peribadinya. Widget berhenti menggunakan petikan selepas tujuh hari dan meminta
anda membuka aplikasi untuk menyegarkannya. Selepas perjalanan, buka aplikasi
supaya widget menggunakan lokasi dan zon waktu baharu.

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
