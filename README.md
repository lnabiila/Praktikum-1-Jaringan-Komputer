[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/8b_y5Av8)
| Name           | NRP        | Kelas     |
| ---            | ---        | ----------|
| Hilmi Fawwaz Sa'ad | 5025221103 | Jaringan Komputer (A) |
| Lathiifah Nabiila Bakhtiar | 5025221130 | Jaringan Komputer (A) |

## Task 1

> a. Berapa banyak packet yang terekam pada file pcapng?

> _a. How many packets are recorded in the pcapng file?_

**Answer:**

- Flag

  `JARKOM24{K4mu_K3r3n_Ko1NI5Z4J9MMOH0YJPLZ57FTI3GCSA0xL4ughplzarg3qdw2rmcntrskwaa7}`

- Filter expression

  `None (-)`
  
- Explanation

  `Saat membuka file soal, terlihat jumlah packet di bagian paling bawah display wireshark`
  ![image](https://github.com/user-attachments/assets/4abd24d5-39b4-4d74-a8ff-fd077b7933d3)
  
- Output result

  ![Screenshot 2024-09-11 183328](https://github.com/user-attachments/assets/073a398e-73c0-465b-bd0b-71078c155c62)

<br>
<br>

> b. Ada berapa jenis protocol yang terekam pada traffic

> _b. How many types of protocols are recorded in the traffic?_

**Answer:**

- Flag

  `JARKOM24{K4mu_K3r3n_Ko1NI5Z4J9MMOH0YJPLZ57FTI3GCSA0xL4ughplzarg3qdw2rmcntrskwaa7}`

- Filter expression

  `None (-)`
  
- Explanation

  `Klik "Protocol" sehingga protocol-protocolnya terurut. Dengan hitung manual, maka akan menemukan 4 protocol`
  <br>
  ![image](https://github.com/user-attachments/assets/4135db29-4925-4fdf-bc78-fe484a83df0d)
  ![image](https://github.com/user-attachments/assets/068da1b0-bbb5-47e6-a8e4-fd917e48c8f4)

- Output result

  ![Screenshot 2024-09-11 183328](https://github.com/user-attachments/assets/edfb71ed-eb3e-4ed9-9b5a-3d0498b657be)

<br>
<br>

> c. Sebutkan secara berurutan berdasarkan alfabet menurun dengan koma sebagai separator, contoh: protocol1,protocol2

> _c. List the protocols in descending alphabetical order, separated by commas. Example: protocol1,protocol2_

**Answer:**

- Flag

  `JARKOM24{K4mu_K3r3n_Ko1NI5Z4J9MMOH0YJPLZ57FTI3GCSA0xL4ughplzarg3qdw2rmcntrskwaa7}`

- Filter expression

  `None (-)`
  
- Explanation

  `Klik "Protocol" sehingga protocol-protocolnya terurut. Dengan hitung manual, ditemukan terdapat 4 protocol, yaitu HTTP, MDNS, SSDP, dan TCP`
  <br>
  ![image](https://github.com/user-attachments/assets/4135db29-4925-4fdf-bc78-fe484a83df0d)
  ![image](https://github.com/user-attachments/assets/068da1b0-bbb5-47e6-a8e4-fd917e48c8f4)

- Output result

  ![Screenshot 2024-09-11 183328](https://github.com/user-attachments/assets/dc9afbd2-3924-4d3a-9f5e-fdf71ac40093)

## Task 2

> a. Berapa banyak packet berbasis TCP yang memiliki flag [RST, ACK]

> _a. How many TCP based packets have the flags [RST, ACK]?_

**Answer:**

- Flag

`JARKOM24{W0w_4nother_Sh0t_VNUTTLKSVEH0mptyrnyqhtzpgzxmrvhryjocM4r139310488841829416611}`

- Filter expression

  `tcp.flags.ack == 1 && tcp.flags.reset == 1`
  
- Explanation

  `Untuk mencari packet berbasis TCP yang memiliki flag [RST, ACK] bisa menggunakan filter di atas yang kemudian hasilnya (jumlah packet) akan terlihat di bagian paling bawah display wireshark`
  <br>
  ![image](https://github.com/user-attachments/assets/3e0de027-3e4d-466f-986c-9460f6a211e0)

- Output result

  ![Screenshot 2024-09-11 184855](https://github.com/user-attachments/assets/5bb124e7-07a9-4e8a-9a5c-c024aaa891e3)

<br>
<br>

> b. How many TCP based packets have only the [SYN] flag?

> _b. How many TCP based packets have only the [SYN] flag?_

**Answer:**

- Flag

  `JARKOM24{W0w_4nother_Sh0t_VNUTTLKSVEH0mptyrnyqhtzpgzxmrvhryjocM4r139310488841829416611}`

- Filter expression

  `tcp.flags.ack == 0 && tcp.flags.reset == 0`
  
- Explanation

  `Untuk mencari packet berbasis TCP yang memiliki flag [SYN] bisa menggunakan filter di atas yang kemudian hasilnya (jumlah packet) akan terlihat di bagian paling bawah display wireshark`
  <br>
  ![image](https://github.com/user-attachments/assets/cc47655b-7bb6-4648-ae62-7d1b8da1dbee)

- Output result

  ![Screenshot 2024-09-11 184855](https://github.com/user-attachments/assets/5bb124e7-07a9-4e8a-9a5c-c024aaa891e3)

<br>
<br>

> c. How many TCP based packets have the ACK flag but do not have SYN or RST?

> _c. How many TCP based packets have the ACK flag but do not have SYN or RST?_

**Answer:**

- Flag

  `JARKOM24{W0w_4nother_Sh0t_VNUTTLKSVEH0mptyrnyqhtzpgzxmrvhryjocM4r139310488841829416611}`

- Filter expression

  `tcp.flags.syn == 0 && tcp.flags.reset == 0`
  
- Explanation

  `Untuk mencari packet berbasis TCP yang memiliki flag [ACK] bisa menggunakan filter di atas yang kemudian hasilnya (jumlah packet) akan terlihat di bagian paling bawah display wireshark`
  <br>
  ![image](https://github.com/user-attachments/assets/47f07336-0e8d-46c6-8e20-992329ca8438)

- Output result

  ![Screenshot 2024-09-11 184855](https://github.com/user-attachments/assets/5bb124e7-07a9-4e8a-9a5c-c024aaa891e3)

<br>
<br>

## Task 3

> a. Pada port berapa server http terbuka?

> _a. On which port is the HTTP server open?_


**Answer:**

- Flag

  `JARKOM24{Y0u_4r3_4_g00d_4nalyz3r_E447XL1tsbjwgvsnlprllzoalscdlji}`

- Filter expression

  `http`
  
- Explanation

  `Setelah melakukan filter, dapat dilihat pada destination port packet paling atas adalah 9282 yang merupakan destination port dari HTTP`
  <br>
  ![WhatsApp Image 2024-09-12 at 23 30 51](https://github.com/user-attachments/assets/60e73368-1a1c-4321-86f0-7a02577d6290)

- Output result

  ![Screenshot 2024-09-11 190954-1](https://github.com/user-attachments/assets/fa2d0520-2991-4d12-8e7e-e0ef964f438a)

<br>
<br>

> b. Berapa byte file response yang dikirim dari server

> _b. How many bytes of file response are sent from the server?_


**Answer:**

- Flag

  `JARKOM24{Y0u_4r3_4_g00d_4nalyz3r_E447XL1tsbjwgvsnlprllzoalscdlji}`

- Filter expression

  `http`
  
- Explanation

  `Setelah melakukan filter, klik packet kedua, akan muncul informasi "427 bytes on wire (3416 bits), 427 bytes captured (3416 bits) on interface" yang berarti byte file yang dikirim dari server adalah 427`
  <br>
  ![WhatsApp Image 2024-09-12 at 23 32 27](https://github.com/user-attachments/assets/b6de1f00-e556-4207-aa4f-6a653043ba98)

- Output result

  ![Screenshot 2024-09-11 190954-1](https://github.com/user-attachments/assets/fa2d0520-2991-4d12-8e7e-e0ef964f438a)

<br>
<br>

> c. Berapa jumlah file yang terdapat pada server?

> _c. How many files are there on the server?_


**Answer:**

- Flag

  `JARKOM24{Y0u_4r3_4_g00d_4nalyz3r_E447XL1tsbjwgvsnlprllzoalscdlji}`

- Filter expression

  `http`
  
- Explanation

  `ctrl + alt + shift + t pada salah satu packet setelah melakukan filtering. Terdapat informasi jumlah file pada server http, yaitu 4`
  <br>
  ![WhatsApp Image 2024-09-12 at 23 33 56](https://github.com/user-attachments/assets/fd60e5c5-7aa6-419f-88eb-003b699725cc)

- Output result

  ![Screenshot 2024-09-11 190954-1](https://github.com/user-attachments/assets/fa2d0520-2991-4d12-8e7e-e0ef964f438a)

<br>
<br>

> d. Sebutkan nama file secara berurutan berdasarkan alfabet menurun dengan koma sebagai separator, contoh: file1,file2

> _d. List the filenames in descending alphabetical order, separated by commas. Example: file1,file2_


**Answer:**

- Flag

  `JARKOM24{Y0u_4r3_4_g00d_4nalyz3r_E447XL1tsbjwgvsnlprllzoalscdlji}`

- Filter expression

  `http`
  
- Explanation

  `ctrl + alt + shift + t pada salah satu packet setelah melakukan filtering. Terdapat informasi jumlah file pada server http, yaitu 4. File-file tersebut adalah file.pdf, hello.html, lion.jpg, dan present.pptx yang terdapat di dalam text/html. File tersebut sudah tersusun secara alfabet menurun`
  <br>
  ![WhatsApp Image 2024-09-12 at 23 33 56](https://github.com/user-attachments/assets/f45303a9-77a7-43ff-89f1-87c6e3193e58)

- Output result

  ![Screenshot 2024-09-11 190954-1](https://github.com/user-attachments/assets/fa2d0520-2991-4d12-8e7e-e0ef964f438a)

<br>
<br>

## Task 4

> Protokol apa yang paling banyak terdapat di file hasil capture traffic?

> _Which protocol is the most frequent in the traffic capture file?_


**Answer:**

- Flag

  `JARKOM24{M4ster_4n4lyzer_64328t1k1WQAILQDDMAR41sk3jswqtu10}`

- Filter expression

  `None (-)`
  
- Explanation

  `Klik "Statistics" kemudian pilih "Protocol Hierarchy", terdapat informasi bahwa semua packetnya berbasis FTP yang berarti protokol paling banyak di file hasil capture traffic adalah FTP`
  <br>
  ![image](https://github.com/user-attachments/assets/67f1d8e7-324f-4923-9e54-54329cea8c1d)

- Output result

  ![Screenshot 2024-09-11 185216](https://github.com/user-attachments/assets/f4a29bde-bc2c-4d09-89d1-e630920d6448)

<br>
<br>

## Task 5

> Berdasarkan hasil bruteforce, apa user yang tepat dari hasil bruteforce?

> _Based on the brute force results, what is the correct username?_


**Answer:**

- Flag

  `JARKOM24{He_1s_g3d4g3d1g3d4g3d40_OZERQZHLGAWZUIKJYIFNMunskydzruqmdwwst459454446784}`

- Filter expression

  `tcp contains "successful"`
  
- Explanation

  `Di awal, saya mencari secara manual packet yang memiliki info 'Login successful'. Kemudian, kepikiran bisa menggunakan filter. Setelah menemukan packet tersebut, packet nomor 260, klik ctrl + alt + shift + t dan akan muncul informasi lebih lanjutnya. Terdapat informasi user adalah gedagedigedagedao`
  <br>
  ![image](https://github.com/user-attachments/assets/1d6b24ef-d4dd-4036-9213-0faafc8c3323)

- Output result

  ![Screenshot 2024-09-11 185610](https://github.com/user-attachments/assets/db0b26cb-2dd3-4815-bea0-f03fcb3aad4c)

<br>
<br>

## Task 6

> Apa password yang tepat?

> _What is the correct password?_


**Answer:**

- Flag

  `JARKOM24{h1s_fr1end_1s_g3d4g3d1g3d4g3d03_L8TRNDH2UOyksnUmcysnghafdcB4Sur1QCHKVLVIUU}`

- Filter expression

  `tcp contains "successful"`
  
- Explanation

  `Di awal, saya mencari secara manual packet yang memiliki info 'Login successful'. Kemudian, kepikiran bisa menggunakan filter. Setelah menemukan packet tersebut, packet nomor 260, klik ctrl + alt + shift + t dan akan muncul informasi lebih lanjutnya. Terdapat informasi pass adalah gedagedigedagedoe`
  <br>
   ![image](https://github.com/user-attachments/assets/1d6b24ef-d4dd-4036-9213-0faafc8c3323)

- Output result

  ![Screenshot 2024-09-11 185715](https://github.com/user-attachments/assets/7b87a987-e9fb-460e-ab48-6e3ee02399c2)

<br>
<br>

## Task 7

> Pada port berapa telnet yang bisa diakses?

> _On which port is Telnet accessible?_


**Answer:**

- Flag

  `JARKOM24{Gr34t_Sn1ff3r_B1P88yksnUmye2rpy76r2T3t0t4h0eqNXPaH}`

- Filter expression

  `tcp contains "telnet"`
  
- Explanation

  `Setelah melakukan filter, dapat dilihat destination port packet paling atas adalah 2423 yang merupakan destination port dari telnet`
  <br>
  ![image](https://github.com/user-attachments/assets/45a2cd75-eb36-4691-9c59-fdc26f6579c7)

- Output result

  ![Screenshot 2024-09-11 191425](https://github.com/user-attachments/assets/41c7c44d-3a66-4850-bd92-9d51e5d4055a)

<br>
<br>

## Task 8

> Ada berapa file di dalam server?

> _How many files are on the server?_


**Answer:**

- Flag

  `JARKOM24{P4ck3t_4n4lyz3r_7y60hMlLEI3112pagvnxdbbdS1SLDCESQNIRB}`

- Filter expression

  `tcp contains "telnet"`
  
- Explanation

  `ctrl + alt + shift + t pada packet ketiga. Scroll informasinya, akan terlihat user mengetik ls dan server menampilkan 7 nama file (chakra.txt, code07.txt, djumanto.txt, dongsoo.txt, echo, gendra.txt, dan junggoo.txt)`
  <br>
  ![image](https://github.com/user-attachments/assets/19fd8321-0ad2-4240-95a2-280945306b83)

- Output result

  ![Screenshot 2024-09-11 190605](https://github.com/user-attachments/assets/15a9c4cd-fd7d-4f41-a4f7-244f5316769b)

<br>
<br>

## Task 9

> Apa nama file yang dieksekusi oleh user?

> _What is the name of the file executed by the user?_


**Answer:**

- Flag

  `JARKOM24{333ch000_us3r_045334587112NBlAUbKrxmd33dHL84NDJML6}`

- Filter expression

  `tcp contains "telnet"`
  
- Explanation

  `ctrl + alt + shift + t pada packet ketiga. Scroll informasinya, akan terlihat user mengetik "./echo". Saat praktikum sisop semester lalu, file dieksekusi dengan command "./(nama file)". Jadi, file yang dieksekusi oleh user adalah "echo". Soal ini juga bisa diselesaikan dengan mencoba menginput semua nama filenya :D`
  <br>
  ![image](https://github.com/user-attachments/assets/f1ac1011-197d-4ec5-adc4-5d5f59851219)

- Output result

  ![Screenshot 2024-09-11 195851](https://github.com/user-attachments/assets/136fb01e-07a1-4fa0-9c30-47dcfcb190fa)

<br>
<br>

## Task 10

> Apa output dari file dalam bentuk base64 decode?

> _What is the output of the file in base64-decoded form?_


**Answer:**

- Flag

  `JARKOM24{tH4ts_1t_w3ll_d0n3_21796080151337c2bl6ecdwl12314214213NBBTLEBCUMZZZ0}`

- Filter expression

  `tcp contains "telnet"`
  
- Explanation

  `ctrl + alt + shift + t pada packet ketiga. Scroll informasinya, akan terlihat hasil output dari "./echo" yaitu`
  <br>
  ![image](https://github.com/user-attachments/assets/53a4abb3-6069-47f2-86a9-dadd8eb463a7)
  <br>
  `Kemudian, decode teks tersebut melalui website "Base64 Decode"`

- Output result

  ![Screenshot 2024-09-11 202924](https://github.com/user-attachments/assets/f26b2c8a-7302-4288-8b8b-a1136abc3a04)

<br>
<br>

## Summary
Berdasarkan praktikum 1 wireshark kali ini, kami mengerjakan beberapa soal yang:

1. Mencari jumlah paket yang terekam
2. Mencari jenis protokol yang digunakan (termasuk protokol yang paling banyak digunakan)
3. Mencari flag pada paket TCP
4. Mencari port yang terbuka oleh server HTTP
5. Mencari ukuran file yang dikirim oleh server sekaligus nama file-nya
6. Mencari port telnet yang terbuka
7. Mencari username dan password dari hasil bruteforce
8. Mencari file yang dieksekusi oleh user
9. Mencari dan mendekode output dari file yang dieksekusi dalam format base64

## Problems
Sejauh ini, belum menemukan problem atau permasalahan yang signifikan dalam mengerjakan soal praktikum 1 wireshark
