# tugas-akhir-2
**1. Membuat Repository Lokal**
<img width="227" height="42" alt="Screenshot 2025-11-05 194744" src="https://github.com/user-attachments/assets/f972f941-045d-4b06-a80d-80ee5f320ec4" />
pertama kita membuat direktori yang saya beri nama tugas-akhir-2

<img width="227" height="40" alt="Screenshot 2025-11-05 194751" src="https://github.com/user-attachments/assets/09cb27e0-ff8c-4408-b7d2-dc39212868b9" />
selanjutnya kita masuk direktorinya untuk membuat file

**2. Inisialisasi Git repository**
<img width="644" height="62" alt="Screenshot 2025-11-05 194757" src="https://github.com/user-attachments/assets/108c5ce2-205b-4ec9-9606-7cdf90d00de1" />
selanjutnya disini kita melakukan git init untuk menginisialisasi repository git baru

<img width="421" height="113" alt="Screenshot 2025-11-05 194803" src="https://github.com/user-attachments/assets/bbcb3994-ff18-4f45-8342-ecc06426ed12" />
selanjutnya ada perintah ls -la untuk menampilkan daftar semua file dan folder dalam direktori saat ini

**3. Check Status, ADD file, dan Melakukan Commit**
<img width="694" height="535" alt="Screenshot 2025-11-05 200343" src="https://github.com/user-attachments/assets/92dfbd64-6e70-48ad-8e7d-12314097b290" />
Selanjutnya terdapat perintah Git untuk mengelola perubahan di repositori. Perintah pertama git status digunakan untuk melihat kondisi repositori saat ini dan hasilnya menunjukkan ada tiga file baru (PP.jpg, TA1.css, dan TAI.html) yang masih berstatus untracked, artinya Git belum melacak file-file tersebut. Setelah itu saya lanjut menjalankan git add TAI.html, yang berfungsi menambahkan file TA1.html ke dalam staging area, yaitu tahap persiapan sebelum file disimpan ke dalam repositori melalui commit. Lalu terdapat git status lagi, terlihat bahwa file TA1.html sudah berada di daftar Changes to be committed, artinya siap untuk di-commit, sementara dua file lainnya (PP.jpg dan TAI.css) masih belum ditambahkan dan tetap berstatus untracked

<img width="528" height="315" alt="Screenshot 2025-11-05 200743" src="https://github.com/user-attachments/assets/be445003-820f-4bd2-950d-6579d40bcc55" />
selanjutnya terdapat perintah git commit untuk menyimpan file TA1.html sebagai "Initial commit," yang menciptakan mode file baru untuk TA1.html. Setelah komit awal ini, saya menambahkan file untuk disiapkan yaitu TA1.css dan PP.jpg lalu saya jalankan perintah git add secara terpisah, untuk memindahkannya ke staging area. Terakhir saya membuat komit kedua dengan pesan "Initial TA1 css and Profile Image," untuk menyimpan kedua file yang di-stage tersebut, sehingga kini file TA1.css dan PP.jpg tercatat dalam riwayat repositori.


**4. Membuat repository baru di GitHub**
<img width="595" height="56" alt="Screenshot 2025-11-05 201628" src="https://github.com/user-attachments/assets/1593d404-ee56-43c0-99c6-6daa6c372896" />
selanjutnya disini terdapat perintah git remote untuk untuk menghubungkan repository lokal saya dengan repository yang ada digithub 

**5. Push ke Remote Repository**
<img width="559" height="195" alt="Screenshot 2025-11-05 201640" src="https://github.com/user-attachments/assets/267f5e55-d309-4605-84d1-d19c776a9f60" />
selanjtunya disini ada perintah it push -u origin main, yang berfungsi untuk mengirimkan semua komit terbaru dari repositori lokal pada cabang main ke repositori jarak jauh yang diberi nama alias origin, yang dalam kasus ini terhubung ke GitHub pada URL https://github.com/Arlopen/tugas-akhir-2.


**6. Membuat Branch untuk proyek-saya**
<img width="410" height="111" alt="Screenshot 2025-11-05 202754" src="https://github.com/user-attachments/assets/ff506468-8ba5-4ada-ab2b-fde8a64ae338" />
selanjutnya terdapat perintah git branch proyek-saya yang berfungsi untuk membuat cabang baru bernama proyek-saya berdasarkan kondisi saat ini dari cabang main. Setelah cabang baru berhasil dibuat, perintah selanjutnya git checkout proyek-saya digunakan untuk berpindah dari cabang main ke cabang yang baru dibuat tersebut, dikonfirmasi oleh pesan “Switched to branch 'proyek-saya'”, yang berarti semua pekerjaan dan commit yang dilakukan setelah ini akan tercatat hanya pada cabang proyek-saya dan tidak akan memengaruhi cabang main yang stabil.

**7. Melakukan Commit di proyek-saya Branch**
<img width="475" height="127" alt="Screenshot 2025-11-05 202802" src="https://github.com/user-attachments/assets/ab243094-03ea-45c4-8194-3b28412e216b" />
Selanjutnya terdapat perintah git add . digunakan untuk menambahkan semua perubahan (file yang dimodifikasi, ditambahkan, atau dihapus) di direktori kerja saat ini ke dalam staging area, mempersiapkannya untuk komit. Setelah semua perubahan di-stage, perintah git commit -m "Add section Proyek saya" dijalankan untuk menyimpan perubahan tersebut secara permanen ke riwayat cabang proyek-saya. Hasilnya, sebuah komit baru berhasil dibuat (027b863) dengan pesan yang jelas, mencatat bahwa 2 file telah diubah dengan total 42 penambahan baris, yang semuanya kini hanya ada pada riwayat pengembangan cabang proyek-saya.

**8. Merge ke main Branch**
<img width="468" height="277" alt="Screenshot 2025-11-05 202920" src="https://github.com/user-attachments/assets/c73b18e3-a0fe-4d9f-84c6-456ad6e9bc7b" />
Selanjtunya disini ktia menggabungkan dan membersihkan cabang proyek-saya. Langkah pertama adalah git checkout main untuk kembali ke cabang utama (main) yang stabil, dikonfirmasi dengan pesan “Switched to branch 'main'” dan status bahwa cabang ini sudah up to date dengan remote. Selanjutnya, perintah git merge proyek-saya dijalankan untuk menggabungkan perubahan dari proyek-saya ke dalam main, yang dilakukan dengan metode Fast-forward karena main tidak memiliki commit baru sejak proyek-saya dibuat, menghasilkan pembaruan 2 file dengan 42 penambahan baris. Terakhir, setelah penggabungan berhasil, perintah git branch -d proyek-saya digunakan untuk menghapus cabang proyek-saya secara lokal, karena pekerjaan di dalamnya sudah aman tersimpan di main.


