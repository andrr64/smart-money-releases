# smart-money-releases

Repositori ini hanya berisi **rilis APK** Smart Money: berkas `smart-money-X.Y.Z.apk` dan catatan rilisnya. Source code ada di repositori privat, jadi tidak ada kode di sini.

## Untuk pengguna

- Buka rilis terbaru di tab **Releases**, lalu unduh `smart-money-X.Y.Z.apk`.
- Atau buka Smart Money › Pengaturan › Tentang › **Cek pembaruan**. Aplikasi membaca rilis terbaru dari repositori ini.

## Untuk pengembang

- Aplikasi memanggil `GET https://api.github.com/repos/andrr64/smart-money-releases/releases/latest` tanpa login. Endpoint ini hanya membaca rilis yang **tidak** ditandai pra-rilis atau draf. Jadi rilis yang harus dibaca aplikasi harus berupa rilis biasa.
- Aset APK harus berakhiran `.apk`. Aplikasi memilih aset pertama yang berakhiran itu.
- Tag rilis berbentuk `vX.Y.Z`. Aplikasi membuang awalan `v` sebelum membandingkan versi.
