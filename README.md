# Jarkom_Modul1_Lapres_D11
Lapres praktikum jarkom modul 1 kelompok D11
## Nomor 1
Sebutkan webserver yang digunakan pada "testing.mekanis.me"!

- Pertama, kita filter menggunakan http.host=="testing.mekanis.me" lalu pilih salah satu paketnya
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/nomor1a.JPG" >

- Kemudian, klik kanan, lalu pilih follow, dan klik TCP stream. Web server yang digunakan adalah nginx seperti yang terlihat pada gambar
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/nomor1.JPG" >

## Nomor 2
Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!

- Petama kita cari dengan cara export object HTTP
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/2.png" >

- Kedua ketik pada text filter "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/2a.PNG">

- Setelah didownload lalu buka file .jpg dan akan terlihat gambarnya

<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/2b.PNG">

## Nomor 3
Cari username dan password ketika login di "ppid.dpr.go.id"!

- Menggunakan display filter, ketik http.host=="ppid.dpr.go.id", lalu pilih paket yang method nya POST. Username adalah "10pemuda" dan password adalah "guncangdunia"
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/3.JPG">

## Nomor 4
Temukan paket dari web-web yang menggunakan basic authentication method!

- Menggunakan display filter, ketik "http.authbasic", maka akan terlihat paket dari web-web yang menggunakan basic authentication
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/4.JPG">

## Nomor 5
Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!

- Menggunakan display filter, ketik http.host=="aku.pengen.pw", lalu buka salah satu paket, dan terlihat username dan password untuk login adalah seperti yang tertera di gambar
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/5.JPG">

- Kemudian login di aku.pengen.pw dan hasilnya adalah seperti gambar dibawah
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/5b.JPG">

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

## Nomor 7
Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf"

- Gunakan syntax frame contains "Yes.pdf", kemudian pilih paket yang paling atas, kemudian klik kanan, pilih follow kemudian TCP stream
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/7a.JPG">

- Kemudian save paket tersebut sebagai file .zip
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/7b.JPG">

- Kemudian extract file .zip tersebut dan buka folder Yes.pdf
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/7c.JPG">

## Nomor 9
Cari username dan password ketika login FTP pada localhost!

- Untuk mencari username menggunakan ftp.request.command == USER
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/9a.PNG">

- Untuk mencari password menggunakan ftp.request.command == PASS
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/9b.PNG">

## Nomor 10
Cari file .pdf di wireshark lalu download dan buka file tersebut!
clue: "25 50 44 46" 

- Untuk mencari file .pdf kita menggunakan perintah frame contains "application/pdf"
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/10a.PNG">

- di follow stream tcp lalu pada show and save data kita ubah menjadi raw dan setelah itu kita save .pdf
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/10b.PNG">

- Ini adalah isi dari Nomer 10.pdf
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/10c.PNG">

## Nomor 13
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!

- Menggunakan command tcp dst port 443
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/13.PNG">

## Nomor 15
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!

- Menggunakan command dst host monta.if.its.ac.id
<img src="https://github.com/pangestuf/Jarkom_Modul1_Lapres_D11/blob/main/Gambar/15.PNG">

