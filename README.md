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

3. Which user logged in on Sep 19, 2025 23:17:44 (GMT+7)?

4. What time did one of the public computers got access to admin user? 

5. Which IP accessed the admin user? 

6. How did the attacker gain access to the admin user? 

7. What book did the attacker delete? 

8. The attacker added a new book to the database, what was it called? 

9. How did the attacker successfully leak all the usernames and passwords?

10. What was the password hash of admin account?
