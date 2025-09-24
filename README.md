![alt text](https://c.top4top.io/p_35541lw0j1.png?raw=true)
🔍 Penjelasan Umum

Script ini ditujukan untuk digunakan oleh peretas atau defacer untuk mengunggah file deface (biasanya halaman HTML atau PHP berisi pesan hacking) ke banyak direktori sekaligus secara otomatis.

🧨 Tujuan Utama Script

Script ini dirancang untuk:

1. Membypass proteksi server seperti: LiteSpeed Cache (LSCache), Imunify360, ModSecurity, Cloudflare, Wordfence (plugin keamanan WordPress)
2. Menulis file deface (index.php) ke semua subdirektori dari direktori utama (base_dir) yang diinput pengguna.


Bypass dilakukan dengan cara:

Memeriksa apakah sistem memiliki plugin keamanan tertentu.
Mengatur header tertentu agar plugin-plugin itu mengabaikan request ini atau menganggap request valid.

💥 Bypass yang dilakukan:

X-LSCACHE: off → Mematikan cache LiteSpeed (mencegah tampilan lama).

X-Imunify360-Request: bypass → Lewati proteksi Imunify360.

X-Imunify360-Captcha-Bypass → Lewati captcha.

X-Mod-Security → Menyesuaikan dengan header dari Apache jika terdeteksi.

REMOTE_ADDR dimodifikasi agar menyamarkan IP asli pengguna melalui Cloudflare.

🚨 Kesimpulan

Kode ini adalah web shell berbahaya yang digunakan untuk:

Melakukan mass defacing pada situs web yang sudah berhasil diretas.

Menghindari deteksi sistem keamanan menggunakan teknik header spoofing dan pengaturan server internal.

