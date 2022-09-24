# Jarkom-Modul-1-D03-2022

### Kelompok D03

| **No** | **Nama**                   | **NRP**    |
| ------ | -------------------------- | ---------- |
| 1      | Antonio Taifan Montana     | 5025201219 |
| 2      | Wina Tungmiharja           | 5025201242 |
| 3      | Vania Rizky Juliana Wachid | 5025201215 |



# PEMBAHASAN

## 1. Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
-	Pertama, kita membuka file ```soal1-2.pcapng```

-	Kemudian menggunakan command ```tcp contains monta.if.its.ac.id``` pada  Display Filter  

![image](https://cdn.discordapp.com/attachments/869563207658913802/1022348757444067399/unknown.png)

-	Kita kemudian memilih salah satu packet, klik kanan, dan pilih ```Follow > TCP Stream```  

![image](https://cdn.discordapp.com/attachments/869563207658913802/1022349639195828324/unknown.png)

-	Kemudian akan muncul Pop-up seperti ini  

![image](https://cdn.discordapp.com/attachments/869563207658913802/1022349933153615882/unknown.png)

**Dari informasi diatas, terlihat bahwa Informasi server yang digunakan pada website tersebut adalah ```nginx/1.10.3```**



## 2.	Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?  

-	Pertama, kita memilih paket yang mengandung keyword ```detailTopik```  

![image](https://cdn.discordapp.com/attachments/869563207658913802/1022350579554603028/unknown.png)

-	Kemudian, kita klik kanan pada paket tersebut, dan memilih ```Follow > HTTP Stream```  

![image](https://cdn.discordapp.com/attachments/869563207658913802/1022350783284519023/unknown.png)

-	Lalu pada search input, kita dapat melakukan pencarian Topik ```Tugas Akhir```  

![image](https://cdn.discordapp.com/attachments/869563207658913802/1022351059303268402/unknown.png)    

**Dari hasil diatas, terlihat bahwa Topik Tugas Akhir yang dilihat ishaq adalah `Evaluasi unjuk kerja User Space Filesystem`**



## 3.	Filter sehingga wireshark hanya menampilkan paket yang menuju port 80! 

- Menggunakan command `tcp.dstport == 80 || udp.dstport == 80`

![image](https://user-images.githubusercontent.com/64743796/191659594-b0b69079-d5e0-4732-ace1-dbbc91bfc97c.png)



## 4.	Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!

- Menggunakan command `tcp.srcport == 21 || udp.srcport == 21`

![image](https://user-images.githubusercontent.com/64743796/191659666-74cddf69-5c70-4657-9543-60d0316d80be.png)
![image](https://user-images.githubusercontent.com/64743796/191659673-a83a389b-f47a-4be8-8f90-c904f6172156.png)



## 5.	Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!

- Menggunakan command `tcp.srcport == 443 || udp.srcport == 443`

![image](https://user-images.githubusercontent.com/64743796/191659735-4a29fb6d-10d9-4c91-9dd5-918fb513be0b.png)



## 6.	Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !

- Menggunakan command `http.host == "lipi.go.id"`

![image](https://user-images.githubusercontent.com/64743796/191659846-355432d0-e773-4b80-9ae3-e44a9a3d32e4.png)



## 7.	Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

- Untuk mengetahui IP kita, maka dari cmd, jalankan `ipconfig`

![image](https://user-images.githubusercontent.com/64743796/191660110-772e1cb1-fed5-4dd0-9063-4e409ec178bf.png)


- Menggunakan command `src host 192.168.123.35` pada Capture FIlter

![image](https://user-images.githubusercontent.com/64743796/191660285-e58049d9-b8e3-494f-afaf-0fcba8bf56e1.png)


Di sebuah planet bernama Viltrumite, terdapat Kementerian Komunikasi dan Informatika yang baru saja menetapkan kebijakan baru. Dalam kebijakan baru tersebut, pemerintah dapat mengakses data pribadi masyarakat secara bebas jika memang dibutuhkan, baik dengan maupun tanpa persetujuan pihak yang bersangkutan. Sebagai mahasiswa yang sedang melaksanakan program magang di kementerian tersebut, kalian mendapat tugas berupa penyadapan percakapan mahasiswa yang diduga melakukan tindak kecurangan dalam kegiatan Praktikum Komunikasi Data dan Jaringan Komputer 2022. Selain itu, terdapat sebuah password rahasia (flag) yang diduga merupakan milik sebuah organisasi bawah tanah yang selama ini tidak sejalan dengan pemerintahan Planet Viltrumite. Tunggu apa lagi, segera kerjakan tugas magang tersebut agar kalian bisa mendapatkan pujian serta kenaikan jabatan di kementerian tersebut!


## 8.	Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.

- Disini kita menggunakan display filter `tcp`

![image](https://cdn.discordapp.com/attachments/968145735713456189/1023207928427204608/Picture1.png)
![image](https://cdn.discordapp.com/attachments/968145735713456189/1023207938917146704/Picture2.png)
![image](https://cdn.discordapp.com/attachments/968145735713456189/1023207951986593824/Picture3.png)

