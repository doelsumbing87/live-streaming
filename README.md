# LIVE STREAMING WITH TELEGRAM BOT

## FITUR :
-  Upload Video by Telegram Bot ( MAX FILE UPLOAD 50MB ) , BISA UPLOAD MANUAL KE SERVER DEPLOY VPS / RDP KALAU DIATAS 50 MB
- Setting RTMP ( Support Youtube / Facebook Live stream )
- Input Stream key
- Set Video to target live
- Set resolution , buat setting resolusi Live ( semakin tinggi resolusinya. semakin berat ) saran gunakan 720p60 untuk spek VPS / RDP 8GB RAM 4CPU
- Mode Live ( Potrait or Landspace ). Potrait = Vertikal , Landspace = Horizontal
- Auto Looping. Bisa di atur ON / OFF
- Start Live. untuk memulai Live streaming , seteleah  semua disetting ( Set RTMP > Input Stream Key > Pilih Video > Set Resolusi > Mode Live > Auto Looping )
- Stop Live. untuk menghentikan Live
- Jadwal Stop, otomatis stop live untuk dijadwalkan
- Hapus Video, untuk menghapus video yang ada di folder
- Show Configure , untuk melihat konfigurasi yang di setting
- Cek Status Live , untuk nampilin status Live ( by FFMPEG status )

## FITUR TAMBAHAN :
- Auto Reconnect, Otomatis Reconnect ke live jika terputus max 3x

Cara Penggunaan bisa kalian tonton pada video ini :

## UBUNTU :
[YOTUBE : CARA INSTALL AOTUO LOOPING STREAMING. CLICK INI KOCAK](https://youtu.be/Qqm2LUaOkBA)

## WINDOWS :
COMING SOON

Langkah-langkah Menjalankan Proyek
Instal Python: Pastikan Anda sudah menginstal Python di sistem Anda. Anda bisa mengunduhnya dari situs resmi Python.

Buat dan Aktifkan Lingkungan Virtual (venv):
Ini adalah praktik yang baik untuk mengisolasi dependensi proyek Anda.

Bash

`python -m venv venv`
Untuk mengaktifkan lingkungan virtual:

Di Windows:
Bash

.\venv\Scripts\activate
Di macOS/Linux:
Bash

`source venv/bin/activate`
Instal Dependensi:
Setelah lingkungan virtual aktif, instal semua dependensi yang diperlukan dari file requirements.txt.

Bash

`pip install -r requirements.txt`
Konfigurasi config.json:
Anda perlu memasukkan ID obrolan Telegram Anda dan token bot yang Anda dapatkan dari BotFather ke dalam file config.json. Pastikan formatnya benar sesuai dengan struktur JSON.

Jalankan Skrip Python:
Setelah semua konfigurasi selesai, Anda bisa menjalankan skrip Python utama.

Bash

python bot.py

Setup di Bot Telegram:
Setelah bot berjalan, lakukan penyiapan atau interaksi awal yang diperlukan di bot Telegram yang telah Anda buat melalui BotFather. Ini mungkin melibatkan mengirim perintah /start atau perintah lain yang relevan untuk bot Anda.


CARA UPLOAD VIDEO JIKA DIATAS 50MB KE VPS 

`scp "/mnt/d/Downloads/konten1!/contoh.mp4" root@IP_VPS:/root/live-streaming/videos/`
