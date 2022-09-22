# Jarkom-Modul-1-D03-2022

### Kelompok D03

| **No** | **Nama**                   | **NRP**    |
| ------ | -------------------------- | ---------- |
| 1      | Antonio Taifan Montana     | 5025201219 |
| 2      | Wina Tungmiharja           | 5025201242 |
| 3      | Vania Rizky Juliana Wachid | 5025201215 |

# PEMBAHASAN
### 1. Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 
-	Pertama, kita membuka file ```soal1-2.pcapng```
-	Kemudian menggunakan command ```tcp contains monta.if.its.ac.id``` pada  Display Filter  
![image](https://cdn.discordapp.com/attachments/869563207658913802/1022348757444067399/unknown.png)

-	Kita kemudian memilih salah satu packet, klik kanan, dan pilih ```Follow > TCP Stream```  
![image](https://cdn.discordapp.com/attachments/869563207658913802/1022349639195828324/unknown.png)

-	Kemudian akan muncul Pop-up seperti ini  
![image](https://cdn.discordapp.com/attachments/869563207658913802/1022349933153615882/unknown.png)

#### Dari infromasi diatas, terlihat bahwa Informasi server yang digunakan pada website tersebut adalah ```nginx/1.10.3```

### 2.	Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?  
-	Pertama, kita memilih paket yang mengandung keyword ```detailTopik```  
![image](https://cdn.discordapp.com/attachments/869563207658913802/1022350579554603028/unknown.png)

-	Kemudian, kita klik kanan pada paket tersebut, dan memilih ```Follow > HTTP Stream```  
![image](https://cdn.discordapp.com/attachments/869563207658913802/1022350783284519023/unknown.png)

-	Lalu pada search input, kita dapat melakukan pencarian Topik ```Tugas Akhir```  
![image](https://cdn.discordapp.com/attachments/869563207658913802/1022351059303268402/unknown.png)    
#### Dari hasil diatas, terlihat bahwa Topik Tugas Akhir yang dilihat ishaq adalah ```Evaluasi unjuk kerja User Space Filesystem```







