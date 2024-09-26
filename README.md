 
# 1.	Eksekusi seluruh profile yang ada : 
## a.	 Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
![1](https://github.com/user-attachments/assets/c272beff-5786-45a1-b689-b51ecd12b589)
![2](https://github.com/user-attachments/assets/bf3d3efd-6cf9-48ef-95cb-1c667e36ff2d)

Penjelasan: Ini menambahkan pesan "Profile dari /etc/profile" yang akan ditampilkan setiap kali file profile dieksekusi.

## b.	Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
/home/stD02001/.bash_profile
/home/. stD02001/.bash_login
/home/mahasiswa/.profile
/home/mahasiswa/.bashrc
Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap
file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :
echo “Profile dari .bash_profile”
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.

![3](https://github.com/user-attachments/assets/06f3cedb-0858-4b38-8397-2c526241a875)
![4](https://github.com/user-attachments/assets/cf35c2ae-c8ff-44de-915b-88780233dcb6)
![5](https://github.com/user-attachments/assets/094b1365-9721-47f5-863d-526e89e35d4f)
![6](https://github.com/user-attachments/assets/0f6292bc-a5a3-40f2-8119-24abd10bd862)
![7](https://github.com/user-attachments/assets/56174119-a9ed-4f22-b83e-8971b380e8df)
![8](https://github.com/user-attachments/assets/bf0d6bfb-b436-4d11-86ad-e2ab6d8270c1)
![9](https://github.com/user-attachments/assets/c9a26bf2-2441-4162-b166-fd01d1185c50)
![10](https://github.com/user-attachments/assets/0656997d-c0bf-4128-a1ec-51c0031aa124)
![11](https://github.com/user-attachments/assets/c023be7a-a006-44c0-bafa-1de9bd5fd874)

Penjelasan: Perintah ini menambahkan pesan pada setiap file profil pengguna stD02001, yang akan ditampilkan saat file tersebut dieksekusi.

## c.	Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:
$ su mahasiswa
$ exit
kemudian gunakan opsi – sebagai berikut :
$ su – mahasiswa
$ exit
Jelaskan perbedaan kedua utilitas tersebut.
![16](https://github.com/user-attachments/assets/81e08270-9615-4c10-a6f3-72d464acb965)

Penjelasan:
su mahasiswa: Mengganti pengguna ke mahasiswa tanpa menjalankan shell login, sehingga tidak membaca file profile seperti .bash_profile.
su - mahasiswa: Mengganti pengguna ke mahasiswa dengan shell login penuh, sehingga semua file profile akan dieksekusi.

# 2.	Prompt String (PS)
## a.	Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
![18](https://github.com/user-attachments/assets/40652182-cf78-457b-a373-a72f25cf02c9)

## b.	Eksperimen hasil PS1 :
![17](https://github.com/user-attachments/assets/6dcb7287-58a8-4966-8653-72e109982960)

# 3.	Logout 
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
![19](https://github.com/user-attachments/assets/5201a866-d9fa-467b-a3d9-0f6e93b2f086)

Penjelasan: Menampilkan pesan "Terima kasih atas sesi yang diberikan", menunggu 5 detik, dan membersihkan layar sebelum keluar dari sesi shell.

# 4.	Bach script
## a.	Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
p1.sh
#! /bin/bash
echo “Program p1”
ls –l
p2.sh
#! /bin/bash
echo “Program p2”
who
p3.sh
#! /bin/bash
echo “Program p3”
ps x
![20](https://github.com/user-attachments/assets/fbc6e7dc-e26d-4b0b-8215-f79299271d5f)
![21](https://github.com/user-attachments/assets/d9df4978-de70-4074-8a1c-c3af51925970)
![22](https://github.com/user-attachments/assets/04fe2afc-32bd-4e2f-9e4f-3a1f2d7db3e1)
![23](https://github.com/user-attachments/assets/806b93ae-3ef7-4c2d-b0cb-c36c5e12ee60)
![24](https://github.com/user-attachments/assets/183b18e2-962d-444b-ad1c-cf0cae8afb35)
![25](https://github.com/user-attachments/assets/b1a0c4c7-258d-4055-bbd3-87a06abf4951)

## b.	Jalankan script tersebut sebagai berikut :
![26](https://github.com/user-attachments/assets/c3aced38-df42-4f46-ba34-4749b7d460cc)
![27](https://github.com/user-attachments/assets/012b07d4-edb0-40b8-b22a-a7fab5a3c2a6)
![28](https://github.com/user-attachments/assets/9c67762d-8dec-4d71-acb4-f27031d67b4c)
![29](https://github.com/user-attachments/assets/511d8876-8028-4019-be8c-2b158522c047)
![30](https://github.com/user-attachments/assets/e4a77b0a-47cf-4589-bca5-cd296dcf3273)

Penjelasan: Menjalankan script dengan berbagai metode: secara berurutan, paralel, dan dalam subshell di background.

# 5.	Jobs
## a.	Buat shell-script yang melakukan loop dengan nama pwaktu.sh, 
setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.
![31](https://github.com/user-attachments/assets/bd991f51-7748-4134-bcda-405a1c9e4243)
![32](https://github.com/user-attachments/assets/381ac2c7-844d-4964-81ec-d101043d383f)

Penjelasan: Script ini mencatat tanggal dan waktu ke file hasil setiap 10 detik.

## b.	Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :
![33](https://github.com/user-attachments/assets/2516be2c-cc4d-472a-b24e-48dfa7eb4881)

Penjelasan: Melihat dan menjalankan beberapa proses di background dengan jobs.

## c.	Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background
![34](https://github.com/user-attachments/assets/a23edeff-2573-48fd-9e7e-fbc76ed37701)

Penjelasan: Mengelola proses foreground dan background.

## d.	Stop program background dengan utilitas kil
![35](https://github.com/user-attachments/assets/77ddb42a-ee32-49b4-bfa5-785942f11ddd)
![36](https://github.com/user-attachments/assets/2ca5866f-9e74-4569-abba-0c56758f08bc)

Penjelasan: Menghentikan proses dengan kill berdasarkan PID.

# 6.	History
## a.	Ganti nilai HISTSIZE dari 1000 menjadi 20
![37](https://github.com/user-attachments/assets/c9727418-8099-4b1e-8472-19ea3ff6c979)

Penjelasan: Mengurangi ukuran buffer history menjadi 20.

## b.	Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan
![38](https://github.com/user-attachments/assets/3843349b-607c-4273-8a06-45ecf855d05b)

Penjelasan: Menjalankan ulang perintah yang ke-5 dari belakang.

## c.	Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history buffer
![39](https://github.com/user-attachments/assets/e5fde0a3-9366-4281-aeb4-486da34c477e)

Penjelasan: Menggunakan navigasi history buffer dengan ^P (ke atas) dan ^N (ke bawah).

##  d.	Ulangi instruksi pada history bufer nomor 150
![40](https://github.com/user-attachments/assets/62be795b-3c49-4166-b486-fc1b49b88036)

Penjelasan: Menjalankan ulang perintah yang berada pada posisi 150 di history.

## e.	Ulangi instruksi dengan prefix “ls”
![41](https://github.com/user-attachments/assets/e2e8833e-66c2-4e66-b658-65df58d00412)

Penjelasan: Menjalankan ulang perintah terakhir yang dimulai dengan ls.
