# SoalShift_modul1_C12

5. Buatlah sebuah script bash untuk menyimpan record dalam syslog yang memenuhi
kriteria berikut:

a. Tidak mengandung string “sudo”, tetapi mengandung string “cron”,
serta buatlah pencarian stringnya tidak bersifat case sensitive,
sehingga huruf kapital atau tidak, tidak menjadi masalah.

![5a - shift 1](https://user-images.githubusercontent.com/47876805/53219667-7571de80-3693-11e9-852f-599b239beb2d.png) 

Ketika di bash maka hasilnya akan seperti ini:
![5a bash - shift 1](https://user-images.githubusercontent.com/47876805/53219666-7571de80-3693-11e9-8054-ddf44fc79a9f.png) 

b. Jumlah field (number of field) pada baris tersebut berjumlah kurang
dari 13.

![5b - shift 1](https://user-images.githubusercontent.com/47876805/53219669-760a7500-3693-11e9-94bd-353ac84723af.png) 

Ketika di bash maka hasilnya akan seperti ini:
![5b bash - shift 1](https://user-images.githubusercontent.com/47876805/53219668-760a7500-3693-11e9-9713-79b7a6531c87.png) 

c. Masukkan record tadi ke dalam file logs yang berada pada direktori

![5c - shift 1](https://user-images.githubusercontent.com/47876805/53219672-76a30b80-3693-11e9-9c3c-411e83351fcf.png) 

Maka hasilnya akan terlihat terbentuk file bernama soal5.log yang berisi:


d. Jalankan script tadi setiap 6 menit dari menit ke 2 hingga 30, contoh
13:02, 13:08, 13:14, dst.

Maka kita merubah settingan crontab dengan cara crontab -e, lalu kita ubah menjadi seperti ini:
![5d - shift 1](https://user-images.githubusercontent.com/47876805/53219673-76a30b80-3693-11e9-9a99-4403c384e01d.png)

Setelah itu, kita tunggu sampai terdapat file bernama soal5.log. Kalau file tersebut sudah ada berarti crontab kita sudah berhasil.
