Cek di mana lokasi Anda sekarang:
# pwd

Buat folder baru khusus untuk latihan ini:
# mkdir latihan_terminal

Masuk ke dalam folder yang baru saja dibuat:
# cd latihan_terminal

Cek isi foldernya (pasti tidak muncul apa-apa karena masih kosong):
# ls

Buat sub-folder pertama bernama "dokumen":
# mkdir dokumen

Buat sub-folder kedua bernama "cadangan":
# mkdir cadangan

Lihat hasilnya, sekarang ada dua folder:
# ls -l

Coba masuk ke folder dokumen:
# cd dokumen

Cek lagi lokasi Anda saat ini (akan terlihat Anda ada di dalam folder dokumen):
# pwd

Mundur satu langkah kembali ke folder "latihan_terminal":
# cd ..

Tahap 2: Membuat dan Mengisi File
Buat sebuah file teks kosong bernama "catatan.txt":
# touch catatan.txt

Buat file teks kedua bernama "profil.txt":
# touch profil.txt

Cek apakah kedua file tersebut sudah terbuat:
# ls

Isi tulisan ke dalam file catatan.txt menggunakan perintah echo:
# echo "Ini adalah catatan pertama saya di terminal" > catatan.txt

Baca isi file catatan.txt yang baru saja Anda isi:
# cat catatan.txt

Sekarang isi file profil.txt dengan nama Anda:
# echo "Nama saya adalah Pengguna Terminal" > profil.txt

Tambahkan baris baru ke file profil.txt (gunakan >> agar teks sebelumnya tidak terhapus):
# echo "Saya sedang belajar 50 perintah dasar" >> profil.txt

Baca isi file profil.txt (sekarang harusnya ada dua baris teks):
# cat profil.txt

Gandakan (copy) file profil.txt menjadi file baru bernama "profil_copy.txt":
# cp profil.txt profil_copy.txt

Cek isi folder untuk melihat file hasil copy:
# ls

Tahap 3: Memindahkan dan Mengganti Nama
Pindahkan file profil_copy.txt ke dalam folder "cadangan":
# mv profil_copy.txt cadangan/

Cek isi folder cadangan untuk memastikan filenya sudah pindah:
# ls cadangan/

Ganti nama file "catatan.txt" menjadi "jurnal.txt":
# mv catatan.txt jurnal.txt

Cek lagi isi folder Anda saat ini (nama catatan.txt sudah berubah):
# ls

Copy file jurnal.txt ke dalam folder dokumen:
# cp jurnal.txt dokumen/

Masuk ke folder dokumen:
# cd dokumen

Pastikan filenya ada di sana:
# ls

Baca baris pertama saja dari file jurnal.txt:
# head -n 1 jurnal.txt

Baca baris terakhir dari file jurnal.txt:
# tail -n 1 jurnal.txt

Mundur lagi ke folder latihan_terminal:
# cd ..

Tahap 4: Pencarian dan Informasi Sistem
Cari kata "belajar" di dalam file profil.txt:
# grep "belajar" profil.txt

Cari di mana letak file bernama "jurnal.txt" berada di folder ini:
# find . -name "jurnal.txt"

Tampilkan tanggal dan waktu hari ini:
# date

Tampilkan kalender bulan ini:
# cal

Cek nama username komputer yang sedang Anda gunakan:
# whoami

Cek informasi sistem operasi Anda:
# uname -a

Cek berapa ukuran memori (kapasitas) folder latihan ini:
# du -sh

Cek sisa memori hardisk komputer Anda secara keseluruhan:
# df -h

Tampilkan semua file beserta ukuran dan hak aksesnya secara detail:
# ls -la

Ubah hak akses profil.txt agar bisa diedit oleh siapa saja (kode 777):
# chmod 777 profil.txt

Tahap 5: Arsip, Jaringan, dan Pembersihan (Cleanup)
Cek perubahan hak akses profil.txt (perhatikan huruf rwx di sebelah kiri):
# ls -l profil.txt

Jadikan folder "dokumen" dan "cadangan" menjadi satu file arsip (mirip ZIP):
# tar -cvf arsip_data.tar dokumen/ cadangan/

Cek apakah file "arsip_data.tar" sudah berhasil dibuat:
# ls

Uji koneksi internet komputer Anda ke server Google (hanya 3 kali ping):
# ping -c 3 8.8.8.8

Tampilkan riwayat semua perintah yang sudah Anda ketik dari tadi:
# history

Bersihkan layar terminal Anda yang sudah penuh dengan teks:
# clear

Mari kita mulai bersih-bersih, hapus file jurnal.txt yang ada di luar:
# rm jurnal.txt

Hapus folder "cadangan" beserta semua isi di dalamnya secara permanen:
# rm -r cadangan

Cek hasil akhirnya, folder sudah lebih bersih:
# ls

Cetak pesan kebanggaan di layar terminal Anda:
# echo "Selamat! Saya berhasil menyelesaikan 50 perintah Command Line!"

Menjalankan perintah dengan hak akses administrator penuh (Superuser).
# sudo
 
Melihat daftar koneksi jaringan, protokol, dan port yang sedang aktif.
# netstat

Menampilkan daftar proses aplikasi yang saat ini sedang berjalan di background.
# ps

Memantau kinerja prosesor (CPU) dan RAM secara real-time (mirip Task Manager).
# top

Menghentikan paksa sebuah proses aplikasi yang macet menggunakan nomor ID-nya (PID).
# kill

Menghentikan seluruh proses secara serentak berdasarkan nama aplikasinya.
#killall

Menampilkan rincian sisa kapasitas RAM dan ruang Swap komputer.
#free

Melihat durasi komputer atau server menyala sejak restart terakhir
#uptime

Menampilkan buku panduan (manual) resmi dari sebuah perintah (contoh: man ls untuk melihat cara pakai ls).
# man

Membuat kata kunci (shortcut) baru untuk mempersingkat perintah yang panjang.
# alias

Menghapus kata kunci shortcut yang sebelumnya sudah Anda buat dengan perintah alias.
# unalias

Fungsinya untuk memperbarui daftar (katalog) aplikasi dari server pusat Linux.
# sudo apt update

Fungsinya untuk memasang (menginstal) pembaruan ke sistem Anda. 
# sudo apt upgrade

Fungsinya untuk mengunduh dan menginstal aplikasi baru ke dalam system
# sudo apt install nama_paket

Fungsinya untuk menghapus (uninstall) aplikasi dari komputer Anda
# sudo apt remove nama_paket 

menampilkan daftar semua aplikasi yang sudah terinstal 
# dpkg -l

menampilkan daftar semua proses program yang sedang berjalan.
# ps aux 
