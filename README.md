# Quiz-Network-Traffic-Analysis

## Kelompok 15

## Anggota

| Nama                      | NRP        |
| ------------------------- | ---------- |
| Wildan Alfarezy       | 5027251088 |
| Muhammad Yusuf | 5027251067 |

## Laporan (Soal No 2)

1. What is the IP and Port of the web server? 

jawaban: IP 192.168.223.129 port 4167

Gunakan filter di wireshark dengan mengetik `http` lalu kami cari paket dengan tulisan `Get/login` dari situ kami bisa mendapatkan `host` yang berisikan `ip` beserta `port` web servernya di bagian hypertext transfer protocol. 

![alt text](assets/soal1.png)

jadi suatu browser itu meminta halaman web, browser diwajibkan untuk mengirim informasi bernama `Host` yang berisi alamat tujuan. jadi dari situ kamii bisa tau bahwa apa pun yang tertulis di `Host` adalah alamat `IP (atau domain)` dan `Port` dari web server yang sedang diakses.

2. To help with viewing the server packets going in and out, what's a good filter to use and why? 

Untuk melihat paket keluar dan masuk, kita bisa menggunakan filter `ip.addr == <ip>` kemudian jika ingin memfilter paket yang keluar saja bisa menggunakan `ip.src == <ip>`, lalu untuk paket yang masuk bisa menggunakan `ip.dst == <ip>`

Paket dari ip `192.168.223.129` yang masuk dan juga keluar
  ![alt text](assets/image.png)

Paket yang masuk ke ip `192.168.223.129`
  ![alt text](assets/image1.png)

Paket yang keluar dari ip `192.168.223.129`
  ![alt text](assets/image2.png)

Filter yang sebaiknya digunakan adalah filter keluar atau masuk dari ip tertentu secara tersendiri, seperti `ip.dst == <ip>` atau `ip.src == <ip>`, kenapa tidak menggunakan `ip.addr == <ip>`, karena walaupun ip sudah terfilter, paket yang masuk dan keluar tetap terlihat, sehingga masih lumayan susah untuk mencari penyerang yang menyusupkan paket mencurigakan, Dengan filter keluar atau masuk, kita dapat melihat siapa yang mengirim ataupun siapa yang dikirim secara terpisah.

3. Which user logged in on Sep 19, 2025 23:17:44 (GMT+7)?

4. What time did one of the public computers got access to admin user? 

5. Which IP accessed the admin user? 

6. How did the attacker gain access to the admin user? 

7. What book did the attacker delete? 

8. The attacker added a new book to the database, what was it called? 

9. How did the attacker successfully leak all the usernames and passwords?

10. What was the password hash of admin account?
