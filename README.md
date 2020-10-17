# Jarkom_Modul1_Lapres_D11
Lapres praktikum jarkom modul 1 kelompok D11
## Nomor 1
Sebutkan webserver yang digunakan pada "testing.mekanis.me"!

## Nomor 2
Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!

- Petama kita cari dengan cara export object HTTP
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/2.png" >

- Kedua ketik pada text filter "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/2a.PNG">

- Setelah didownload lalu buka file .jpg dan akan terlihat gambarnya

<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/2b.PNG">

## Nomor 6
Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).

- Pertama kita menggunakan find packet untuk mencari " zipkey.txt "
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/6a.PNG">

- Lalu pada “zipkey.txt” , di follow stream tcp sehingga memunculkan password yang akan digunakan untuk mengekstrak file “Answer.zip”
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/6b.PNG">

- Lalu kita menggunakan find packet untuk mencari " Answer.zip "
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/6c.PNG">

- Lalu pada “Answer.zip” , di follow stream tcp lalu pada show and save data kita ubah menjadi raw dan setelah itu kita save
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/6d.PNG">

- Setelah kita save file " Answer.zip " kita extract dengan password yang ada pada " zipkey.txt " dan muncul file " Open This.pdf "
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/6e.PNG">

- Dan ini adalah isi dari " Open This.pdf "
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/6f.PNG">

## Nomor 9
Cari username dan password ketika login FTP pada localhost!

- Untuk mencari username menggunakan ftp.request.command == USER
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/9a.PNG">

- Untuk mencari password menggunakan ftp.request.command == PASS
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/9b.PNG">

## Nomor 10
Cari file .pdf di wireshark lalu download dan buka file tersebut!
clue: "25 50 44 46" 

- Untuk mencari file .pdf kita menggunakan frame contains "application/pdf"
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/10a.PNG">

- Setelah menemukan hasil dari filter , di follow stream tcp lalu pada show and save data kita ubah menjadi raw dan setelah itu kita save
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/10b.PNG">

- Lalu buka file .pdf yang sudah di save tadi
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/10c.PNG">


## Nomor 13

## Nomor 15

